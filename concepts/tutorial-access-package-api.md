---
title: 'Tutorial: Gerenciar o acesso a recursos no gerenciamento de direitos do Active Directory usando as APIs do Microsoft Graph'
description: Saiba como gerenciar o acesso a recursos no gerenciamento de direitos do Active Directory (Azure AD) usando as APIs do Microsoft Graph.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ae9dfec7ae5db453ff6962ffd5684dd3bd9ee7d1
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50271859"
---
# <a name="tutorial-manage-access-to-resources-in-active-directory-entitlement-management-using-microsoft-graph-apis"></a><span data-ttu-id="96a9e-103">Tutorial: Gerenciar o acesso a recursos no gerenciamento de direitos do Active Directory usando as APIs do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="96a9e-103">Tutorial: Manage access to resources in Active Directory entitlement management using Microsoft Graph APIs</span></span>

<span data-ttu-id="96a9e-104">Gerenciar o acesso a todos os recursos de que os funcionários precisam, como grupos, aplicativos e sites, é uma função importante para as organizações.</span><span class="sxs-lookup"><span data-stu-id="96a9e-104">Managing access to all the resources that employees need, such as groups, applications, and sites, is an important function for organizations.</span></span> <span data-ttu-id="96a9e-105">Você deseja conceder aos funcionários o nível certo de acesso que eles precisam para serem produtivos e remover o acesso quando não for mais necessário.</span><span class="sxs-lookup"><span data-stu-id="96a9e-105">You want to grant employees the right level of access they need to be productive and remove their access when it is no longer needed.</span></span> <span data-ttu-id="96a9e-106">O gerenciamento de direitos do [Azure Active Directory (Azure AD)](/azure/active-directory/governance/entitlement-management-overview) usando AS APIs do Microsoft Graph permite gerenciar esse tipo de acesso.</span><span class="sxs-lookup"><span data-stu-id="96a9e-106">[Azure Active Directory (Azure AD) entitlement management](/azure/active-directory/governance/entitlement-management-overview) using Microsoft Graph APIs enables you to manage this type of access.</span></span>

<span data-ttu-id="96a9e-107">Neste tutorial, você foi solicitado a desenvolver código para criar um pacote de recursos para uma campanha de marketing que os usuários internos podem solicitar por autoatendigo.</span><span class="sxs-lookup"><span data-stu-id="96a9e-107">In this tutorial, you've been asked to develop code to create a package of resources for a marketing campaign that internal users can self-service request.</span></span> <span data-ttu-id="96a9e-108">As solicitações não exigem aprovação e o acesso do usuário expira após 30 dias.</span><span class="sxs-lookup"><span data-stu-id="96a9e-108">Requests do not require approval and user's access expires after 30 days.</span></span> <span data-ttu-id="96a9e-109">Para este tutorial, os recursos da campanha de marketing são apenas membros de um único grupo, mas pode ser um conjunto de grupos, aplicativos ou sites do SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="96a9e-109">For this tutorial, the marketing campaign resources are just membership in a single group, but it could be a collection of groups, applications, or SharePoint Online sites.</span></span>

><span data-ttu-id="96a9e-110">**Observação:** Os objetos de resposta mostrados neste tutorial podem ser reduzidos para maior leitura.</span><span class="sxs-lookup"><span data-stu-id="96a9e-110">**Note:** The response objects shown in this tutorial might be shortened for readability.</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="96a9e-111">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="96a9e-111">Prerequisites</span></span>

<span data-ttu-id="96a9e-112">Para concluir com êxito este tutorial, certifique-se de que você tem os pré-requisitos necessários:</span><span class="sxs-lookup"><span data-stu-id="96a9e-112">To successfully complete this tutorial, make sure that you have the required prerequisites:</span></span>
- <span data-ttu-id="96a9e-113">O gerenciamento de direitos do Azure AD requer licenças específicas.</span><span class="sxs-lookup"><span data-stu-id="96a9e-113">Azure AD entitlement management requires specific licenses.</span></span> <span data-ttu-id="96a9e-114">Para obter mais informações, consulte [Requisitos de licença.](/azure/active-directory/governance/entitlement-management-overview#license-requirements)</span><span class="sxs-lookup"><span data-stu-id="96a9e-114">For more information, see [License requirements](/azure/active-directory/governance/entitlement-management-overview#license-requirements).</span></span> <span data-ttu-id="96a9e-115">As seguintes licenças são necessárias em seu locatário:</span><span class="sxs-lookup"><span data-stu-id="96a9e-115">The following licenses are required in your tenant:</span></span>
    - <span data-ttu-id="96a9e-116">Azure AD Premium P2</span><span class="sxs-lookup"><span data-stu-id="96a9e-116">Azure AD Premium P2</span></span>
    - <span data-ttu-id="96a9e-117">Licença enterprise Mobility + Security (EMS) E5</span><span class="sxs-lookup"><span data-stu-id="96a9e-117">Enterprise Mobility + Security (EMS) E5 license</span></span>
- <span data-ttu-id="96a9e-118">Este tutorial assume que você está usando o Microsoft Graph Explorer, mas você pode usar o Postman ou criar seu próprio aplicativo cliente para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="96a9e-118">This tutorial assumes that you are using Microsoft Graph Explorer, but you can use Postman, or create your own client app to call Microsoft Graph.</span></span> <span data-ttu-id="96a9e-119">Para chamar as APIs do Microsoft Graph neste tutorial, você precisa usar uma conta com a função de administrador global e as permissões apropriadas.</span><span class="sxs-lookup"><span data-stu-id="96a9e-119">To call the Microsoft Graph APIs in this tutorial, you need to use an account with the global administrator role and the appropriate permissions.</span></span> <span data-ttu-id="96a9e-120">Para este tutorial, as permissões , e `User.ReadWrite.All` `Group.ReadWrite.All` `EntitlementManagement.ReadWrite.All` delegadas são necessárias.</span><span class="sxs-lookup"><span data-stu-id="96a9e-120">For this tutorial, the `User.ReadWrite.All`, `Group.ReadWrite.All`, and `EntitlementManagement.ReadWrite.All` delegated permissions are needed.</span></span> <span data-ttu-id="96a9e-121">Conclua as seguintes etapas para definir permissões no Microsoft Graph Explorer:</span><span class="sxs-lookup"><span data-stu-id="96a9e-121">Complete the following steps to set permissions in Microsoft Graph Explorer:</span></span>
    1. <span data-ttu-id="96a9e-122">Iniciar [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="96a9e-122">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
    2. <span data-ttu-id="96a9e-123">Selecione **Entrar com a Microsoft** e entre usando uma conta de administrador global do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="96a9e-123">Select **Sign-In with Microsoft** and sign in using an Azure AD global administrator account.</span></span> <span data-ttu-id="96a9e-124">Depois de entrar com êxito, você poderá ver os detalhes da conta de usuário no painel esquerdo.</span><span class="sxs-lookup"><span data-stu-id="96a9e-124">After you successfully sign in, you can see the user account details in the left-hand pane.</span></span>
    3. <span data-ttu-id="96a9e-125">Selecione o ícone de configurações à direita dos detalhes da conta do usuário e selecione **Selecionar permissões.**</span><span class="sxs-lookup"><span data-stu-id="96a9e-125">Select the settings icon to the right of the user account details, and then select **Select permissions**.</span></span>

        ![Selecionar as permissões do Microsoft Graph](./images/tutorial-access-package-api/set-permissions.png)
        
    4. <span data-ttu-id="96a9e-127">Role pela lista de permissões para as `Group` permissões, expanda **Grupo (2),** selecione a **permissão Group.ReadWrite.All.**</span><span class="sxs-lookup"><span data-stu-id="96a9e-127">Scroll through the list of permissions to the `Group` permissions, expand **Group (2)**, select the **Group.ReadWrite.All** permission.</span></span> <span data-ttu-id="96a9e-128">Role mais para baixo a lista de permissões para as `User` permissões, expanda **Usuário (8)** e selecione a **permissão User.ReadWrite.All.**</span><span class="sxs-lookup"><span data-stu-id="96a9e-128">Scroll further down the list of permissions to the `User` permissions, expand **User (8)**, and select the **User.ReadWrite.All** permission.</span></span>

        ![Pesquisar as permissões de usuário, grupo e direito](./images/tutorial-access-package-api/set-user-permission.png)
    
    5. <span data-ttu-id="96a9e-130">Selecione **Consentimento** e, em **seguida, selecione Aceitar** para aceitar o consentimento das permissões.</span><span class="sxs-lookup"><span data-stu-id="96a9e-130">Select **Consent**, and then select **Accept** to accept the consent of the permissions.</span></span> <span data-ttu-id="96a9e-131">Você não precisa consentir em nome de sua organização para essas permissões.</span><span class="sxs-lookup"><span data-stu-id="96a9e-131">You do not need to consent on behalf of your organization for these permissions.</span></span>
    6. <span data-ttu-id="96a9e-132">Pesquise as `EntitlementManagement` permissões, expanda **EntitlementManagement (2)**, selecione a permissão **Entitlement.ReadWrite.All** e selecione **Consent**.</span><span class="sxs-lookup"><span data-stu-id="96a9e-132">Search for the `EntitlementManagement` permissions, expand **EntitlementManagement (2)**, select the **Entitlement.ReadWrite.All** permission, and then select **Consent**.</span></span> <span data-ttu-id="96a9e-133">Como essa permissão requer consentimento do administrador e é necessária por uma conta de usuário que você cria neste tutorial, você deve selecionar Consentimento **em nome da sua organização.**</span><span class="sxs-lookup"><span data-stu-id="96a9e-133">Because this permission requires admin consent and is needed by a user account that you create in this tutorial, you must select **Consent on behalf of your organization**.</span></span>

        ![Consentimento para a organização](./images/tutorial-access-package-api/consent-for-organization.png)

    7. <span data-ttu-id="96a9e-135">Selecione **Aceitar** para aceitar o consentimento das permissões.</span><span class="sxs-lookup"><span data-stu-id="96a9e-135">Select **Accept** to accept the consent of the permissions.</span></span>

## <a name="step-1-create-a-user-account-and-a-group"></a><span data-ttu-id="96a9e-136">Etapa 1: Criar uma conta de usuário e um grupo</span><span class="sxs-lookup"><span data-stu-id="96a9e-136">Step 1: Create a user account and a group</span></span>

<span data-ttu-id="96a9e-137">Nesta etapa, você cria um grupo chamado Recursos de **Marketing** no diretório que é o recurso de destino para o gerenciamento de direitos.</span><span class="sxs-lookup"><span data-stu-id="96a9e-137">In this step, you create a group named **Marketing resources** in the directory that is the target resource for entitlement management.</span></span> <span data-ttu-id="96a9e-138">Você também cria uma conta de usuário que está configurada como um solicitante interno.</span><span class="sxs-lookup"><span data-stu-id="96a9e-138">You also create a user account that is set up as an internal requestor.</span></span>

### <a name="create-a-user-account"></a><span data-ttu-id="96a9e-139">Criar uma conta de usuário</span><span class="sxs-lookup"><span data-stu-id="96a9e-139">Create a user account</span></span>

<span data-ttu-id="96a9e-140">Para este tutorial, você cria uma conta de usuário que é usada para solicitar acesso aos recursos no pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="96a9e-140">For this tutorial, you create a user account that is used to request access to the resources in the access package.</span></span> <span data-ttu-id="96a9e-141">Ao fazer essas chamadas, mude para `contoso.onmicrosoft.com` o nome de domínio do seu locatário.</span><span class="sxs-lookup"><span data-stu-id="96a9e-141">When you make these calls, change `contoso.onmicrosoft.com` to the domain name of your tenant.</span></span> <span data-ttu-id="96a9e-142">Você pode encontrar informações de locatário na página de visão geral do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="96a9e-142">You can find tenant information on the Azure Active Directory overview page.</span></span> <span data-ttu-id="96a9e-143">Grave o valor da **propriedade de id** que será usada posteriormente no tutorial.</span><span class="sxs-lookup"><span data-stu-id="96a9e-143">Record the value of the **id** property that is returned to be used later in the tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="96a9e-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96a9e-144">Request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "accountEnabled":true,
  "displayName":"Requestor1",
  "mailNickname":"Requestor1",
  "userPrincipalName":"Requestor1@contoso.onmicrosoft.com",
  "passwordProfile": {
    "forceChangePasswordNextSignIn":true,
    "password":"Contoso1234"
  }
}
```

#### <a name="response"></a><span data-ttu-id="96a9e-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="96a9e-145">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
  "id": "007d1c7e-7fa8-4e33-b678-5e437acdcddc",
  "deletedDateTime": null,
  "accountEnabled": true,
  "ageGroup": null,
  "businessPhones": [],
  "city": null,
  "createdDateTime": null,
  "creationType": null,
  "companyName": null,
  "consentProvidedForMinor": null,
  "country": null,
  "department": null,
  "displayName": "Requestor1",
  "employeeId": null,
  "faxNumber": null,
  "givenName": null,
  "imAddresses": [],
  "infoCatalogs": [],
  "isResourceAccount": null,
  "jobTitle": null,
  "legalAgeGroupClassification": null,
  "mail": null,
  "mailNickname": "Requestor1",
}
```

### <a name="create-a-group"></a><span data-ttu-id="96a9e-146">Criar um grupo</span><span class="sxs-lookup"><span data-stu-id="96a9e-146">Create a group</span></span>

<span data-ttu-id="96a9e-147">Neste tutorial, você cria um grupo chamado Recursos de **Marketing** que é o recurso de destino para o gerenciamento de direitos.</span><span class="sxs-lookup"><span data-stu-id="96a9e-147">In this tutorial, you create a group named **Marketing resources** that is the target resource for entitlement management.</span></span> <span data-ttu-id="96a9e-148">Você pode usar um grupo existente se já tiver um.</span><span class="sxs-lookup"><span data-stu-id="96a9e-148">You can use an existing group if you already have one.</span></span> <span data-ttu-id="96a9e-149">Grave o valor da **propriedade de ID** que será retornada para uso posteriormente neste tutorial.</span><span class="sxs-lookup"><span data-stu-id="96a9e-149">Record the value of the **id** property that is returned to use later in this tutorial.</span></span> 

#### <a name="request"></a><span data-ttu-id="96a9e-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96a9e-150">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json

{
  "description":"Marketing group",
  "displayName":"Marketing resources",
  "mailEnabled":false,
  "mailNickname":"markres",
  "securityEnabled":true
}
```

#### <a name="response"></a><span data-ttu-id="96a9e-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="96a9e-151">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
  "id": "e93e24d1-2b65-4a6c-a1dd-654a12225487",
  "deletedDateTime": null,
  "classification": null,
  "createdDateTime": "2020-06-24T16:47:37Z",
  "createdByAppId": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
  "description": "Marketing group",
  "displayName": "Marketing resources",
  "expirationDateTime": null,
  "groupTypes": [],
  "infoCatalogs": [],
  "isAssignableToRole": null,
  "mail": null,
  "mailEnabled": false,
  "mailNickname": "markres"
}
```

## <a name="step-2-add-resources-to-a-catalog-and-create-an-access-package"></a><span data-ttu-id="96a9e-152">Etapa 2: Adicionar recursos a um catálogo e criar um pacote de acesso</span><span class="sxs-lookup"><span data-stu-id="96a9e-152">Step 2: Add resources to a catalog and create an access package</span></span>

<span data-ttu-id="96a9e-153">Um *pacote de acesso* é um pacote de recursos que uma equipe ou projeto precisa e é governado por políticas.</span><span class="sxs-lookup"><span data-stu-id="96a9e-153">An *access package* is a bundle of resources that a team or project needs and is governed with policies.</span></span> <span data-ttu-id="96a9e-154">Os pacotes de acesso são definidos em contêineres chamados catálogos.</span><span class="sxs-lookup"><span data-stu-id="96a9e-154">Access packages are defined in containers called catalogs.</span></span> <span data-ttu-id="96a9e-155">Os catálogos podem fazer referência a recursos, como grupos, aplicativos e sites, que são usados no pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="96a9e-155">Catalogs can reference resources, such as groups, apps and sites, that are used in the access package.</span></span> <span data-ttu-id="96a9e-156">Nesta etapa, você cria um pacote **de acesso** à Campanha de Marketing no catálogo Geral.</span><span class="sxs-lookup"><span data-stu-id="96a9e-156">In this step, you create a **Marketing Campaign** access package in the General catalog.</span></span> <span data-ttu-id="96a9e-157">Se você tiver um catálogo diferente, use seu nome na próxima seção.</span><span class="sxs-lookup"><span data-stu-id="96a9e-157">If you have a different catalog, use its name in the next section.</span></span>

### <a name="get-the-catalog-identifier"></a><span data-ttu-id="96a9e-158">Obter o identificador de catálogo</span><span class="sxs-lookup"><span data-stu-id="96a9e-158">Get the catalog identifier</span></span>

<span data-ttu-id="96a9e-159">Para adicionar recursos ao catálogo, primeiro você deve obter o identificador dele.</span><span class="sxs-lookup"><span data-stu-id="96a9e-159">To add resources to the catalog, you must first get the identifier of it.</span></span> <span data-ttu-id="96a9e-160">Se você estiver usando o catálogo Geral, execute a solicitação a seguir para obter seu identificador.</span><span class="sxs-lookup"><span data-stu-id="96a9e-160">If you are using the General catalog, run the following request to get its identifier.</span></span> <span data-ttu-id="96a9e-161">Se você estiver usando umlog diferente, altere o valor do filtro na solicitação para o nome do seu catálogo.</span><span class="sxs-lookup"><span data-stu-id="96a9e-161">If you are using a different calalog, change the filter value in the request to the name of your catalog.</span></span> <span data-ttu-id="96a9e-162">Grave o valor da **propriedade de id** que será retornada para uso posteriormente neste tutorial.</span><span class="sxs-lookup"><span data-stu-id="96a9e-162">Record the value of the **id** property that is returned to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="96a9e-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96a9e-163">Request</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs?$filter=(displayName eq 'General')
```

#### <a name="response"></a><span data-ttu-id="96a9e-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="96a9e-164">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageCatalogs",
  "value": [ 
    {
      "id": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
      "displayName": "General",
      "description": "Built-in catalog.",
      "catalogType": "ServiceDefault",
      "catalogStatus": "Published",
      "isExternallyVisible": true,
      "createdBy": "Azure AD",
      "createdDateTime": "2020-05-30T10:58:05.363Z",
      "modifiedBy": "Azure AD",
      "modifiedDateTime": "2020-05-30T10:58:05.363Z"
    }
  ]
}
```

<span data-ttu-id="96a9e-165">A resposta deve conter apenas o catálogo cujo nome você forneceu na solicitação.</span><span class="sxs-lookup"><span data-stu-id="96a9e-165">The response should only contain the catalog whose name you provided in the request.</span></span> <span data-ttu-id="96a9e-166">Se não houver valores retornados, verifique se o nome do catálogo está correto antes de prosseguir.</span><span class="sxs-lookup"><span data-stu-id="96a9e-166">If there are no values returned, check that the name of the catalog is correct before you proceed.</span></span>

### <a name="add-the-group-to-the-catalog"></a><span data-ttu-id="96a9e-167">Adicionar o grupo ao catálogo</span><span class="sxs-lookup"><span data-stu-id="96a9e-167">Add the group to the catalog</span></span>

<span data-ttu-id="96a9e-168">Para adicionar o grupo que você criou ao catálogo, forneça os seguintes valores de propriedade:</span><span class="sxs-lookup"><span data-stu-id="96a9e-168">To add the group that you created to the catalog, provide the following property values:</span></span>
- <span data-ttu-id="96a9e-169">**catalogId** - **a id** do catálogo que você está usando</span><span class="sxs-lookup"><span data-stu-id="96a9e-169">**catalogId** - the **id** of the catalog that you are using</span></span>
- <span data-ttu-id="96a9e-170">**displayName** - o nome do grupo</span><span class="sxs-lookup"><span data-stu-id="96a9e-170">**displayName** - the name of the group</span></span>
- <span data-ttu-id="96a9e-171">**description** - a descrição do grupo</span><span class="sxs-lookup"><span data-stu-id="96a9e-171">**description** - the description of the group</span></span>
- <span data-ttu-id="96a9e-172">**originId** - **a id** do grupo que você criou</span><span class="sxs-lookup"><span data-stu-id="96a9e-172">**originId** - the **id** of the group that you created</span></span>

#### <a name="request"></a><span data-ttu-id="96a9e-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96a9e-173">Request</span></span>

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
Content-type: application/json

{
  "catalogId":"cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
  "requestType": "AdminAdd",
  "justification": "",
  "accessPackageResource": {
    "displayName": "Marketing resources",
    "description": "Marketing group",
    "resourceType": "AadGroup",
    "originId": "e93e24d1-2b65-4a6c-a1dd-654a12225487",
    "originSystem": "AadGroup"
  }
}
```

#### <a name="response"></a><span data-ttu-id="96a9e-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="96a9e-174">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageResourceRequests/$entity",
  "catalogId": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
  "executeImmediately": false,
  "id": "44e521e0-fb6b-4d5e-a282-e7e68dc59493",
  "requestType": "AdminAdd",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled",
  "isValidationOnly": false,
  "expirationDateTime": null,
  "justification": ""
}
```

### <a name="get-catalog-resources"></a><span data-ttu-id="96a9e-175">Obter recursos de catálogo</span><span class="sxs-lookup"><span data-stu-id="96a9e-175">Get catalog resources</span></span>

<span data-ttu-id="96a9e-176">Nas etapas posteriores deste tutorial, você precisará da **id** que foi atribuída ao recurso de grupo no catálogo.</span><span class="sxs-lookup"><span data-stu-id="96a9e-176">In later steps in this tutorial, you need the **id** that was assigned to the group resource in the catalog.</span></span> <span data-ttu-id="96a9e-177">Esse identificador, que representa o grupo como um recurso no catálogo, é diferente do identificador do próprio grupo no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="96a9e-177">This identifier, which represents the group as a resource in the catalog, is different than the identifier of the group itself in Microsoft Graph.</span></span> <span data-ttu-id="96a9e-178">Isso porque um catálogo pode ter recursos que não são representados no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="96a9e-178">This is because a catalog can have resources which aren't represented in Microsoft Graph.</span></span>

<span data-ttu-id="96a9e-179">Na solicitação, forneça **a id** do catálogo que você está usando.</span><span class="sxs-lookup"><span data-stu-id="96a9e-179">In the request, provide the **id** of the catalog that you are using.</span></span> <span data-ttu-id="96a9e-180">Registrar o valor da propriedade **de ID** para o recurso de catálogo de grupo.</span><span class="sxs-lookup"><span data-stu-id="96a9e-180">Record the value of the **id** property for the group catalog resource.</span></span>

#### <a name="request"></a><span data-ttu-id="96a9e-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96a9e-181">Request</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/cec5d6ab-c75d-47c0-9c1c-92e89f66e384/accessPackageResources?$filter=(displayName eq 'Marketing resources')
```

#### <a name="response"></a><span data-ttu-id="96a9e-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="96a9e-182">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageResources",
  "value": [
    {
      "id": "4a1e21c5-8a76-4578-acb1-641160e076e8",
      "displayName": "Marketing resources",
      "description": "Marketing group",
      "url": "https://account.activedirectory.windowsazure.com/r?tenantId=d3030981-8fb9-4919-9980-5580caeddd75#/manageMembership?objectType=Group&objectId=e93e24d1-2b65-4a6c-a1dd-654a12225487",
      "resourceType": "Security Group",
      "originId": "e93e24d1-2b65-4a6c-a1dd-654a12225487",
      "originSystem": "AadGroup",
      "isPendingOnboarding": false,
      "addedBy": "admin@contoso.onmicrosoft.com",
      "addedOn": "2020-08-21T19:27:29.967Z"
    }
  ]
}
```

### <a name="get-resources-roles"></a><span data-ttu-id="96a9e-183">Obter funções de recursos</span><span class="sxs-lookup"><span data-stu-id="96a9e-183">Get resources roles</span></span>

<span data-ttu-id="96a9e-184">O pacote de acesso atribui usuários às funções de um recurso.</span><span class="sxs-lookup"><span data-stu-id="96a9e-184">The access package assigns users to the roles of a resource.</span></span> <span data-ttu-id="96a9e-185">A função típica de um grupo é a função de membro.</span><span class="sxs-lookup"><span data-stu-id="96a9e-185">The typical role of a group is the member role.</span></span> <span data-ttu-id="96a9e-186">Outros recursos, como sites e aplicativos do SharePoint Online, podem ter muitas funções.</span><span class="sxs-lookup"><span data-stu-id="96a9e-186">Other resources, such as SharePoint Online sites and applications, might have many roles.</span></span> <span data-ttu-id="96a9e-187">A função típica de um grupo usado em um pacote de acesso é a função de membro.</span><span class="sxs-lookup"><span data-stu-id="96a9e-187">The typical role of a group used in an access package is the member role.</span></span> <span data-ttu-id="96a9e-188">Você precisará da função de membro ao adicionar uma função de recurso ao pacote de acesso posteriormente neste tutorial.</span><span class="sxs-lookup"><span data-stu-id="96a9e-188">You'll need the member role when you add a resource role to the access package later in this tutorial.</span></span> 

<span data-ttu-id="96a9e-189">Na solicitação, use a **id** do catálogo e a **id** do recurso de grupo no catálogo que você gravou para obter **a originId** da função de recurso Membro.</span><span class="sxs-lookup"><span data-stu-id="96a9e-189">In the request, use the **id** of the catalog and the **id** of the group resource in the catalog that you recorded to get the **originId** of the Member resource role.</span></span> <span data-ttu-id="96a9e-190">Grave o valor da **propriedade originId** a ser usada posteriormente neste tutorial.</span><span class="sxs-lookup"><span data-stu-id="96a9e-190">Record the value of the **originId** property to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="96a9e-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96a9e-191">Request</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/cec5d6ab-c75d-47c0-9c1c-92e89f66e384/accessPackageResourceRoles?$filter=(originSystem+eq+%27AadGroup%27+and+accessPackageResource/id+eq+%274a1e21c5-8a76-4578-acb1-641160e076e8%27+and+displayName+eq+%27Member%27)&$expand=accessPackageResource
```

#### <a name="response"></a><span data-ttu-id="96a9e-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="96a9e-192">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageCatalogs('ede67938-cda7-4127-a9ca-7c7bf86a19b7')/accessPackageResourceRoles(accessPackageResource())",
  "value": [
    {
      "id": "00000000-0000-0000-0000-000000000000",
      "displayName": "Member",
      "description": null,
      "originSystem": "AadGroup",
      "originId": "Member_e93e24d1-2b65-4a6c-a1dd-654a12225487",
      "accessPackageResource@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageCatalogs('cec5d6ab-c75d-47c0-9c1c-92e89f66e384')/accessPackageResourceRoles('00000000-0000-0000-0000-000000000000')/accessPackageResource/$entity",
      "accessPackageResource": {
        "id": "4a1e21c5-8a76-4578-acb1-641160e076e8",
        "displayName": "Marketing resources",
        "description": "Marketing group",
        "url": "https://account.activedirectory.windowsazure.com/r?tenantId=d3030981-8fb9-4919-9980-5580caeddd75#/manageMembership?objectType=Group&objectId=e93e24d1-2b65-4a6c-a1dd-654a12225487",
        "resourceType": "Security Group",
        "originId": "e93e24d1-2b65-4a6c-a1dd-654a12225487",
        "originSystem": "AadGroup",
        "isPendingOnboarding": false,
        "addedBy": "admin@contoso.onmicrosoft.com",
        "addedOn": "2020-06-26T17:13:23.723Z",
        "accessPackageResourceScopes@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageCatalogs('cec5d6ab-c75d-47c0-9c1c-92e89f66e384')/accessPackageResourceRoles('00000000-0000-0000-0000-000000000000')/accessPackageResource/accessPackageResourceScopes",
        "accessPackageResourceScopes": []
      }
    }
  ]
}
```

<span data-ttu-id="96a9e-193">Se bem-sucedido, um único valor é retornado, que representa a função membro desse grupo.</span><span class="sxs-lookup"><span data-stu-id="96a9e-193">If successful, a single value is returned, which represents the Member role of that group.</span></span> <span data-ttu-id="96a9e-194">Se nenhuma função for retornada, verifique os **valores de ID** do catálogo e o recurso do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="96a9e-194">If no roles are returned, check the **id** values of the catalog and the access package resource.</span></span>

### <a name="create-the-access-package"></a><span data-ttu-id="96a9e-195">Criar o pacote de acesso</span><span class="sxs-lookup"><span data-stu-id="96a9e-195">Create the access package</span></span>

<span data-ttu-id="96a9e-196">Neste ponto, você tem um catálogo com um recurso de grupo e sabe que usará a função de recurso do membro do grupo no pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="96a9e-196">At this point, you have a catalog with a group resource, and you know that you'll use the resource role of group member in the access package.</span></span> <span data-ttu-id="96a9e-197">A próxima etapa é criar o pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="96a9e-197">The next step is to create the access package.</span></span> <span data-ttu-id="96a9e-198">Depois de ter o pacote de acesso, você pode adicionar a função de recurso a ele e criar uma política de como os usuários podem solicitar acesso a essa função de recurso.</span><span class="sxs-lookup"><span data-stu-id="96a9e-198">After you have the access package, you can add the resource role to it, and create a policy for how users can request access to that resource role.</span></span> <span data-ttu-id="96a9e-199">Use a **id do** catálogo que você gravou anteriormente para criar o pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="96a9e-199">You use the **id** of the catalog that you recorded earlier to create the access package.</span></span> <span data-ttu-id="96a9e-200">Grave a **id** do pacote de acesso para usar mais adiante neste tutorial.</span><span class="sxs-lookup"><span data-stu-id="96a9e-200">Record the **id** of the access package to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="96a9e-201">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96a9e-201">Request</span></span>

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages
Content-type: application/json

{
  "catalogId": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
  "displayName": "Marketing Campaign",
  "description": "Access to resources for the campaign"
}
```

#### <a name="response"></a><span data-ttu-id="96a9e-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="96a9e-202">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackages/$entity",
  "id": "88203d16-0e31-41d4-87b2-dd402f1435e9",
  "catalogId": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
  "displayName": "Marketing Campaign",
  "description": "Access to resources for the campaign",
  "isHidden": false,
  "isRoleScopesVisible": false,
  "createdBy": "admin@contoso.onmicrosoft.com",
  "createdDateTime": "2020-08-21T19:45:33.2042281Z",
  "modifiedBy": "admin@contoso.onmicrosoft.com",
  "modifiedDateTime": "2020-08-21T19:45:33.2042281Z"
}
```

### <a name="add-a-resource-role-to-the-access-package"></a><span data-ttu-id="96a9e-203">Adicionar uma função de recurso ao pacote de acesso</span><span class="sxs-lookup"><span data-stu-id="96a9e-203">Add a resource role to the access package</span></span>

<span data-ttu-id="96a9e-204">Adicione a função Membro do recurso de grupo ao pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="96a9e-204">Add the Member role of the group resource to the access package.</span></span> <span data-ttu-id="96a9e-205">Na solicitação, forneça a **id** do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="96a9e-205">In the request, provide the **id** of the access package.</span></span> <span data-ttu-id="96a9e-206">No corpo da solicitação, forneça a **id** do recurso do catálogo de grupos para accessPackageResource e forneça a **originId** da função Membro que você gravou anteriormente.</span><span class="sxs-lookup"><span data-stu-id="96a9e-206">In the request body provide the **id** of the group catalog resource for accessPackageResource, and provide the **originId** of the Member role that you previously recorded.</span></span>

#### <a name="request"></a><span data-ttu-id="96a9e-207">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96a9e-207">Request</span></span>

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/88203d16-0e31-41d4-87b2-dd402f1435e9/accessPackageResourceRoleScopes
Content-type: application/json

{
  "accessPackageResourceRole": {
    "originId":"Member_e93e24d1-2b65-4a6c-a1dd-654a12225487",
    "displayName":"Member",
    "originSystem":"AadGroup",
    "accessPackageResource": {
      "id":"4a1e21c5-8a76-4578-acb1-641160e076e8","resourceType":"Security Group",  
      "originId":"e93e24d1-2b65-4a6c-a1dd-654a12225487","originSystem":"AadGroup"
    }
  },
  "accessPackageResourceScope": {
    "originId":"e93e24d1-2b65-4a6c-a1dd-654a12225487","originSystem":"AadGroup"
  }
}
```

#### <a name="response"></a><span data-ttu-id="96a9e-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="96a9e-208">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackages('88203d16-0e31-41d4-87b2-dd402f1435e9')/accessPackageResourceRoleScopes/$entity",
  "id": "e081321b-2802-4834-a6ca-6f598ce3cdf7_6dbd2209-9d14-4c76-b92b-fcb00e835fe1",
  "createdBy": "admin@contoso.onmicrosoft.com",
  "createdDateTime": "2020-08-21T19:56:00.6320729Z",
  "modifiedBy": "admin@contoso.onmicrosoft.com",
  "modifiedDateTime": "2020-08-21T19:56:00.6320729Z"
}
```

<span data-ttu-id="96a9e-209">O pacote de acesso agora tem uma função de recurso, que é a associação de grupo.</span><span class="sxs-lookup"><span data-stu-id="96a9e-209">The access package now has one resource role, which is group membership.</span></span> <span data-ttu-id="96a9e-210">A função é atribuída a qualquer usuário que tenha o pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="96a9e-210">The role is assigned to any user who has the access package.</span></span>

### <a name="create-an-access-package-policy"></a><span data-ttu-id="96a9e-211">Criar uma política de pacote de acesso</span><span class="sxs-lookup"><span data-stu-id="96a9e-211">Create an access package policy</span></span>

<span data-ttu-id="96a9e-212">Agora que você criou o pacote de acesso e adicionou recursos e funções, pode decidir quem pode acessá-lo criando uma política de pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="96a9e-212">Now that you created the access package and added resources and roles, you can decide who can access it by creating an access package policy.</span></span> <span data-ttu-id="96a9e-213">Neste tutorial, você habilita a **conta Solicitante1** que você criou para solicitar acesso aos recursos no pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="96a9e-213">In this tutorial, you enable the **Requestor1** account that you created to request access to the resources in the access package.</span></span> <span data-ttu-id="96a9e-214">Para essa tarefa, você precisa destes valores:</span><span class="sxs-lookup"><span data-stu-id="96a9e-214">For this task, you need these values:</span></span>
- <span data-ttu-id="96a9e-215">**id** do pacote de acesso para o valor da **propriedade accessPackageId**</span><span class="sxs-lookup"><span data-stu-id="96a9e-215">**id** of the access package for the value of the **accessPackageId** property</span></span>
- <span data-ttu-id="96a9e-216">**id** da conta **de usuário Solicitante1** para o valor da **propriedade de id** em **allowedRequestors**</span><span class="sxs-lookup"><span data-stu-id="96a9e-216">**id** of the **Requestor1** user account for the value of the **id** property in **allowedRequestors**</span></span>
 
<span data-ttu-id="96a9e-217">O valor da propriedade **durationInDays** permite que a conta **Solicitante1** acesse os recursos no pacote de acesso por até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="96a9e-217">The value of the **durationInDays** property enables the **Requestor1** account to access the resources in the access package for up to 30 days.</span></span> <span data-ttu-id="96a9e-218">Grave o valor da **propriedade de ID** que será retornada para uso posteriormente neste tutorial.</span><span class="sxs-lookup"><span data-stu-id="96a9e-218">Record the value of the **id** property that is returned to use later in this tutorial.</span></span> 

#### <a name="request"></a><span data-ttu-id="96a9e-219">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96a9e-219">Request</span></span>

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
Content-type: application/json

{
  "accessPackageId": "88203d16-0e31-41d4-87b2-dd402f1435e9",
  "displayName": "Specific users",
  "description": "Specific users can request assignment",
  "accessReviewSettings": null,
  "durationInDays": 30,
  "requestorSettings": {
    "scopeType": "SpecificDirectorySubjects",
    "acceptRequests": true,
    "allowedRequestors": [
       {
         "@odata.type": "#microsoft.graph.singleUser",
         "isBackup": false,
         "id": "007d1c7e-7fa8-4e33-b678-5e437acdcddc",
         "description": "Requestor1"
       }
    ]
  },
  "requestApprovalSettings": {
    "isApprovalRequired": false,
    "isApprovalRequiredForExtension": false,
    "isRequestorJustificationRequired": false,
    "approvalMode": "NoApproval",
    "approvalStages": []
  }
}
```

#### <a name="response"></a><span data-ttu-id="96a9e-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="96a9e-220">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentPolicies/$entity",
  "id": "db440482-1210-4a60-9b55-3ac7a72f63ba",
  "accessPackageId": "88203d16-0e31-41d4-87b2-dd402f1435e9",
  "displayName": "Specific users",
  "description": "Specific users can request assignment",
  "canExtend": false,
  "durationInDays": 30,
  "expirationDateTime": null,
  "createdBy": "admin@contoso.onmicrosoft.com",
  "createdDateTime": "2020-06-29T19:47:44.7399675Z",
  "modifiedBy": "admin@contoso.onmicrosoft.com",
  "modifiedDateTime": "2020-06-29T19:47:44.7555489Z",
  "accessReviewSettings": null,
  "requestorSettings": {
    "scopeType": "SpecificDirectorySubjects",
    "acceptRequests": true,
    "allowedRequestors": [
      {
        "@odata.type": "#microsoft.graph.singleUser",
        "isBackup": false,
        "id": "007d1c7e-7fa8-4e33-b678-5e437acdcddc",
        "description": "Requestor1"
      }
    ]
  },
  "requestApprovalSettings": {
    "isApprovalRequired": false,
    "isApprovalRequiredForExtension": false,
    "isRequestorJustificationRequired": false,
    "approvalMode": "NoApproval",
    "approvalStages": []
  }
}
```

## <a name="step-3-request-access"></a><span data-ttu-id="96a9e-221">Etapa 3: Solicitar acesso</span><span class="sxs-lookup"><span data-stu-id="96a9e-221">Step 3: Request access</span></span>

<span data-ttu-id="96a9e-222">Nesta etapa, a conta **de usuário Solicitante1** solicita acesso aos recursos no pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="96a9e-222">In this step, the **Requestor1** user account requests access to the resources in the access package.</span></span>

<span data-ttu-id="96a9e-223">Para solicitar acesso aos recursos no pacote de acesso, você precisa fornecer estes valores:</span><span class="sxs-lookup"><span data-stu-id="96a9e-223">To request access to resources in the access package, you need to provide these values:</span></span>
- <span data-ttu-id="96a9e-224">**id** da conta **de usuário Solicitante1** que você criou para o valor da **propriedade targetId**</span><span class="sxs-lookup"><span data-stu-id="96a9e-224">**id** of the **Requestor1** user account that you created for the value of the **targetId** property</span></span>
- <span data-ttu-id="96a9e-225">**id** da diretiva de atribuição para o valor da **propriedade assignmentPolicyId**</span><span class="sxs-lookup"><span data-stu-id="96a9e-225">**id** of the assignment policy for the value of the **assignmentPolicyId** property</span></span>
- <span data-ttu-id="96a9e-226">**id** do pacote de acesso para o valor da **propriedade accessPackageId**</span><span class="sxs-lookup"><span data-stu-id="96a9e-226">**id** of the access package for the value of **accessPackageId** property</span></span>

<span data-ttu-id="96a9e-227">Na resposta, você pode ver o status **de Aceito e** um estado de **Enviado.**</span><span class="sxs-lookup"><span data-stu-id="96a9e-227">In the response you can see the status of **Accepted** and a state of **Submitted**.</span></span> <span data-ttu-id="96a9e-228">Registrar o valor da **propriedade de ID** retornada para obter o status da solicitação mais tarde.</span><span class="sxs-lookup"><span data-stu-id="96a9e-228">Record the value of the **id** property that is returned to get the status of the request later.</span></span>

<span data-ttu-id="96a9e-229">Se você ainda não fez isso, saia da conta de administrador que estava usando no Microsoft Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="96a9e-229">If you haven't done so already, sign out of the administrator account that you were using in Microsoft Graph Explorer.</span></span> <span data-ttu-id="96a9e-230">Entre na conta **de usuário Solicitante1** que você criou.</span><span class="sxs-lookup"><span data-stu-id="96a9e-230">Sign in to the **Requestor1** user account that you created.</span></span> <span data-ttu-id="96a9e-231">Você será solicitado a alterar a senha se for a primeira vez que você estiver fazendo login.</span><span class="sxs-lookup"><span data-stu-id="96a9e-231">You will be asked to change the password if it is the first time you are signing in.</span></span>

#### <a name="request"></a><span data-ttu-id="96a9e-232">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96a9e-232">Request</span></span>

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
  "requestType": "UserAdd",
  "accessPackageAssignment":{
     "targetId":"007d1c7e-7fa8-4e33-b678-5e437acdcddc",
     "assignmentPolicyId":"db440482-1210-4a60-9b55-3ac7a72f63ba",
     "accessPackageId":"88203d16-0e31-41d4-87b2-dd402f1435e9"
  }
}
```

#### <a name="response"></a><span data-ttu-id="96a9e-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="96a9e-233">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentRequests/$entity",
    "createdDateTime": null,
    "completedDate": null,
    "id": "a6bb6942-3ae1-4259-9908-0133aaee9377",
    "requestType": "UserAdd",
    "requestState": "Submitted",
    "requestStatus": "Accepted",
    "isValidationOnly": false,
    "expirationDateTime": null,
    "justification": null
}
```

## <a name="step-4-validate-that-access-has-been-assigned"></a><span data-ttu-id="96a9e-234">Etapa 4: Validar se o acesso foi atribuído</span><span class="sxs-lookup"><span data-stu-id="96a9e-234">Step 4: Validate that access has been assigned</span></span>

<span data-ttu-id="96a9e-235">Nesta etapa, confirme se a conta de usuário **Solicitante1** foi atribuída ao pacote de acesso e que agora ele é membro do grupo de recursos **marketing.**</span><span class="sxs-lookup"><span data-stu-id="96a9e-235">In this step, you confirm that the **Requestor1** user account was assigned the access package and that they are now a member of the **Marketing resources** group.</span></span>

<span data-ttu-id="96a9e-236">Saia da conta solicitante1 e entre novamente na conta de administrador para ver o status da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96a9e-236">Sign out of the Requestor1 account and sign back in to the administrator account to see the status of the request.</span></span>

### <a name="get-the-status-of-the-request"></a><span data-ttu-id="96a9e-237">Obter o status da solicitação</span><span class="sxs-lookup"><span data-stu-id="96a9e-237">Get the status of the request</span></span>

<span data-ttu-id="96a9e-238">Use o valor da **propriedade de ID** da solicitação para obter o status atual dela.</span><span class="sxs-lookup"><span data-stu-id="96a9e-238">Use the value of the **id** property of the request to get the current status of it.</span></span> <span data-ttu-id="96a9e-239">Na resposta, você pode ver o status alterado para **Fulfilled** e o estado alterado para **Entregue.**</span><span class="sxs-lookup"><span data-stu-id="96a9e-239">In the response, you can see the status changed to **Fulfilled** and the state changed to **Delivered**.</span></span>

#### <a name="request"></a><span data-ttu-id="96a9e-240">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96a9e-240">Request</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/a6bb6942-3ae1-4259-9908-0133aaee9377
```

#### <a name="response"></a><span data-ttu-id="96a9e-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="96a9e-241">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentRequests/$entity",
  "createdDateTime": "2020-06-29T20:24:24.683Z",
  "completedDate": "2020-06-29T20:24:47.937Z",
  "id": "a6bb6942-3ae1-4259-9908-0133aaee9377",
  "requestType": "UserAdd",
  "requestState": "Delivered",
  "requestStatus": "FulfilledNotificationTriggered",
  "isValidationOnly": false,
  "expirationDateTime": null,
  "justification": null
}
```

### <a name="get-access-package-assignments"></a><span data-ttu-id="96a9e-242">Obter atribuições de pacote de acesso</span><span class="sxs-lookup"><span data-stu-id="96a9e-242">Get access package assignments</span></span>

<span data-ttu-id="96a9e-243">Você também pode usar a **id** da política de pacote de acesso que você criou para ver se os recursos foram atribuídos à conta de usuário **Solicitante1.**</span><span class="sxs-lookup"><span data-stu-id="96a9e-243">You can also use the **id** of the access package policy that you created to see that resources have been assigned to the **Requestor1** user account.</span></span>

#### <a name="request"></a><span data-ttu-id="96a9e-244">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96a9e-244">Request</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=accessPackageAssignmentPolicy/Id eq 'db440482-1210-4a60-9b55-3ac7a72f63ba'
```

#### <a name="response"></a><span data-ttu-id="96a9e-245">Resposta</span><span class="sxs-lookup"><span data-stu-id="96a9e-245">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignments",
  "value": [
    {
      "id": "a6bb6942-3ae1-4259-9908-0133aaee9377",
      "catalogId": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
      "accessPackageId": "88203d16-0e31-41d4-87b2-dd402f1435e9",
      "assignmentPolicyId": "db440482-1210-4a60-9b55-3ac7a72f63ba",
      "targetId": "2bc42425-6dc5-4f2a-9ebb-7a7464481eb0",
      "assignmentStatus": "Delivered",
      "assignmentState": "Delivered",
      "isExtended": false,
      "expiredDateTime": null
    }
  ]
}
```

### <a name="get-the-members-of-the-group"></a><span data-ttu-id="96a9e-246">Obter os membros do grupo</span><span class="sxs-lookup"><span data-stu-id="96a9e-246">Get the members of the group</span></span>

<span data-ttu-id="96a9e-247">Depois que a solicitação for concedida, você poderá usar a **id** registrada para o grupo de recursos **marketing** para ver se a conta de usuário **Solicitante1** foi adicionada a ela.</span><span class="sxs-lookup"><span data-stu-id="96a9e-247">After the request has been granted, you can use the **id** that you recorded for the **Marketing resources** group to see that the **Requestor1** user account has been added to it.</span></span>

#### <a name="request"></a><span data-ttu-id="96a9e-248">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96a9e-248">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/groups/e93e24d1-2b65-4a6c-a1dd-654a12225487/members
```

#### <a name="response"></a><span data-ttu-id="96a9e-249">Resposta:</span><span class="sxs-lookup"><span data-stu-id="96a9e-249">Response:</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "007d1c7e-7fa8-4e33-b678-5e437acdcddc",
      "deletedDateTime": null,
      "accountEnabled": true,
      "ageGroup": null,
      "businessPhones": [],
      "city": null,
      "createdDateTime": "2020-06-23T18:43:24Z",
      "creationType": null,
      "companyName": null,
      "consentProvidedForMinor": null,
      "country": null,
      "department": null,
      "displayName": "Requestor1",
      "employeeId": null,
      "faxNumber": null,
      "givenName": null,
      "imAddresses": [],
      "infoCatalogs": [],
      "isResourceAccount": null,
      "jobTitle": null,
      "legalAgeGroupClassification": null,
      "mail": null,
      "mailNickname": "Requestor1"
    }
  ]
}
```

## <a name="step-5-clean-up-resources"></a><span data-ttu-id="96a9e-250">Etapa 5: Limpar recursos</span><span class="sxs-lookup"><span data-stu-id="96a9e-250">Step 5: Clean up resources</span></span>

<span data-ttu-id="96a9e-251">Nesta etapa, remova as alterações feitas e exclua o pacote de acesso da Campanha de **Marketing.**</span><span class="sxs-lookup"><span data-stu-id="96a9e-251">In this step, you remove the changes you made and delete the **Marketing Campaign** access package.</span></span>

### <a name="remove-an-access-package-assignment"></a><span data-ttu-id="96a9e-252">Remover uma atribuição de pacote de acesso</span><span class="sxs-lookup"><span data-stu-id="96a9e-252">Remove an access package assignment</span></span>

<span data-ttu-id="96a9e-253">Você deve remover todas as atribuições do pacote de acesso antes de excluí-lo.</span><span class="sxs-lookup"><span data-stu-id="96a9e-253">You must remove any assignments to the access package before you can delete it.</span></span> <span data-ttu-id="96a9e-254">Use a **id da** solicitação de atribuição que você gravou anteriormente para excluí-la.</span><span class="sxs-lookup"><span data-stu-id="96a9e-254">Use the **id** of the assignment request that you previously recorded to delete it.</span></span>

#### <a name="request"></a><span data-ttu-id="96a9e-255">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96a9e-255">Request</span></span>

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
  "requestType": "AdminRemove",
  "accessPackageAssignment":{
     "id": "a6bb6942-3ae1-4259-9908-0133aaee9377"
  }
}
```

#### <a name="response"></a><span data-ttu-id="96a9e-256">Resposta</span><span class="sxs-lookup"><span data-stu-id="96a9e-256">Response</span></span>

```http
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentRequests/$entity",
    "createdDateTime": null,
    "completedDate": null,
    "id": "78eaee8c-e6cf-48c9-8f99-aae44c35e379",
    "requestType": "AdminRemove",
    "requestState": "Submitted",
    "requestStatus": "Accepted",
    "isValidationOnly": false,
    "expirationDateTime": null,
    "justification": null
}
```

### <a name="delete-the-access-package-assignment-policy"></a><span data-ttu-id="96a9e-257">Excluir a política de atribuição do pacote de acesso</span><span class="sxs-lookup"><span data-stu-id="96a9e-257">Delete the access package assignment policy</span></span>

<span data-ttu-id="96a9e-258">Use a **id da** diretiva de atribuição que você gravou anteriormente para excluí-la.</span><span class="sxs-lookup"><span data-stu-id="96a9e-258">Use the **id** of the assignment policy that you previously recorded to delete it.</span></span> <span data-ttu-id="96a9e-259">Certifique-se de que todas as atribuições foram removidas primeiro.</span><span class="sxs-lookup"><span data-stu-id="96a9e-259">Make sure all assignments are removed first.</span></span>

#### <a name="request"></a><span data-ttu-id="96a9e-260">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96a9e-260">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/6c1f65ec-8c25-4a45-83c2-a1de2a6d0e9f
```

#### <a name="response"></a><span data-ttu-id="96a9e-261">Resposta</span><span class="sxs-lookup"><span data-stu-id="96a9e-261">Response</span></span>

```http
No Content - 204
```

### <a name="delete-the-access-package"></a><span data-ttu-id="96a9e-262">Excluir o pacote de acesso</span><span class="sxs-lookup"><span data-stu-id="96a9e-262">Delete the access package</span></span>

<span data-ttu-id="96a9e-263">Use a **id do** pacote de acesso que você gravou anteriormente para excluí-lo.</span><span class="sxs-lookup"><span data-stu-id="96a9e-263">Use the **id** of the access package that you previously recorded to delete it.</span></span>

#### <a name="request"></a><span data-ttu-id="96a9e-264">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96a9e-264">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/cf54c6ca-d717-49bc-babe-d140d035dfdd
```

#### <a name="response"></a><span data-ttu-id="96a9e-265">Resposta</span><span class="sxs-lookup"><span data-stu-id="96a9e-265">Response</span></span>

```http
No Content - 204
```

### <a name="delete-the-user-account"></a><span data-ttu-id="96a9e-266">Excluir a conta de usuário</span><span class="sxs-lookup"><span data-stu-id="96a9e-266">Delete the user account</span></span>

<span data-ttu-id="96a9e-267">Exclua **a conta de usuário Solicitante1.**</span><span class="sxs-lookup"><span data-stu-id="96a9e-267">Delete the **Requestor1** user account.</span></span>

#### <a name="request"></a><span data-ttu-id="96a9e-268">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96a9e-268">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/users/ce02eca8-752b-4ecf-ac29-aa9bccd87606
```

#### <a name="response"></a><span data-ttu-id="96a9e-269">Resposta</span><span class="sxs-lookup"><span data-stu-id="96a9e-269">Response</span></span>

```http
No Content - 204
```

### <a name="delete-the-group"></a><span data-ttu-id="96a9e-270">Adicionar ou remover membros do grupo</span><span class="sxs-lookup"><span data-stu-id="96a9e-270">Delete the group</span></span>

<span data-ttu-id="96a9e-271">Exclua o **grupo de recursos marketing.**</span><span class="sxs-lookup"><span data-stu-id="96a9e-271">Delete the **Marketing resources** group.</span></span>

#### <a name="request"></a><span data-ttu-id="96a9e-272">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96a9e-272">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/groups/a468eaea-ed6c-4290-98d2-a96bb1cb4209
```

#### <a name="response"></a><span data-ttu-id="96a9e-273">Resposta</span><span class="sxs-lookup"><span data-stu-id="96a9e-273">Response</span></span>

```http
No Content - 204
```

## <a name="see-also"></a><span data-ttu-id="96a9e-274">Confira também</span><span class="sxs-lookup"><span data-stu-id="96a9e-274">See also</span></span>

<span data-ttu-id="96a9e-275">Neste tutorial, você usou muitas APIs para realizar tarefas.</span><span class="sxs-lookup"><span data-stu-id="96a9e-275">In this tutorial, you used many APIs to accomplish tasks.</span></span> <span data-ttu-id="96a9e-276">Explore a referência de API para essas APIs para saber mais sobre o que as APIs podem fazer.</span><span class="sxs-lookup"><span data-stu-id="96a9e-276">Explore the API reference for these APIs to learn more about what the APIs can do.</span></span>


- [<span data-ttu-id="96a9e-277">Trabalhar com a API de gerenciamento de direitos do Azure AD</span><span class="sxs-lookup"><span data-stu-id="96a9e-277">Working with the Azure AD entitlement management API</span></span>](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta)
- [<span data-ttu-id="96a9e-278">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="96a9e-278">accessPackageCatalog</span></span>](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta)
- [<span data-ttu-id="96a9e-279">accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="96a9e-279">accessPackageResourceRequest</span></span>](/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta)
- [<span data-ttu-id="96a9e-280">accessPackage</span><span class="sxs-lookup"><span data-stu-id="96a9e-280">accessPackage</span></span>](/graph/api/resources/accesspackage?view=graph-rest-beta)
- [<span data-ttu-id="96a9e-281">accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="96a9e-281">accessPackageResourceRoleScope</span></span>](/graph/api/resources/accesspackageresourcerolescope?view=graph-rest-beta)
- [<span data-ttu-id="96a9e-282">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="96a9e-282">accessPackageAssignmentPolicy</span></span>](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta)
- [<span data-ttu-id="96a9e-283">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="96a9e-283">accessPackageAssignmentRequest</span></span>](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta)
- [<span data-ttu-id="96a9e-284">group</span><span class="sxs-lookup"><span data-stu-id="96a9e-284">group</span></span>](/graph/api/resources/group?view=graph-rest-1.0)
- [<span data-ttu-id="96a9e-285">user</span><span class="sxs-lookup"><span data-stu-id="96a9e-285">user</span></span>](/graph/api/resources/user?view=graph-rest-1.0)