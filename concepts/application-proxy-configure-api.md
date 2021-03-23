---
title: Configurar Proxy de Aplicativo usando APIs do Microsoft Graph
description: Configure o Proxy de Aplicativo usando as APIs do Microsoft Graph para fornecer acesso remoto e um único login a aplicativos locais.
author: davidmu1
ms.topic: conceptual
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: efc22ff03bf5b32398be6711a8f44394bf623050
ms.sourcegitcommit: 74a1fb3874e04c488e1b87dcee80d76cc586c1f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51031076"
---
# <a name="configure-application-proxy-using-the-microsoft-graph-api"></a><span data-ttu-id="50071-103">Configurar o Proxy de Aplicativo usando a API do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="50071-103">Configure Application Proxy using the Microsoft Graph API</span></span>

<span data-ttu-id="50071-104">Neste artigo, você aprenderá a configurar o Proxy de Aplicativo do Azure Active Directory (Azure AD) para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="50071-104">In this article, you'll learn how to configure Azure Active Directory (Azure AD) Application Proxy for an application.</span></span> <span data-ttu-id="50071-105">O Proxy de Aplicativo fornece acesso remoto seguro e um único login em aplicativos Web locais.</span><span class="sxs-lookup"><span data-stu-id="50071-105">Application Proxy provides secure remote access and single sign-on to on-premises web applications.</span></span> <span data-ttu-id="50071-106">Depois de configurar o Proxy de Aplicativo para um aplicativo, os usuários podem acessar seus aplicativos locais por meio de uma URL externa, do portal Meus Aplicativos ou de outros portais de aplicativos internos.</span><span class="sxs-lookup"><span data-stu-id="50071-106">After configuring Application Proxy for an application, users can access their on-premises applications through an external URL, the My Apps portal, or other internal application portals.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50071-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="50071-107">Prerequisites</span></span>

- <span data-ttu-id="50071-108">Este tutorial supõe que você já instalou um conector e concluiu os [pré-requisitos](/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) para o Proxy de Aplicativo para que os conectores possam se comunicar com os serviços do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="50071-108">This tutorial assumes you have already installed a connector and completed the [prerequisites](/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) for Application Proxy so that connectors can communicate with Azure AD services.</span></span>
- <span data-ttu-id="50071-109">Este tutorial assume que você está usando o Microsoft Graph Explorer, mas você pode usar o Postman ou criar seu próprio aplicativo cliente para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="50071-109">This tutorial assumes that you are using Microsoft Graph Explorer, but you can use Postman, or create your own client app to call Microsoft Graph.</span></span> <span data-ttu-id="50071-110">Para chamar as APIs do Microsoft Graph neste tutorial, você precisa usar uma conta com a função de administrador global e as permissões apropriadas.</span><span class="sxs-lookup"><span data-stu-id="50071-110">To call the Microsoft Graph APIs in this tutorial, you need to use an account with the global administrator role and the appropriate permissions.</span></span> <span data-ttu-id="50071-111">Conclua as seguintes etapas para definir as permissões no Microsoft Graph Explorer:</span><span class="sxs-lookup"><span data-stu-id="50071-111">Complete the following steps to set permissions in Microsoft Graph Explorer:</span></span>
    1. <span data-ttu-id="50071-112">Inicie o [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="50071-112">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
    2. <span data-ttu-id="50071-113">Selecione **Entrar com a conta da Microsoft** e entre usando uma conta de administrador global do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="50071-113">Select **Sign-In with Microsoft** and sign in using an Azure AD global administrator account.</span></span> <span data-ttu-id="50071-114">Uma vez acessado, você verá os detalhes da conta do usuário no painel esquerdo.</span><span class="sxs-lookup"><span data-stu-id="50071-114">After you successfully sign in, you can see the user account details in the left-hand pane.</span></span>
    3. <span data-ttu-id="50071-115">Selecione o ícone de configurações à direita dos detalhes da conta do usuário e, em seguida, selecione **Selecionar permissões**.</span><span class="sxs-lookup"><span data-stu-id="50071-115">Select the settings icon to the right of the user account details, and then select **Select permissions**.</span></span>

        ![Definir permissões](./images/application-proxy-configure-api/set-permissions.png)
        
    4. <span data-ttu-id="50071-117">Role a lista de permissões para **Directory (3),** expanda e selecione `Directory.ReadWrite.All` .</span><span class="sxs-lookup"><span data-stu-id="50071-117">Scroll through the list of permissions to **Directory (3)**, expand and then select `Directory.ReadWrite.All`.</span></span>

        ![Pesquisar permissões](./images/application-proxy-configure-api/select-permissions.png)
    
    5. <span data-ttu-id="50071-119">Selecione **Consentimento** e, em seguida, selecione **Aceitar** para aceitar o consentimento das permissões.</span><span class="sxs-lookup"><span data-stu-id="50071-119">Select **Consent**, and then select **Accept** to accept the consent of the permissions.</span></span> <span data-ttu-id="50071-120">Você não precisa consentir em nome da organização para essas permissões.</span><span class="sxs-lookup"><span data-stu-id="50071-120">You do not need to consent on behalf of your organization for these permissions.</span></span>

        ![Aceitar permissões](./images/application-proxy-configure-api/accept-permissions.png)

> [!NOTE]
> <span data-ttu-id="50071-122">Os objetos de resposta mostrados podem ser reduzidos para a capacidade de leitura.</span><span class="sxs-lookup"><span data-stu-id="50071-122">The response objects shown might be shortened for readability.</span></span> 

## <a name="step-1-create-a-custom-application"></a><span data-ttu-id="50071-123">Etapa 1: Criar um aplicativo personalizado</span><span class="sxs-lookup"><span data-stu-id="50071-123">Step 1: Create a custom application</span></span>

<span data-ttu-id="50071-124">Para configurar o Proxy de Aplicativo para um aplicativo usando a API, primeiro crie um aplicativo personalizado e atualize a propriedade **onPremisesPublishing** do aplicativo para configurar as configurações do Proxy de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="50071-124">To configure Application Proxy for an app using the API, you first create a custom application, and then update the application's **onPremisesPublishing** property to configure the App Proxy settings.</span></span> <span data-ttu-id="50071-125">Neste tutorial, você usa um modelo de aplicativo para criar uma instância de um aplicativo personalizado e entidade de serviço em seu locatário para gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="50071-125">In this tutorial, you use an application template to create an instance of a custom application and service principal in your tenant for management.</span></span> <span data-ttu-id="50071-126">A ID do modelo de um aplicativo personalizado é `8adf8e6e-67b2-4cf2-a259-e3dc5476c621` .</span><span class="sxs-lookup"><span data-stu-id="50071-126">The template ID for a custom application is `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span></span>

<span data-ttu-id="50071-127">Grave o **id**, **appId**, **servicePrincipalId** do aplicativo a ser usado posteriormente no tutorial.</span><span class="sxs-lookup"><span data-stu-id="50071-127">Record the **id**, **appId**, **servicePrincipalId** of the application to use later in the tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="50071-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50071-128">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/applicationTemplates/8adf8e6e-67b2-4cf2-a259-e3dc5476c621/instantiate
Content-type: application/json

{
  "displayName": "Contoso IWA App"
}
```

#### <a name="response"></a><span data-ttu-id="50071-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="50071-129">Response</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#applications/$entity",
  "id": "bf21f7e9-9d25-4da2-82ab-7fdd85049f83",
  "deletedDateTime": null,
  "addIns": [],
  "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b",
  "applicationTemplateId": null,
  "identifierUris": [],
  "createdDateTime": "2020-08-11T21:07:47.5919755Z",
  "description": null,
  "displayName": "Contoso IWA App",
  "isAuthorizationServiceEnabled": false,
  "isDeviceOnlyAuthSupported": null,
  "isFallbackPublicClient": null,
  "groupMembershipClaims": null,
  "notes": null,
  "optionalClaims": null,
  "orgRestrictions": [],
  "publisherDomain": "f128.info",
  "signInAudience": "AzureADandPersonalMicrosoftAccount",
  "tags": [],
  "tokenEncryptionKeyId": null,
  "uniqueName": null,
  "verifiedPublisher": {
      "displayName": null,
      "verifiedPublisherId": null,
      "addedDateTime": null
  },
}
```

## <a name="step-2-configure-application-proxy"></a><span data-ttu-id="50071-130">Etapa 2: Configurar o Proxy de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50071-130">Step 2: Configure Application Proxy</span></span>

<span data-ttu-id="50071-131">Use a **id** que você gravou para o aplicativo para iniciar a configuração do Proxy de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="50071-131">Use the **id** that you recorded for the application to start the configuration of Application Proxy.</span></span> <span data-ttu-id="50071-132">Atualize as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="50071-132">Update the following properties:</span></span>

- <span data-ttu-id="50071-133">**onPremisesPublishing** - Neste exemplo, você está usando um aplicativo com a URL interna: `https://contosoiwaapp.com` .</span><span class="sxs-lookup"><span data-stu-id="50071-133">**onPremisesPublishing** - In this example, you're using an app with the internal URL: `https://contosoiwaapp.com`.</span></span> <span data-ttu-id="50071-134">Você também usa o domínio padrão para a URL externa: `https://contosoiwaapp-contoso.msappproxy.net` .</span><span class="sxs-lookup"><span data-stu-id="50071-134">You also use the default domain for the external URL: `https://contosoiwaapp-contoso.msappproxy.net`.</span></span> 
- <span data-ttu-id="50071-135">**redirectUri**, **identifierUri** e **homepageUrl** - Defina como a mesma URL externa configurada na **propriedade onPremisesPublishing.**</span><span class="sxs-lookup"><span data-stu-id="50071-135">**redirectUri**, **identifierUri**, and **homepageUrl** - Set to the same external URL configured in the **onPremisesPublishing** property.</span></span>
- <span data-ttu-id="50071-136">**implicitGrantSettings** - Definir como `true` **para enabledTokenIssuance** e `false` **enabledAccessTokenIssuance**.</span><span class="sxs-lookup"><span data-stu-id="50071-136">**implicitGrantSettings** - Set to `true` for **enabledTokenIssuance** and `false` for **enabledAccessTokenIssuance**.</span></span>

#### <a name="request"></a><span data-ttu-id="50071-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50071-137">Request</span></span>

```http
PATCH https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83
Content-type: application/json

{
  "onPremisesPublishing": {
    "externalAuthenticationType": "aadPreAuthentication",
    "internalUrl": "https://contosoiwaapp.com",
    "externalUrl": "https://contosoiwaapp-contoso.msappproxy.net"
  }
  "identifierUris": ["https://contosoiwaapp-contoso.msappproxy.net"],
  "web": {
    "redirectUris": ["https://contosoiwaapp-contoso.msappproxy.net"],
    "homePageUrl": "https://contosoiwaapp-contoso.msappproxy.net",
    "implicitGrantSettings": {
      "enableIdTokenIssuance": true,
      "enableAccessTokenIssuance": false
    }
  }
}
```

#### <a name="response"></a><span data-ttu-id="50071-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="50071-138">Response</span></span>

```http
HTTP/1.1 204 No content
```

## <a name="step-3-assign-a-connector-group-to-the-application"></a><span data-ttu-id="50071-139">Etapa 3: Atribuir um grupo de conectores ao aplicativo</span><span class="sxs-lookup"><span data-stu-id="50071-139">Step 3: Assign a connector group to the application</span></span>

### <a name="get-connectors"></a><span data-ttu-id="50071-140">Obter conectores</span><span class="sxs-lookup"><span data-stu-id="50071-140">Get connectors</span></span>

<span data-ttu-id="50071-141">Listar os conectores disponíveis.</span><span class="sxs-lookup"><span data-stu-id="50071-141">List the connectors that are available.</span></span> <span data-ttu-id="50071-142">Grave a **id** do conector que você deseja atribuir a um grupo de conectores.</span><span class="sxs-lookup"><span data-stu-id="50071-142">Record the **id** of the connector that you want to assign to a connector group.</span></span>

#### <a name="request"></a><span data-ttu-id="50071-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50071-143">Request</span></span>

```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors
```

#### <a name="response"></a><span data-ttu-id="50071-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="50071-144">Response</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#connectors",
  "value": [
    {
      "id": "d2b1e8e8-8511-49d6-a4ba-323cb083fbb0",
      "machineName": "connectorA.redmond.contoso.com"",
      "externalIp": "131.137.147.164",
      "status": "active"
    },
    {
      "id": "f2cab422-a1c8-4d70-a47e-2cb297a2e051",
      "machineName": "connectorB.contoso.com"",
      "externalIp": "68.0.191.210",
      "status": "active"
    }
  ]
}
```

### <a name="create-a-connectorgroup"></a><span data-ttu-id="50071-145">Criar um connectorGroup</span><span class="sxs-lookup"><span data-stu-id="50071-145">Create a connectorGroup</span></span>

<span data-ttu-id="50071-146">Para este exemplo, um novo connectorGroup é criado chamado `IWA Demo Connector Group` que é usado para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="50071-146">For this example, a new connectorGroup is created named `IWA Demo Connector Group` that is used for the application.</span></span> <span data-ttu-id="50071-147">Grave a **id** retornada para uso na próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="50071-147">Record the **id** that is returned to use in the next step.</span></span>

#### <a name="request"></a><span data-ttu-id="50071-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50071-148">Request</span></span>

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups

Content-type: application/json
{
  "name": "IWA Demo Connector Group"
}
```

#### <a name="response"></a><span data-ttu-id="50071-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="50071-149">Response</span></span>

```http
HTTP/1.1 201
Content-type: connectorGroup/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#connectorGroups/$entity",
  "id": "3e6f4c35-a04b-4d03-b98a-66fff89b72e6",
  "name": "IWA Demo Connector Group",
  "connectorGroupType": "applicationProxy",
  "isDefault": false
}
```

### <a name="assign-a-connector-to-the-connectorgroup"></a><span data-ttu-id="50071-150">Atribuir um conector ao connectorGroup</span><span class="sxs-lookup"><span data-stu-id="50071-150">Assign a connector to the connectorGroup</span></span>

#### <a name="request"></a><span data-ttu-id="50071-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50071-151">Request</span></span>

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/f2cab422-a1c8-4d70-a47e-2cb297a2e051/memberOf/$ref
Content-type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/3e6f4c35-a04b-4d03-b98a-66fff89b72e6"
}
```

#### <a name="response"></a><span data-ttu-id="50071-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="50071-152">Response</span></span>

```http
HTTP/1.1 204 No content
```

### <a name="assign-the-application-to-the-connectorgroup"></a><span data-ttu-id="50071-153">Atribuir o aplicativo ao connectorGroup</span><span class="sxs-lookup"><span data-stu-id="50071-153">Assign the application to the connectorGroup</span></span>

#### <a name="request"></a><span data-ttu-id="50071-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50071-154">Request</span></span>

```http
PUT https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83/connectorGroup/$ref
Content-type: application/json

{
"@odata.id":"https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/3e6f4c35-a04b-4d03-b98a-66fff89b72e6"
}
```

#### <a name="response"></a><span data-ttu-id="50071-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="50071-155">Response</span></span>

```http
HTTP/1.1 204 No content
```

## <a name="step-4-configure-single-sign-on"></a><span data-ttu-id="50071-156">Etapa 4: Configurar o login único</span><span class="sxs-lookup"><span data-stu-id="50071-156">Step 4: Configure single sign-on</span></span>

<span data-ttu-id="50071-157">Esse aplicativo usa a Autenticação Integrada do Windows (IWA).</span><span class="sxs-lookup"><span data-stu-id="50071-157">This application uses Integrated Windows Authentication (IWA).</span></span> <span data-ttu-id="50071-158">Para configurar o IWA, de definir as propriedades de login único para **onPremisesPublishing**.</span><span class="sxs-lookup"><span data-stu-id="50071-158">To configure IWA, set the single sign-on properties for **onPremisesPublishing**.</span></span>

#### <a name="request"></a><span data-ttu-id="50071-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50071-159">Request</span></span>

```http
PATCH https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83
Content-type: appplication/json

{
  "onPremisesPublishing": {
    "singleSignOnSettings": {
      "kerberosSignOnSettings": {
        "kerberosServicePrincipalName": "HTTP/iwademo.contoso.com",
        "kerberosSignOnMappingAttributeType": "userPrincipalName"
      },
      "singleSignOnMode": "onPremisesKerberos"
    }
  } 
}
```

#### <a name="response"></a><span data-ttu-id="50071-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="50071-160">Response</span></span>

```http
HTTP/1.1 204 No content
```

## <a name="step-5-assign-a-user"></a><span data-ttu-id="50071-161">Etapa 5: Atribuir um usuário</span><span class="sxs-lookup"><span data-stu-id="50071-161">Step 5: Assign a user</span></span>

### <a name="retrieve-the-approle-for-the-application"></a><span data-ttu-id="50071-162">Recuperar o appRole para o aplicativo</span><span class="sxs-lookup"><span data-stu-id="50071-162">Retrieve the appRole for the application</span></span>

<span data-ttu-id="50071-163">Obter as funções do aplicativo usando a **id** da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="50071-163">Get the app roles for the application using the **id** of the service principal.</span></span> <span data-ttu-id="50071-164">Grave a **id** da **função de** aplicativo usuário a ser usada na próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="50071-164">Record the **id** of the **User** app role to be used in the next step.</span></span>

#### <a name="request"></a><span data-ttu-id="50071-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50071-165">Request</span></span>

```http
GET https://graph.microsoft.com/beta/servicePrincipals/a8cac399-cde5-4516-a674-819503c61313/appRoles
```

#### <a name="response"></a><span data-ttu-id="50071-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="50071-166">Response</span></span>

```http
HTTP/1.1 200
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals('a8cac399-cde5-4516-a674-819503c61313')/appRoles",
  "value": [
    {
      "allowedMemberTypes": [
        "User"
      ],
      "description": "User",
      "displayName": "User",
      "id": "18d14569-c3bd-439b-9a66-3a2aee01d14f",
      "isEnabled": true,
      "origin": "Application",
      "value": null
    },
  ]
}
```

### <a name="create-a-user-account"></a><span data-ttu-id="50071-167">Criar uma conta de usuário</span><span class="sxs-lookup"><span data-stu-id="50071-167">Create a user account</span></span>

<span data-ttu-id="50071-168">Para este tutorial, você cria uma conta de usuário atribuída à função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="50071-168">For this tutorial, you create a user account that is assigned to the app role.</span></span> <span data-ttu-id="50071-169">No corpo da solicitação, `contoso.com` altere para o nome de domínio do locatário.</span><span class="sxs-lookup"><span data-stu-id="50071-169">In the request body, change `contoso.com` to the domain name of your tenant.</span></span> <span data-ttu-id="50071-170">Encontre informações sobre locatários na página de visão geral do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="50071-170">You can find tenant information on the Azure Active Directory overview page.</span></span> <span data-ttu-id="50071-171">Grave a **id** da conta de usuário a ser usada na próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="50071-171">Record the **id** of the user account to be used in the next step.</span></span>

#### <a name="request"></a><span data-ttu-id="50071-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50071-172">Request</span></span>

```http
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

#### <a name="response"></a><span data-ttu-id="50071-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="50071-173">Response</span></span>

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

### <a name="assign-the-user-to-the-application"></a><span data-ttu-id="50071-174">Atribuir o usuário ao aplicativo</span><span class="sxs-lookup"><span data-stu-id="50071-174">Assign the user to the application</span></span>

<span data-ttu-id="50071-175">No exemplo a seguir, substitua os valores dessas propriedades:</span><span class="sxs-lookup"><span data-stu-id="50071-175">In the following example, replace the values of these properties:</span></span>

- <span data-ttu-id="50071-176">**principalId** com **a id** do usuário</span><span class="sxs-lookup"><span data-stu-id="50071-176">**principalId** with the **id** of the user</span></span>
- <span data-ttu-id="50071-177">**appRoleId** com **a id** da função de aplicativo</span><span class="sxs-lookup"><span data-stu-id="50071-177">**appRoleId** with the **id** of the app role</span></span>
- <span data-ttu-id="50071-178">**resourceId** com **a id** da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="50071-178">**resourceId** with the **id** of the service principal</span></span>

#### <a name="request"></a><span data-ttu-id="50071-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50071-179">Request</span></span>

```http
POST https://graph.microsoft.com/beta/servicePrincipals/b00c693f-9658-4c06-bd1b-c402c4653dea/appRoleAssignments
Content-type: appRoleAssignments/json

{
  "principalId": "4628e7df-dff3-407c-a08f-75f08c0806dc",
  "principalType": "User",
  "appRoleId":"18d14569-c3bd-439b-9a66-3a2aee01d14f",
  "resourceId":"a8cac399-cde5-4516-a674-819503c61313"
}
```

#### <a name="response"></a><span data-ttu-id="50071-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="50071-180">Response</span></span>

```http
HTTP/1.1 200
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#appRoleAssignments/$entity",
  "id": "I23pL8ZdNU-CIgQmqMEVyLJ0E6fx0ixEo92az8MnhtU",
  "creationTimestamp": "2020-06-09T00:06:07.5129268Z",
  "appRoleId": "18d14569-c3bd-439b-9a66-3a2aee01d14f",
  "principalDisplayName": "MyTestUser1",
  "principalId": "2fe96d23-5dc6-4f35-8222-0426a8c115c8",
  "principalType": "User",
  "resourceDisplayName": "Contoso IWA App",
  "resourceId": "a8cac399-cde5-4516-a674-819503c61313"
}
```
## <a name="step-6-test-access-to-the-application"></a><span data-ttu-id="50071-181">Etapa 6: Testar o acesso ao aplicativo</span><span class="sxs-lookup"><span data-stu-id="50071-181">Step 6: Test access to the application</span></span>

<span data-ttu-id="50071-182">Teste o aplicativo visitando a **URL externa** configurada para o aplicativo em seu navegador e, em seguida, entre com seu usuário de teste.</span><span class="sxs-lookup"><span data-stu-id="50071-182">Test the application by visiting the **External URL** configured for the app on your browser and then sign in with your test user.</span></span> <span data-ttu-id="50071-183">Você deve poder fazer logoff no aplicativo e acessar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="50071-183">You should be able to log into the app and access the application.</span></span>

## <a name="step-7-clean-up-resources"></a><span data-ttu-id="50071-184">Etapa 7: Limpar recursos</span><span class="sxs-lookup"><span data-stu-id="50071-184">Step 7: Clean up resources</span></span>

<span data-ttu-id="50071-185">Os recursos criados neste tutorial não se destinam a ser usados em um ambiente de produção.</span><span class="sxs-lookup"><span data-stu-id="50071-185">The resources that you created in this tutorial are not intended to be used in a production environment.</span></span> <span data-ttu-id="50071-186">Nessa etapa, remova os recursos que criou.</span><span class="sxs-lookup"><span data-stu-id="50071-186">In this step, you remove the resources that you created.</span></span>

### <a name="delete-the-user-account"></a><span data-ttu-id="50071-187">Excluir a conta de usuário</span><span class="sxs-lookup"><span data-stu-id="50071-187">Delete the user account</span></span>

<span data-ttu-id="50071-188">Exclua a conta de usuário MyTestUser1.</span><span class="sxs-lookup"><span data-stu-id="50071-188">Delete the MyTestUser1 user account.</span></span>

#### <a name="request"></a><span data-ttu-id="50071-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50071-189">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/users/4628e7df-dff3-407c-a08f-75f08c0806dc
```

#### <a name="response"></a><span data-ttu-id="50071-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="50071-190">Response</span></span>

```http
No Content - 204
```

### <a name="delete-the-application"></a><span data-ttu-id="50071-191">Excluir o aplicativo</span><span class="sxs-lookup"><span data-stu-id="50071-191">Delete the application</span></span>

#### <a name="request"></a><span data-ttu-id="50071-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50071-192">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83
```

#### <a name="response"></a><span data-ttu-id="50071-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="50071-193">Response</span></span>

```http
No Content - 204
```

### <a name="delete-the-connector-group"></a><span data-ttu-id="50071-194">Excluir o grupo de conectores</span><span class="sxs-lookup"><span data-stu-id="50071-194">Delete the connector group</span></span>

#### <a name="request"></a><span data-ttu-id="50071-195">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50071-195">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/3e6f4c35-a04b-4d03-b98a-66fff89b72e6
```

#### <a name="response"></a><span data-ttu-id="50071-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="50071-196">Response</span></span>

```http
No Content - 204
```

## <a name="see-also"></a><span data-ttu-id="50071-197">Confira também</span><span class="sxs-lookup"><span data-stu-id="50071-197">See also</span></span>

- [<span data-ttu-id="50071-198">Proxy de aplicativo</span><span class="sxs-lookup"><span data-stu-id="50071-198">Application Proxy</span></span>](/azure/active-directory/manage-apps/what-is-application-proxy)
- [<span data-ttu-id="50071-199">aplicativo</span><span class="sxs-lookup"><span data-stu-id="50071-199">application</span></span>](/graph/api/resources/application?view=graph-rest-1.0)
- [<span data-ttu-id="50071-200">applicationTemplate: instaurá-lo</span><span class="sxs-lookup"><span data-stu-id="50071-200">applicationTemplate: instantiate</span></span>](/graph/api/applicationtemplate-instantiate?view=graph-rest-1.0)
- [<span data-ttu-id="50071-201">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="50071-201">appRoleAssignment</span></span>](/graph/api/resources/approleassignment?view=graph-rest-beta)
- [<span data-ttu-id="50071-202">connector</span><span class="sxs-lookup"><span data-stu-id="50071-202">connector</span></span>](/graph/api/resources/connector?view=graph-rest-beta)
- [<span data-ttu-id="50071-203">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="50071-203">connectorGroup</span></span>](/graph/api/resources/connectorGroup?view=graph-rest-beta)
- [<span data-ttu-id="50071-204">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="50071-204">implicitGrantSettings</span></span>](/graph/api/resources/implicitgrantsettings?view=graph-rest-1.0)
- [<span data-ttu-id="50071-205">perfis de publicação local</span><span class="sxs-lookup"><span data-stu-id="50071-205">on-premises publishing profiles</span></span>](/graph/api/resources/onpremisespublishingprofile-root?view=graph-rest-beta)
- [<span data-ttu-id="50071-206">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="50071-206">servicePrincipal</span></span>](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)
- [<span data-ttu-id="50071-207">singleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="50071-207">singleSignOnSettings</span></span>](/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta)
- [<span data-ttu-id="50071-208">user</span><span class="sxs-lookup"><span data-stu-id="50071-208">user</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
