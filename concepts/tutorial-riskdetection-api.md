---
title: 'Tutorial: identificar e corrigir riscos usando as APIs do Microsoft Graph'
description: Saiba como identificar e corrigir riscos usando as APIs do Microsoft Graph.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0bec8dc51c81b9d2d0349294c0f0d1f6bd4c1e98
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664163"
---
# <a name="tutorial-identify-and-remediate-risks-using-microsoft-graph-apis"></a><span data-ttu-id="330c3-103">Tutorial: identificar e corrigir riscos usando as APIs do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="330c3-103">Tutorial: Identify and remediate risks using Microsoft Graph APIs</span></span>

<span data-ttu-id="330c3-104">O Azure AD Identity Protection fornece às organizações informações sobre riscos baseados em identidade e diferentes maneiras de investigar e corrigir automaticamente o risco.</span><span class="sxs-lookup"><span data-stu-id="330c3-104">Azure AD Identity Protection provides organizations insight into identity-based risk and different ways to investigate and automatically remediate risk.</span></span> <span data-ttu-id="330c3-105">As APIs de proteção de identidade usadas neste tutorial podem ajudá-lo a identificar riscos e configurar um fluxo de trabalho para confirmar o comprometimento ou habilitar a correção.</span><span class="sxs-lookup"><span data-stu-id="330c3-105">The Identity Protection APIs used in this tutorial can help you identify risk and configure a workflow to confirm compromise or enable remediation.</span></span> <span data-ttu-id="330c3-106">Para obter mais informações, consulte [o que é risco?](/azure/active-directory/identity-protection/concept-identity-protection-risks)</span><span class="sxs-lookup"><span data-stu-id="330c3-106">For more information, see [What is risk?](/azure/active-directory/identity-protection/concept-identity-protection-risks)</span></span>

<span data-ttu-id="330c3-107">Neste tutorial, você aprenderá a gerar um usuário arriscado e a corrigir o status arriscado do usuário com uma política de acesso condicional que requer autenticação multifator (MFA).</span><span class="sxs-lookup"><span data-stu-id="330c3-107">In this tutorial, you learn how to generate a risky user and remediate the risky status of the user with a conditional access policy that requires multi-factor authentication (MFA).</span></span> <span data-ttu-id="330c3-108">Uma seção opcional mostra como bloquear o usuário de entrar também usando uma política de acesso condicional e descartar o risco do usuário.</span><span class="sxs-lookup"><span data-stu-id="330c3-108">An optional section shows you how to block the user from signing in also using a conditional access policy, and dismissing the user risk.</span></span>

><span data-ttu-id="330c3-109">**Observação:** Os objetos de resposta mostrados neste tutorial podem ser reduzidos para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="330c3-109">**Note:** The response objects shown in this tutorial might be shortened for readability.</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="330c3-110">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="330c3-110">Prerequisites</span></span>

<span data-ttu-id="330c3-111">Para concluir com êxito este tutorial, verifique se você tem os pré-requisitos necessários:</span><span class="sxs-lookup"><span data-stu-id="330c3-111">To successfully complete this tutorial, make sure that you have the required prerequisites:</span></span>

- <span data-ttu-id="330c3-112">Você deve ter uma licença do Azure AD Premium P1 ou P2 para usar a API de detecção de risco.</span><span class="sxs-lookup"><span data-stu-id="330c3-112">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>
- <span data-ttu-id="330c3-113">Este tutorial usa o navegador do Tor para entrar no portal do Azure anonimamente.</span><span class="sxs-lookup"><span data-stu-id="330c3-113">This tutorial uses the Tor browser to sign in to the Azure portal anonymously.</span></span> <span data-ttu-id="330c3-114">Você pode usar qualquer navegador anônimo para realizar a tarefa.</span><span class="sxs-lookup"><span data-stu-id="330c3-114">You can use any anonymous browser to accomplish the task.</span></span> <span data-ttu-id="330c3-115">Para baixar o navegador do Tor, consulte [Download Tor browser](https://www.torproject.org/download/).</span><span class="sxs-lookup"><span data-stu-id="330c3-115">To download the Tor browser, see [Download Tor Browser](https://www.torproject.org/download/).</span></span>
- <span data-ttu-id="330c3-116">Este tutorial pressupõe que você está usando o Microsoft Graph Explorer, mas você pode usar o postmaster ou criar seu próprio aplicativo cliente para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="330c3-116">This tutorial assumes that you are using Microsoft Graph Explorer, but you can use Postman, or create your own client app to call Microsoft Graph.</span></span> <span data-ttu-id="330c3-117">Para chamar as APIs do Microsoft Graph neste tutorial, você precisa usar uma conta com a função de administrador global e as permissões apropriadas.</span><span class="sxs-lookup"><span data-stu-id="330c3-117">To call the Microsoft Graph APIs in this tutorial, you need to use an account with the global administrator role and the appropriate permissions.</span></span> <span data-ttu-id="330c3-118">Conclua as seguintes etapas para definir permissões no Microsoft Graph Explorer:</span><span class="sxs-lookup"><span data-stu-id="330c3-118">Complete the following steps to set permissions in Microsoft Graph Explorer:</span></span>
    1. <span data-ttu-id="330c3-119">Iniciar [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="330c3-119">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
    2. <span data-ttu-id="330c3-120">Selecione **entrar com a Microsoft** e entre usando uma conta de administrador global do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="330c3-120">Select **Sign-In with Microsoft** and sign in using an Azure AD global administrator account.</span></span> <span data-ttu-id="330c3-121">Após entrar com êxito, você poderá ver os detalhes da conta de usuário no painel esquerdo.</span><span class="sxs-lookup"><span data-stu-id="330c3-121">After you successfully sign in, you can see the user account details in the left-hand pane.</span></span>
    3. <span data-ttu-id="330c3-122">Selecione o ícone de configurações à direita dos detalhes da conta de usuário e selecione **permissões**.</span><span class="sxs-lookup"><span data-stu-id="330c3-122">Select the settings icon to the right of the user account details, and then select **Select permissions**.</span></span>

        ![Definir permissões](./images/tutorial-riskdetection-api/set-permissions.png)
        
    4. <span data-ttu-id="330c3-124">Role a lista de permissões para estas permissões:</span><span class="sxs-lookup"><span data-stu-id="330c3-124">Scroll through the list of permissions to these permissions:</span></span>
        - <span data-ttu-id="330c3-125">**IdentityRiskEvents (2)**, expanda e selecione `IdentityRiskEvent.Read.All`</span><span class="sxs-lookup"><span data-stu-id="330c3-125">**IdentityRiskEvents (2)**, expand and then select `IdentityRiskEvent.Read.All`</span></span>
        - <span data-ttu-id="330c3-126">**Identityriskuser (2)**, expanda e selecione `IdentityRiskyUser.ReadWrite.All`</span><span class="sxs-lookup"><span data-stu-id="330c3-126">**IdentityRiskyUser (2)**, expand and then select `IdentityRiskyUser.ReadWrite.All`</span></span>
        - <span data-ttu-id="330c3-127">**Política (13)**, expanda e, em seguida, selecione `Policy.Read.All` e `Policy.ReadWrite.ConditionalAccess`</span><span class="sxs-lookup"><span data-stu-id="330c3-127">**Policy (13)**, expand and then select `Policy.Read.All` and `Policy.ReadWrite.ConditionalAccess`</span></span>
        - <span data-ttu-id="330c3-128">**Usuário (8)**, expanda e selecione `User.ReadWrite.All`</span><span class="sxs-lookup"><span data-stu-id="330c3-128">**User (8)**, expand and then select `User.ReadWrite.All`</span></span>
        
        ![Pesquisar permissões](./images/tutorial-riskdetection-api/permissions-consent.png)
    
    5. <span data-ttu-id="330c3-130">Selecione **consentimento** e, em seguida, selecione **aceitar** para aceitar o consentimento das permissões.</span><span class="sxs-lookup"><span data-stu-id="330c3-130">Select **Consent**, and then select **Accept** to accept the consent of the permissions.</span></span> <span data-ttu-id="330c3-131">Você não precisa consentir em nome da sua organização para essas permissões.</span><span class="sxs-lookup"><span data-stu-id="330c3-131">You do not need to consent on behalf of your organization for these permissions.</span></span>

        ![Aceitar permissões](./images/tutorial-riskdetection-api/accept-permissions.png)

## <a name="step-1-create-a-user-account"></a><span data-ttu-id="330c3-133">Etapa 1: criar uma conta de usuário</span><span class="sxs-lookup"><span data-stu-id="330c3-133">Step 1: Create a user account</span></span>

<span data-ttu-id="330c3-134">Para este tutorial, você cria uma conta de usuário que é usada para testar as detecções de risco.</span><span class="sxs-lookup"><span data-stu-id="330c3-134">For this tutorial, you create a user account that is used to test risk detections.</span></span> <span data-ttu-id="330c3-135">No corpo da solicitação, mude `contoso.com` para o nome de domínio do seu locatário.</span><span class="sxs-lookup"><span data-stu-id="330c3-135">In the request body, change `contoso.com` to the domain name of your tenant.</span></span> <span data-ttu-id="330c3-136">Você pode encontrar informações sobre o locatário na página Visão geral do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="330c3-136">You can find tenant information on the Azure Active Directory overview page.</span></span>

### <a name="request"></a><span data-ttu-id="330c3-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="330c3-137">Request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "accountEnabled":true,
  "displayName":"MyTestUser1",
  "mailNickname":"MyTestUser1",
  "userPrincipalName":"MyTestUser1@contoso.com",
  "passwordProfile": {
    "forceChangePasswordNextSignIn":true,
    "password":"Contoso1234"
  }
}
```

### <a name="response"></a><span data-ttu-id="330c3-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="330c3-138">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
  "id": "4628e7df-dff3-407c-a08f-75f08c0806dc",
  "businessPhones": [],
  "displayName": "MyTestUser1",
  "givenName": null,
  "jobTitle": null,
  "mail": null,
  "mobilePhone": null,
  "officeLocation": null,
  "preferredLanguage": null,
  "surname": null,
  "userPrincipalName": "MyTestUser1@contoso.com"
}
```

## <a name="step-2-trigger-a-risk-detection"></a><span data-ttu-id="330c3-139">Etapa 2: disparar uma detecção de risco</span><span class="sxs-lookup"><span data-stu-id="330c3-139">Step 2: Trigger a risk detection</span></span>

### <a name="trigger-a-risk-detection"></a><span data-ttu-id="330c3-140">Acionar uma detecção de risco</span><span class="sxs-lookup"><span data-stu-id="330c3-140">Trigger a risk detection</span></span>

<span data-ttu-id="330c3-141">Uma maneira de acionar uma detecção de risco em uma conta de usuário é fazer logon no portal do Azure anonimamente.</span><span class="sxs-lookup"><span data-stu-id="330c3-141">One way to trigger a risk detection on a user account is to sign in to the Azure portal anonymously.</span></span> <span data-ttu-id="330c3-142">Neste tutorial, o navegador do Tor é usado para entrar anonimamente.</span><span class="sxs-lookup"><span data-stu-id="330c3-142">In this tutorial, the Tor browser is used to sign in anonymously.</span></span> 

1. <span data-ttu-id="330c3-143">Abra o navegador e insira `portal.azure.com` o endereço do site.</span><span class="sxs-lookup"><span data-stu-id="330c3-143">Open the browser and enter `portal.azure.com` for the site address.</span></span>
2. <span data-ttu-id="330c3-144">Entre no portal usando as credenciais da conta do **MyTestUser1** que você criou anteriormente.</span><span class="sxs-lookup"><span data-stu-id="330c3-144">Sign in to the portal using the credentials for the **MyTestUser1** account that you previously created.</span></span> <span data-ttu-id="330c3-145">Você será solicitado a alterar a senha existente.</span><span class="sxs-lookup"><span data-stu-id="330c3-145">You will be asked to change the existing password.</span></span>

### <a name="list-risk-detections"></a><span data-ttu-id="330c3-146">Listar detecções de riscos</span><span class="sxs-lookup"><span data-stu-id="330c3-146">List risk detections</span></span>

<span data-ttu-id="330c3-147">Quando você entrou no portal do Azure usando o navegador anônimo, um `anonymizedIPAddress` evento de risco foi detectado.</span><span class="sxs-lookup"><span data-stu-id="330c3-147">When you signed in to the Azure portal using the anonymous browser, an `anonymizedIPAddress` risk event was detected.</span></span> <span data-ttu-id="330c3-148">Você pode usar o `$filter` parâmetro de consulta para obter apenas as detecções de risco associadas à conta de usuário **MyTestUser1** .</span><span class="sxs-lookup"><span data-stu-id="330c3-148">You can use the `$filter` query parameter to get only the risk detections that are associated with the **MyTestUser1** user account.</span></span>

#### <a name="request"></a><span data-ttu-id="330c3-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="330c3-149">Request</span></span>

``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskDetections?$filter=userDisplayName eq 'MyTestUser1'
```

#### <a name="response"></a><span data-ttu-id="330c3-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="330c3-150">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#riskDetections",
  "value": [
    {
      "id": "d52a631815aaa527bf642b196715da5cf0f35b6879204ea5b5c99b21bd4c16f4",
      "requestId": "06f7fd18-b8f1-407d-86a3-f6cbe3a4be00",
      "correlationId": "2a38abff-5701-4073-a81e-fd3aac09cba3",
      "riskType": "anonymizedIPAddress",
      "riskEventType": "anonymizedIPAddress",
      "riskState": "atRisk",
      "riskLevel": "medium",
      "riskDetail": "none",
      "source": "IdentityProtection",
      "detectionTimingType": "realtime",
      "activity": "signin",
      "tokenIssuerType": "AzureAD",
      "ipAddress": "178.17.170.23",
      "activityDateTime": "2020-11-03T20:51:34.6245276Z",
      "detectedDateTime": "2020-11-03T20:51:34.6245276Z",
      "lastUpdatedDateTime": "2020-11-03T20:53:12.1984203Z",
      "userId": "4628e7df-dff3-407c-a08f-75f08c0806dc",
      "userDisplayName": "MyTestUser1",
      "userPrincipalName": "MyTestUser1@contoso.com",
      "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; rv:78.0) Gecko/20100101 Firefox/78.0\"}]",
      "location": {
        "city": "Chisinau",
        "state": "Chisinau",
        "countryOrRegion": "MD",
        "geoCoordinates": {
          "latitude": 47.0269,
          "longitude": 28.8416
        }
      }
    }
  ]
}
```

> <span data-ttu-id="330c3-151">**Observação:** Pode levar alguns minutos até que o evento seja retornado.</span><span class="sxs-lookup"><span data-stu-id="330c3-151">**Note:** It may take a few minutes for the event to be returned.</span></span>

## <a name="step-3-create-a-conditional-access-policy"></a><span data-ttu-id="330c3-152">Etapa 3: criar uma política de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="330c3-152">Step 3: Create a conditional access policy</span></span>

<span data-ttu-id="330c3-153">Você pode aproveitar as políticas de acesso condicional em sua organização para permitir que os usuários façam a correção automática quando o risco for detectado.</span><span class="sxs-lookup"><span data-stu-id="330c3-153">You can leverage conditional access policies in your organization to allow users to self-remediate when risk is detected.</span></span> <span data-ttu-id="330c3-154">A AutoCorreção permite que os usuários se desbloqueiem para acessar seus recursos de forma segura após a conclusão do prompt da política.</span><span class="sxs-lookup"><span data-stu-id="330c3-154">Self-remediation enables your users to unblock themselves to access their resources securely after completing the policy prompt.</span></span> <span data-ttu-id="330c3-155">Nesta etapa, você criará uma política de acesso condicional que requer que o usuário entre usando a MFA se ocorrer uma detecção de alto risco.</span><span class="sxs-lookup"><span data-stu-id="330c3-155">In this step, you create a conditional access policy that requires the user to sign in using MFA if a medium or high risk detection occurs.</span></span>

### <a name="set-up-multi-factor-authentication"></a><span data-ttu-id="330c3-156">Configurar a autenticação multifator</span><span class="sxs-lookup"><span data-stu-id="330c3-156">Set up multi-factor authentication</span></span>

<span data-ttu-id="330c3-157">Ao configurar uma conta para a MFA, você pode escolher entre vários métodos para autenticar o usuário.</span><span class="sxs-lookup"><span data-stu-id="330c3-157">When setting up an account for MFA, you can choose from several methods for authenticating the user.</span></span> <span data-ttu-id="330c3-158">Escolha o melhor método para a sua situação para concluir este tutorial.</span><span class="sxs-lookup"><span data-stu-id="330c3-158">Choose the best method for your situation to complete this tutorial.</span></span> 

1. <span data-ttu-id="330c3-159">Entre no para [manter seu site seguro de conta](https://aka.ms/MFASetup) usando a conta **MyTestUser1** .</span><span class="sxs-lookup"><span data-stu-id="330c3-159">Sign in the to the [keep your account secure](https://aka.ms/MFASetup) site using the **MyTestUser1** account.</span></span>
2. <span data-ttu-id="330c3-160">Conclua o procedimento de configuração da MFA usando o método apropriado para a sua situação, como ter uma mensagem de texto enviada ao seu telefone.</span><span class="sxs-lookup"><span data-stu-id="330c3-160">Complete the MFA setup procedure using the appropriate method for your situation, such as having a text message sent to your phone.</span></span>

### <a name="create-the-conditional-access-policy"></a><span data-ttu-id="330c3-161">Criar a política de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="330c3-161">Create the conditional access policy</span></span>

<span data-ttu-id="330c3-162">A política de acesso condicional fornece a capacidade de definir as condições da política para identificar os níveis de risco de entrada.</span><span class="sxs-lookup"><span data-stu-id="330c3-162">The conditional access policy provides the ability to set the conditions of the policy to identify sign-in risk levels.</span></span> <span data-ttu-id="330c3-163">Os níveis de risco podem ser `low` , `medium` , `high` , `none` .</span><span class="sxs-lookup"><span data-stu-id="330c3-163">Risk levels can be `low`, `medium`, `high`, `none`.</span></span> <span data-ttu-id="330c3-164">Na resposta retornada pela listar as detecções de risco para o **MyTestUser1**, podemos ver que o nível de risco é `medium` .</span><span class="sxs-lookup"><span data-stu-id="330c3-164">In the response that was returned from listing the risk detections for **MyTestUser1**, we can see that the risk level is `medium`.</span></span> <span data-ttu-id="330c3-165">Este exemplo mostra como exigir a MFA de **MyTestUser1** que foi identificada como um usuário arriscado.</span><span class="sxs-lookup"><span data-stu-id="330c3-165">This example shows how to require MFA for **MyTestUser1** who was identified as a risky user.</span></span>

#### <a name="request"></a><span data-ttu-id="330c3-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="330c3-166">Request</span></span> 

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies 
Content-type: application/json
 
{ 
  "displayName": "Policy for risky sign-in", 
  "state": "enabled", 
  "conditions": { 
    "signInRiskLevels": [ 
      "high", 
      "medium" 
    ], 
    "applications": { 
      "includeApplications": ["All"]
    }, 
    "users": { 
      "includeUsers": [ 
        "4628e7df-dff3-407c-a08f-75f08c0806dc" 
      ] 
    } 
  }, 
  "grantControls": { 
    "operator": "OR", 
    "builtInControls": [ 
      "mfa" 
    ] 
  } 
} 
```

#### <a name="response"></a><span data-ttu-id="330c3-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="330c3-167">Response</span></span> 

```
{ 
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/conditionalAccess/policies/$entity", 
  "id": "9ad78153-b1f8-4714-adc1-1445727678a8", 
  "displayName": "Policy for risky sign-in", 
  "createdDateTime": "2020-11-03T20:56:38.6210843Z", 
  "modifiedDateTime": null, 
  "state": "enabled", 
  "sessionControls": null, 
  "conditions": { 
    "signInRiskLevels": [ 
      "high", 
      "medium" 
    ], 
    "clientAppTypes": [  
      "all"  
    ], 
    "platforms": null, 
    "locations": null, 
    "applications": { 
      "includeApplications": [ 
        "All" 
      ], 
      "excludeApplications": [], 
      "includeUserActions": [] 
    }, 
    "users": { 
      "includeUsers": [ 
        "4628e7df-dff3-407c-a08f-75f08c0806dc" 
      ], 
      "excludeUsers": [], 
      "includeGroups": [], 
      "excludeGroups": [], 
      "includeRoles": [], 
      "excludeRoles": [] 
    } 
  }, 
  "grantControls": { 
    "operator": "OR", 
    "builtInControls": [ 
      "mfa" 
    ], 
    "customAuthenticationFactors": [], 
    "termsOfUse": [] 
  } 
} 
```

<span data-ttu-id="330c3-168">Com essa política de acesso condicional in-loco, a conta **MyTestUser1**   agora é necessária para usar MFA ao entrar porque o nível de risco de entrada é médio ou alto.</span><span class="sxs-lookup"><span data-stu-id="330c3-168">With this conditional access policy in place, the **MyTestUser1** account is now required to use MFA when signing in because the sign-in risk level is medium or high.</span></span> 

### <a name="sign-in-and-complete-multi-factor-authentication"></a><span data-ttu-id="330c3-169">Entrar e concluir a autenticação multifator</span><span class="sxs-lookup"><span data-stu-id="330c3-169">Sign in and complete multi-factor authentication</span></span> 

<span data-ttu-id="330c3-170">Ao entrar no navegador anônimo, um risco é detectado, mas é corrigido pela conclusão da MFA.</span><span class="sxs-lookup"><span data-stu-id="330c3-170">By signing in to the anonymous browser, a risk is detected, but it is remediated by completing MFA.</span></span> 

1. <span data-ttu-id="330c3-171">Abra o navegador e insira  `portal.azure.com`   o endereço do site.</span><span class="sxs-lookup"><span data-stu-id="330c3-171">Open the browser and enter `portal.azure.com` for the site address.</span></span> 
2. <span data-ttu-id="330c3-172">Entre no portal usando as credenciais da conta **MyTestUser1**   e conclua o processo de MFA.</span><span class="sxs-lookup"><span data-stu-id="330c3-172">Sign in to the portal using the credentials for the **MyTestUser1** account and complete the MFA process.</span></span> 

### <a name="list-risk-detections"></a><span data-ttu-id="330c3-173">Listar detecções de riscos</span><span class="sxs-lookup"><span data-stu-id="330c3-173">List risk detections</span></span>

<span data-ttu-id="330c3-174">Porque a MFA foi concluída.</span><span class="sxs-lookup"><span data-stu-id="330c3-174">Because MFA was completed.</span></span> <span data-ttu-id="330c3-175">Agora, quando você listar as detecções de risco, o **riscostate** mostrará o evento como `remediated` .</span><span class="sxs-lookup"><span data-stu-id="330c3-175">Now, when you list risk detections the **riskState** shows the event as `remediated`.</span></span>

#### <a name="request"></a><span data-ttu-id="330c3-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="330c3-176">Request</span></span>

``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskDetections?$filter=userDisplayName eq 'MyTestUser1'
```

#### <a name="response"></a><span data-ttu-id="330c3-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="330c3-177">Response</span></span>

```http
{
  "id": "ba9d45f16d8f87f6ae974efda7336b2120962a398cb362dfd9e5bdc8e9d149d0",
  "requestId": "156c01fb-31cf-4a10-b9a9-beee93e6a400",
  "correlationId": "a8aaac45-fe22-46df-babf-10a8dba85d62",
  "riskType": "anonymizedIPAddress",
  "riskEventType": "anonymizedIPAddress",
  "riskState": "remediated",
  "riskLevel": "medium",
  "riskDetail": "userPassedMFADrivenByRiskBasedPolicy",
  "source": "IdentityProtection",
  "detectionTimingType": "realtime",
  "activity": "signin",
  "tokenIssuerType": "AzureAD",
  "ipAddress": "185.220.101.213",
  "activityDateTime": "2020-11-12T23:45:22.4092789Z",
  "detectedDateTime": "2020-11-12T23:45:22.4092789Z",
  "lastUpdatedDateTime": "2020-11-12T23:47:57.7831423Z",
  "userId": "4b608561-9258-44ba-8cdb-3286dcbf0e3b",
  "userDisplayName": "MyTestUser1",
  "userPrincipalName": "MyTestUser1@contoso.com",
    "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; rv:78.0) Gecko/20100101 Firefox/78.0\"}]",
  "location": {
    "city": "Schoenwalde-Glien",
    "state": "Brandenburg",
    "countryOrRegion": "DE",
    "geoCoordinates": {
      "latitude": 52.61983,
      "longitude": 13.12743
    }
  }
}
```

## <a name="step-4-optional-block-the-user-from-signing-in"></a><span data-ttu-id="330c3-178">Etapa 4 (opcional) bloquear o usuário de entrar</span><span class="sxs-lookup"><span data-stu-id="330c3-178">Step 4 (Optional) Block the user from signing in</span></span>

<span data-ttu-id="330c3-179">Em vez de fornecer a oportunidade para que o usuário seja automaticamente remediado, você pode impedir que o usuário entre.</span><span class="sxs-lookup"><span data-stu-id="330c3-179">Instead of providing the opportunity for the user to self-remediate, you can block the user from signing in.</span></span> <span data-ttu-id="330c3-180">Nesta etapa, você cria uma nova política de acesso condicional que impede o usuário de entrar se ocorrer uma detecção de risco médio ou alto.</span><span class="sxs-lookup"><span data-stu-id="330c3-180">In this step, you create a new conditional access policy that blocks the user from signing in if a medium or high risk detection occurs.</span></span> <span data-ttu-id="330c3-181">A diferença nas políticas é que o **builtInControls** está definido como `block` .</span><span class="sxs-lookup"><span data-stu-id="330c3-181">The difference in policies is that the **builtInControls** is set to `block`.</span></span>

### <a name="request"></a><span data-ttu-id="330c3-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="330c3-182">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies
Content-type: application/json

{
  "displayName": "Policy for risky sign-in block access",
  "state": "enabled",
  "conditions": {
    "signInRiskLevels": [
      "high",
      "medium"
    ],
    "applications": {
      "includeApplications": ["All"]
    },
    "users": {
      "includeUsers": [
        "4628e7df-dff3-407c-a08f-75f08c0806dc"
      ]
    }
  },
  "grantControls": {
    "operator": "OR",
    "builtInControls": [
      "block"
    ]
  }
}
```

### <a name="response"></a><span data-ttu-id="330c3-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="330c3-183">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/conditionalAccess/policies/$entity",
  "id": "9ad78153-b1f8-4714-adc1-1445727678a8",
  "displayName": "Policy for risky sign-in block access",
  "createdDateTime": "2020-11-03T20:56:38.6210843Z",
  "modifiedDateTime": null,
  "state": "enabled",
  "sessionControls": null,
  "conditions": {
    "signInRiskLevels": [
      "high",
      "medium"
    ],
    "clientAppTypes": [ 
      "all" 
    ],
    "platforms": null,
    "locations": null,
    "applications": {
      "includeApplications": [
        "All"
      ],
      "excludeApplications": [],
      "includeUserActions": []
    },
    "users": {
      "includeUsers": [
        "4628e7df-dff3-407c-a08f-75f08c0806dc"
      ],
      "excludeUsers": [],
      "includeGroups": [],
      "excludeGroups": [],
      "includeRoles": [],
      "excludeRoles": []
    }
  },
  "grantControls": {
    "operator": "OR",
    "builtInControls": [
      "block"
    ],
    "customAuthenticationFactors": [],
    "termsOfUse": []
  }
}
```

<span data-ttu-id="330c3-184">Com essa política de acesso condicional in-loco, a conta do **MyTestUser1** agora está impedida de entrar porque o nível de risco de entrada é `medium` ou `high` .</span><span class="sxs-lookup"><span data-stu-id="330c3-184">With this conditional access policy in place, the **MyTestUser1** account is now blocked from signing in because the sign-in risk level is `medium` or `high`.</span></span>

![Entrada bloqueada](./images/tutorial-riskdetection-api/conditionalaccess-policy.png)

## <a name="step-5-dismiss-risky-users"></a><span data-ttu-id="330c3-186">Etapa 5: ignorar usuários arriscados</span><span class="sxs-lookup"><span data-stu-id="330c3-186">Step 5: Dismiss risky users</span></span>

<span data-ttu-id="330c3-187">Se acreditar que o usuário não está em risco e você não deseja impor uma política de acesso condicional, você pode descartar manualmente o usuário arriscado.</span><span class="sxs-lookup"><span data-stu-id="330c3-187">If you believe the user is not at risk, and you don’t want to enforce a conditional access policy, you can manually dismiss the risky user.</span></span>

### <a name="dismiss-the-risky-user"></a><span data-ttu-id="330c3-188">Ignorar o usuário arriscado</span><span class="sxs-lookup"><span data-stu-id="330c3-188">Dismiss the risky user</span></span>

#### <a name="request"></a><span data-ttu-id="330c3-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="330c3-189">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/dismiss
Content-Type: application/json

{
  "userIds": [
    "4628e7df-dff3-407c-a08f-75f08c0806dc"
  ]
}
```

#### <a name="response"></a><span data-ttu-id="330c3-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="330c3-190">Response</span></span>

```http
HTTP/1.1 204 No Content
```        

### <a name="list-risky-users"></a><span data-ttu-id="330c3-191">Listar usuários arriscados</span><span class="sxs-lookup"><span data-stu-id="330c3-191">List risky users</span></span>

<span data-ttu-id="330c3-192">Após descartar o usuário de risco, você poderá ver na resposta ao listar os usuários arriscados que a conta de usuário do **MyTestUser1** agora tem um nível de risco `none` e um risco de `dismissed` .</span><span class="sxs-lookup"><span data-stu-id="330c3-192">After dismissing the risk user, you can see in the response when listing risky users that the **MyTestUser1** user account now has a risk level of `none` and a riskState of `dismissed`.</span></span>

#### <a name="request"></a><span data-ttu-id="330c3-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="330c3-193">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers?$filter=userDisplayName eq 'MyTestUser1'
```

#### <a name="response"></a><span data-ttu-id="330c3-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="330c3-194">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#riskyUsers",
  "value": [
    {
      "id": "4628e7df-dff3-407c-a08f-75f08c0806dc",
      "isDeleted": false,
      "isProcessing": false,
      "riskLevel": "none",
      "riskState": "dismissed",
      "riskDetail": "adminDismissedAllRiskForUser",
      "riskLastUpdatedDateTime": "2020-11-03T21:48:53.4298425Z",
      "userDisplayName": "MyTestUser1",
      "userPrincipalName": "MyTestUser1@contoso.com"
    }
  ]
}
```

## <a name="step-6-clean-up-resources"></a><span data-ttu-id="330c3-195">Etapa 6: limpar recursos</span><span class="sxs-lookup"><span data-stu-id="330c3-195">Step 6: Clean up resources</span></span>

<span data-ttu-id="330c3-196">Nesta etapa, remova os recursos que você criou.</span><span class="sxs-lookup"><span data-stu-id="330c3-196">In this step, you remove the resources that you created.</span></span>

### <a name="delete-the-user-account"></a><span data-ttu-id="330c3-197">Excluir a conta de usuário</span><span class="sxs-lookup"><span data-stu-id="330c3-197">Delete the user account</span></span>

<span data-ttu-id="330c3-198">Exclua a conta de usuário do **MyTestUser1** .</span><span class="sxs-lookup"><span data-stu-id="330c3-198">Delete the **MyTestUser1** user account.</span></span>

#### <a name="request"></a><span data-ttu-id="330c3-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="330c3-199">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/users/4628e7df-dff3-407c-a08f-75f08c0806dc
```

#### <a name="response"></a><span data-ttu-id="330c3-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="330c3-200">Response</span></span>

```http
No Content - 204
```

### <a name="delete-the-conditional-access-policy"></a><span data-ttu-id="330c3-201">Excluir a política de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="330c3-201">Delete the conditional access policy</span></span>

<span data-ttu-id="330c3-202">Exclua a política de acesso condicional que você criou.</span><span class="sxs-lookup"><span data-stu-id="330c3-202">Delete the conditional access policy that you created.</span></span>

#### <a name="request"></a><span data-ttu-id="330c3-203">Solicitação</span><span class="sxs-lookup"><span data-stu-id="330c3-203">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/groups/9ad78153-b1f8-4714-adc1-1445727678a8
```

#### <a name="response"></a><span data-ttu-id="330c3-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="330c3-204">Response</span></span>

```http
No Content - 204
```

## <a name="see-also"></a><span data-ttu-id="330c3-205">Confira também</span><span class="sxs-lookup"><span data-stu-id="330c3-205">See also</span></span>

<span data-ttu-id="330c3-206">Neste tutorial, você usou muitas APIs para realizar tarefas.</span><span class="sxs-lookup"><span data-stu-id="330c3-206">In this tutorial, you used many APIs to accomplish tasks.</span></span> <span data-ttu-id="330c3-207">Explore a referência de API para essas APIs para saber mais sobre o que as APIs podem fazer.</span><span class="sxs-lookup"><span data-stu-id="330c3-207">Explore the API reference for these APIs to learn more about what the APIs can do.</span></span>

- [<span data-ttu-id="330c3-208">O que é proteção de identidade?</span><span class="sxs-lookup"><span data-stu-id="330c3-208">What is Identity Protection?</span></span>](/azure/active-directory/identity-protection/overview-identity-protection)
- [<span data-ttu-id="330c3-209">O que é Acesso Condicional?</span><span class="sxs-lookup"><span data-stu-id="330c3-209">What is Conditional Access?</span></span>](/azure/active-directory/conditional-access/overview)
- [<span data-ttu-id="330c3-210">Como funciona: autenticação multifator do Azure</span><span class="sxs-lookup"><span data-stu-id="330c3-210">How it works: Azure Multi-Factor Authentication</span></span>](/azure/active-directory/authentication/concept-mfa-howitworks)
- [<span data-ttu-id="330c3-211">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="330c3-211">conditionalAccessPolicy</span></span>](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-1.0)
- [<span data-ttu-id="330c3-212">riskDetection</span><span class="sxs-lookup"><span data-stu-id="330c3-212">riskDetection</span></span>](/graph/api/resources/riskdetection?view=graph-rest-1.0)
- [<span data-ttu-id="330c3-213">riskyUser</span><span class="sxs-lookup"><span data-stu-id="330c3-213">riskyUser</span></span>](/graph/api/resources/riskyuser?view=graph-rest-1.0)
- [<span data-ttu-id="330c3-214">user</span><span class="sxs-lookup"><span data-stu-id="330c3-214">user</span></span>](/graph/api/resources/user?view=graph-rest-1.0)