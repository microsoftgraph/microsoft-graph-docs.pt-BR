---
title: Use as APIs do Microsoft Graph para configurar o logon único baseado em SAML
description: Aprenda a economizar tempo usando as APIs do Microsoft Graph para automatizar a configuração de logon único baseado em SAML.
author: kenwith
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.custom: scenarios:getting-started
ms.openlocfilehash: 0be3a07c2dec554c25afcb5c228bc392615c9964
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405362"
---
# <a name="automate-saml-based-sso-app-configuration-with-microsoft-graph-api"></a><span data-ttu-id="6c5c0-103">Automação da configuração do aplicativo de SSO baseado em SAML com o Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="6c5c0-103">Automate SAML-based SSO app configuration with Microsoft Graph API</span></span>

<span data-ttu-id="6c5c0-104">Neste artigo, você aprenderá a criar e configurar um aplicativo da galeria do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="6c5c0-104">In this article, you'll learn how to create and configure an application from the Azure Active Directory (Azure AD) Gallery.</span></span> <span data-ttu-id="6c5c0-105">Esse artigo usa o AWS como um exemplo, mas você pode usar as etapas neste artigo para qualquer aplicativo baseado em SAML na galeria do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-105">This article uses AWS as an example, but you can use the steps in this article for any SAML-based app in the Azure AD Gallery.</span></span>

<span data-ttu-id="6c5c0-106">**Etapas para usar as APIs do Microsoft Graph para automatizar a configuração de logon único baseado em SAML**</span><span class="sxs-lookup"><span data-stu-id="6c5c0-106">**Steps to use Microsoft Graph APIs to automate configuration of SAML-based single sign-on**</span></span>

| <span data-ttu-id="6c5c0-107">Etapa</span><span class="sxs-lookup"><span data-stu-id="6c5c0-107">Step</span></span>  | <span data-ttu-id="6c5c0-108">Detalhes</span><span class="sxs-lookup"><span data-stu-id="6c5c0-108">Details</span></span>  |
|---------|---------|
| [<span data-ttu-id="6c5c0-109">1. Criar o aplicativo galeria</span><span class="sxs-lookup"><span data-stu-id="6c5c0-109">1. Create the gallery application</span></span>](#step-1-create-the-gallery-application) | <span data-ttu-id="6c5c0-110">Entrar no cliente da API</span><span class="sxs-lookup"><span data-stu-id="6c5c0-110">Sign in to the API client</span></span> <br> <span data-ttu-id="6c5c0-111">Recuperar o aplicativo galeria</span><span class="sxs-lookup"><span data-stu-id="6c5c0-111">Retrieve the gallery application</span></span> <br> <span data-ttu-id="6c5c0-112">Criar o aplicativo galeria</span><span class="sxs-lookup"><span data-stu-id="6c5c0-112">Create the gallery application</span></span>|
| [<span data-ttu-id="6c5c0-113">2. Configurar o logon único</span><span class="sxs-lookup"><span data-stu-id="6c5c0-113">2. Configure single sign-on</span></span>](#step-2-configure-single-sign-on) | <span data-ttu-id="6c5c0-114">Recuperar ID de objeto do aplicativo e ID do objeto da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="6c5c0-114">Retrieve app object ID and service principal object ID</span></span> <br> <span data-ttu-id="6c5c0-115">Definir o modo de logon único</span><span class="sxs-lookup"><span data-stu-id="6c5c0-115">Set single sign-on mode</span></span> <br> <span data-ttu-id="6c5c0-116">Definir URLs SAML básicas, como identificador, URL de resposta, URL de logon</span><span class="sxs-lookup"><span data-stu-id="6c5c0-116">Set basic SAML URLs such as identifier, reply URL, sign-on URL</span></span> <br> <span data-ttu-id="6c5c0-117">Adicionar funções de aplicativo (opcional)</span><span class="sxs-lookup"><span data-stu-id="6c5c0-117">Add app roles (Optional)</span></span>|
| [<span data-ttu-id="6c5c0-118">3. Configurar mapeamento de declarações</span><span class="sxs-lookup"><span data-stu-id="6c5c0-118">3. Configure claims mapping</span></span>](#step-3-configure-claims-mapping) | <span data-ttu-id="6c5c0-119">Criar política de mapeamento de declarações</span><span class="sxs-lookup"><span data-stu-id="6c5c0-119">Create claims mapping policy</span></span> <br> <span data-ttu-id="6c5c0-120">Atribuir política de mapeamento de declarações à entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="6c5c0-120">Assign claims mapping policy to service principal</span></span>|
| [<span data-ttu-id="6c5c0-121">4. Configurar o certificado de autenticação</span><span class="sxs-lookup"><span data-stu-id="6c5c0-121">4. Configure signing certificate</span></span>](#step-4-configure-signing-certificate) | <span data-ttu-id="6c5c0-122">Criar um certificado</span><span class="sxs-lookup"><span data-stu-id="6c5c0-122">Create a certificate</span></span> <BR> <span data-ttu-id="6c5c0-123">Adicionar uma chave de assinatura personalizada</span><span class="sxs-lookup"><span data-stu-id="6c5c0-123">Add a custom signing key</span></span> <br> <span data-ttu-id="6c5c0-124">Adicionar a chave de assinatura personalizada</span><span class="sxs-lookup"><span data-stu-id="6c5c0-124">Activate the custom signing key</span></span>|
| [<span data-ttu-id="6c5c0-125">5. Atribuir usuários</span><span class="sxs-lookup"><span data-stu-id="6c5c0-125">5. Assign users</span></span>](#step-5-assign-users) | <span data-ttu-id="6c5c0-126">Atribuir usuários e grupos ao aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c5c0-126">Assign users and groups to the application</span></span>
| [<span data-ttu-id="6c5c0-127">6. Configurar o lado do aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c5c0-127">6. Configure the application side</span></span>](#step-6-configure-the-application-side)| <span data-ttu-id="6c5c0-128">Obter os metadados do SAML do Azure AD</span><span class="sxs-lookup"><span data-stu-id="6c5c0-128">Get Azure AD SAML metadata</span></span>

<span data-ttu-id="6c5c0-129">**Lista de todas as APIs usadas no artigo**</span><span class="sxs-lookup"><span data-stu-id="6c5c0-129">**List of all APIs used in the article**</span></span>

<span data-ttu-id="6c5c0-130">Verifique se você tem as permissões correspondentes para chamar as seguintes APIs.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-130">Make sure you have the corresponding permissions to call the following APIs.</span></span>

|<span data-ttu-id="6c5c0-131">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="6c5c0-131">Resource type</span></span> |<span data-ttu-id="6c5c0-132">Método</span><span class="sxs-lookup"><span data-stu-id="6c5c0-132">Method</span></span> |
|---------|---------|
|[<span data-ttu-id="6c5c0-133">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="6c5c0-133">applicationTemplate</span></span>](/graph/api/resources/applicationtemplate?view=graph-rest-beta)|[<span data-ttu-id="6c5c0-134">Lista applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="6c5c0-134">List applicationTemplate</span></span>](/graph/api/applicationtemplate-list?tabs=http&view=graph-rest-beta) <br>[<span data-ttu-id="6c5c0-135">Instanciar o applicationtemplate</span><span class="sxs-lookup"><span data-stu-id="6c5c0-135">Instantiate applicationTemplate</span></span>](/graph/api/applicationtemplate-instantiate?tabs=http&view=graph-rest-beta)|
|[<span data-ttu-id="6c5c0-136">servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="6c5c0-136">servicePrincipals</span></span>](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)|[<span data-ttu-id="6c5c0-137">Atualizar servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="6c5c0-137">Update servicePrincipal</span></span>](/graph/api/serviceprincipal-update?tabs=http&view=graph-rest-1.0) <br> [<span data-ttu-id="6c5c0-138">Criar appRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="6c5c0-138">Create appRoleAssignments</span></span>](/graph/api/serviceprincipal-post-approleassignments?tabs=http&view=graph-rest-1.0) <br> [<span data-ttu-id="6c5c0-139">Atribuir claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="6c5c0-139">Assign claimsMappingPolicies</span></span>](/graph/api/serviceprincipal-post-claimsmappingpolicies?tabs=http&view=graph-rest-beta)|
|[<span data-ttu-id="6c5c0-140">aplicativos</span><span class="sxs-lookup"><span data-stu-id="6c5c0-140">applications</span></span>](/graph/api/resources/application?view=graph-rest-1.0)|[<span data-ttu-id="6c5c0-141">Atualizar aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c5c0-141">Update application</span></span>](/graph/api/application-update?tabs=http&view=graph-rest-1.0)|
|[<span data-ttu-id="6c5c0-142">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="6c5c0-142">claimsMappingPolicy</span></span>](/graph/api/resources/claimsmappingpolicy?view=graph-rest-beta)| [<span data-ttu-id="6c5c0-143">Criar claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="6c5c0-143">Create claimsMappingPolicy</span></span>](/graph/api/claimsmappingpolicy-post-claimsmappingpolicies?tabs=http&view=graph-rest-beta)

>[!NOTE]
><span data-ttu-id="6c5c0-144">Os objetos de resposta mostrados neste artigo poderiam ser reduzidos para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-144">The response objects shown in this article might be shortened for readability.</span></span> <span data-ttu-id="6c5c0-145">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-145">All the properties will be returned from an actual call.</span></span>

## <a name="step-1-create-the-gallery-application"></a><span data-ttu-id="6c5c0-146">Etapa 1: Criar o aplicativo galeria</span><span class="sxs-lookup"><span data-stu-id="6c5c0-146">Step 1: Create the gallery application</span></span>

### <a name="sign-in-to-microsoft-graph-explorer-recommended-postman-or-any-other-api-client-you-use"></a><span data-ttu-id="6c5c0-147">Entrar no Microsoft Graph Explorer (recomendado), no Postman ou em qualquer outro cliente de API que você usa</span><span class="sxs-lookup"><span data-stu-id="6c5c0-147">Sign in to Microsoft Graph Explorer (recommended), Postman, or any other API client you use</span></span>

1. <span data-ttu-id="6c5c0-148">Iniciar [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="6c5c0-148">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
2. <span data-ttu-id="6c5c0-149">Selecione **Entrar com a Microsoft** e entre usando as credenciais de administrador global do Azure AD ou de Administrador do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-149">Select **Sign-In with Microsoft** and sign in using an Azure AD global administrator or App Admin credentials.</span></span>
3. <span data-ttu-id="6c5c0-150">Uma vez acessado, você verá os detalhes da conta do usuário no painel esquerdo.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-150">Upon successful sign-in, you'll see the user account details in the left-hand pane.</span></span>

### <a name="retrieve-the-gallery-application-template-identifier"></a><span data-ttu-id="6c5c0-151">Recuperar o identificador de modelos de aplicativo de galeria</span><span class="sxs-lookup"><span data-stu-id="6c5c0-151">Retrieve the gallery application template identifier</span></span>

<span data-ttu-id="6c5c0-152">Os aplicativos na galeria do aplicativo do Azure AD têm um [modelo de aplicativo](/graph/api/applicationtemplate-list?tabs=http&view=graph-rest-beta) cada um, que descreve os metadados para esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-152">Applications in the Azure AD application gallery each have an [application template](/graph/api/applicationtemplate-list?tabs=http&view=graph-rest-beta) that describes the metadata for that application.</span></span> <span data-ttu-id="6c5c0-153">Usando esse modelo, você pode criar uma instância do aplicativo e da entidade de serviço no locatário para gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-153">Using this template, you can create an instance of the application and service principal in your tenant for management.</span></span>

#### <a name="request"></a><span data-ttu-id="6c5c0-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c5c0-154">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6c5c0-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c5c0-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplates"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applicationTemplates
```
# <a name="c"></a>[<span data-ttu-id="6c5c0-156">C#</span><span class="sxs-lookup"><span data-stu-id="6c5c0-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c5c0-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c5c0-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c5c0-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c5c0-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6c5c0-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c5c0-159">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationTemplate",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
  {
    "id": "8b1025e4-1dd2-430b-a150-2ef79cd700f5",
        "displayName": "Amazon Web Services (AWS)",
        "homePageUrl": "http://aws.amazon.com/",
        "supportedSingleSignOnModes": [
             "password",
             "saml",
             "external"
         ],
         "supportedProvisioningTypes": [
             "sync"
         ],
         "logoUrl": "https://az495088.vo.msecnd.net/app-logo/aws_215.png",
         "categories": [
             "developerServices"
         ],
         "publisher": "Amazon",
         "description": null    
  
}
```

### <a name="create-the-gallery-application"></a><span data-ttu-id="6c5c0-160">Criar o aplicativo galeria</span><span class="sxs-lookup"><span data-stu-id="6c5c0-160">Create the gallery application</span></span>

<span data-ttu-id="6c5c0-161">Usando a ID do modelo que você recuperou para o aplicativo na última etapa, [criar uma instância](/graph/api/applicationtemplate-instantiate?tabs=http&view=graph-rest-beta) do aplicativo e da entidade de serviço em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-161">Using the template ID that you retrieved for your application in the last step, [create an instance](/graph/api/applicationtemplate-instantiate?tabs=http&view=graph-rest-beta) of the application and service principal in your tenant.</span></span>

> [!NOTE] 
> <span data-ttu-id="6c5c0-162">Você pode usar a API applicationTemplate para criar uma instância [aplicativos Não-Galeria](/azure/active-directory/manage-apps/view-applications-portal).</span><span class="sxs-lookup"><span data-stu-id="6c5c0-162">You can use applicationTemplate API to instantiate [Non-Gallery apps](/azure/active-directory/manage-apps/view-applications-portal).</span></span> <span data-ttu-id="6c5c0-163">Usar o applicationTemplateId `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-163">Use applicationTemplateId `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span></span>

> [!NOTE]
> <span data-ttu-id="6c5c0-164">Aguarde algum tempo para que o aplicativo seja provisionado em seu locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-164">Allow some time for the app to be provisioned into your Azure AD tenant.</span></span> <span data-ttu-id="6c5c0-165">Não é instantâneo.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-165">It is not instant.</span></span> <span data-ttu-id="6c5c0-166">Uma estratégia é fazer uma consulta GET sobre o objeto do aplicativo/entidade de serviço a cada 5-10 segundos até que a consulta seja bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-166">One strategy is to do a GET query on the application / service principal object every 5-10 seconds until the query is successful.</span></span>


#### <a name="request"></a><span data-ttu-id="6c5c0-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c5c0-167">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6c5c0-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c5c0-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "applicationtemplate_instantiate"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/applicationTemplates/8b1025e4-1dd2-430b-a150-2ef79cd700f5/instantiate
Content-type: application/json

{
  "displayName": "AWS Contoso"
}
```
# <a name="c"></a>[<span data-ttu-id="6c5c0-169">C#</span><span class="sxs-lookup"><span data-stu-id="6c5c0-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c5c0-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c5c0-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c5c0-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c5c0-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6c5c0-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c5c0-172">Response</span></span>


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationServicePrincipal"
} -->

```http
HTTP/1.1 201 OK
Content-type: application/json


{
    "application": {
        "objectId": "cbc071a6-0fa5-4859-8g55-e983ef63df63",
        "appId": "92653dd4-aa3a-3323-80cf-e8cfefcc8d5d",
        "applicationTemplateId": "8b1025e4-1dd2-430b-a150-2ef79cd700f5",
        "displayName": "AWS Contoso",
        "homepage": "https://signin.aws.amazon.com/saml?metadata=aws|ISV9.1|primary|z",
        "replyUrls": [
            "https://signin.aws.amazon.com/saml"
        ],
        "logoutUrl": null,
        "samlMetadataUrl": null,
    },
    "servicePrincipal": {
        "objectId": "f47a6776-bca7-4f2e-bc6c-eec59d058e3e",
        "appDisplayName": "AWS Contoso",
        "applicationTemplateId": "8b1025e4-1dd2-430b-a150-2ef79cd700f5",
        "appRoleAssignmentRequired": true,
        "displayName": "My custom name",
        "homepage": "https://signin.aws.amazon.com/saml?metadata=aws|ISV9.1|primary|z",
        "replyUrls": [
            "https://signin.aws.amazon.com/saml"
        ],
        "servicePrincipalNames": [
            "93653dd4-aa3a-4323-80cf-e8cfefcc8d7d"
        ],
        "tags": [
            "WindowsAzureActiveDirectoryIntegratedApp"
        ],
    }
}
```

## <a name="step-2-configure-single-sign-on"></a><span data-ttu-id="6c5c0-173">2. Configurar o logon único</span><span class="sxs-lookup"><span data-stu-id="6c5c0-173">Step 2: Configure single sign-on</span></span>

### <a name="retrieve-app-object-id-and-service-principal-object-id"></a><span data-ttu-id="6c5c0-174">Recuperar ID de objeto do aplicativo e ID do objeto da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="6c5c0-174">Retrieve app object ID and service principal object ID</span></span>

<span data-ttu-id="6c5c0-175">Use a resposta da chamada anterior para recuperar e salvar a ID de objeto do aplicativo e a ID do objeto da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-175">Use the response from the previous call to retrieve and save the application object ID and service principal object ID.</span></span>

```
"application": {
        "objectId": "cbc071a6-0fa5-4859-8g55-e983ef63df63"
}
"servicePrincipal": {
        "objectId": "f47a6776-bca7-4f2e-bc6c-eec59d058e3e"
}
```
### <a name="set-single-sign-on-mode"></a><span data-ttu-id="6c5c0-176">Definir o modo de logon único</span><span class="sxs-lookup"><span data-stu-id="6c5c0-176">Set single sign-on mode</span></span>

<span data-ttu-id="6c5c0-177">Neste exemplo, você definirá o `saml` como o modo de logon único na [tipo de recurso de servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="6c5c0-177">In this example, you'll set `saml` as the single sign-on mode in the [servicePrincipal resource type](/graph/api/resources/serviceprincipal?view=graph-rest-1.0).</span></span> <span data-ttu-id="6c5c0-178">Outras propriedades de SSO do SAML que você pode configurar são: `notificationEmailAddresses`, `loginUrl`e `samlSingleSignOnSettings.relayState`.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-178">Other SAML SSO properties that you can configure are: `notificationEmailAddresses`, `loginUrl`, and `samlSingleSignOnSettings.relayState`.</span></span>

<span data-ttu-id="6c5c0-179">Antes dessa consulta funcionar, você precisará fornecer consentimento na guia **Modificar permissões** no Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-179">Before this query will work you need to provide consent on the **Modify permissions** tab in Graph Explorer.</span></span> <span data-ttu-id="6c5c0-180">Além disso, certifique-se de que você está usando a ID do\*\* servicePrincipal\*\* que você obteve anteriormente.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-180">Also, make sure you are using the **servicePrincipal** ID that you obtained earlier.</span></span>

#### <a name="request"></a><span data-ttu-id="6c5c0-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c5c0-181">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6c5c0-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c5c0-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e
Content-type: application/json

{
    "preferredSingleSignOnMode": "saml"
}
```
# <a name="c"></a>[<span data-ttu-id="6c5c0-183">C#</span><span class="sxs-lookup"><span data-stu-id="6c5c0-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c5c0-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c5c0-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c5c0-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c5c0-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6c5c0-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c5c0-186">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204
```

### <a name="set-basic-saml-urls-such-as-identifier-reply-url-sign-on-url"></a><span data-ttu-id="6c5c0-187">Definir URLs SAML básicas, como identificador, URL de resposta, URL de logon</span><span class="sxs-lookup"><span data-stu-id="6c5c0-187">Set basic SAML URLs such as identifier, reply URL, sign-on URL</span></span>

<span data-ttu-id="6c5c0-188">Defina o identificador e as URLs de resposta para AWS no objeto do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-188">Set the identifier and reply URLs for AWS in the application object.</span></span>

<span data-ttu-id="6c5c0-189"> Verifique se você está usando a ID de **aplicativo** obtida anteriormente.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-189">Make sure you are using the **application** id obtained earlier.</span></span>

#### <a name="request"></a><span data-ttu-id="6c5c0-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c5c0-190">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6c5c0-191">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c5c0-191">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/applications/cbc071a6-0fa5-4859-8g55-e983ef63df63
Content-type: applications/json

{
    "web": {
        "redirectUris": [
            "https://signin.aws.amazon.com/saml"
        ] 
    },
    "identifierUris": [
        "https://signin.aws.amazon.com/saml"
    ]    
}
```
# <a name="c"></a>[<span data-ttu-id="6c5c0-192">C#</span><span class="sxs-lookup"><span data-stu-id="6c5c0-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c5c0-193">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c5c0-193">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c5c0-194">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c5c0-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6c5c0-195">Java</span><span class="sxs-lookup"><span data-stu-id="6c5c0-195">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipals-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6c5c0-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c5c0-196">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204
```
### <a name="add-app-roles-optional"></a><span data-ttu-id="6c5c0-197">Adicionar funções de aplicativo (opcional)</span><span class="sxs-lookup"><span data-stu-id="6c5c0-197">Add app roles (Optional)</span></span>

<span data-ttu-id="6c5c0-198">Se o aplicativo exigir as informações da função no token, adicione a definição das funções no objeto do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-198">If the application requires the role information in the token, add the definition of the roles in the application object.</span></span> <span data-ttu-id="6c5c0-199">No AWS, você pode [habilitar o provisionamento de usuário](/azure/active-directory/app-provisioning/application-provisioning-configure-api) para buscar todas as funções dessa conta do AWS.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-199">For AWS, you can [enable user provisioning](/azure/active-directory/app-provisioning/application-provisioning-configure-api) to fetch all the roles from that AWS account.</span></span> 

<span data-ttu-id="6c5c0-200">Para saber mais, confira [Configurar a declaração de função emitida no token SAML](/azure/active-directory/develop/active-directory-enterprise-app-role-management).</span><span class="sxs-lookup"><span data-stu-id="6c5c0-200">For more information, see [Configure the role claim issued in the SAML token](/azure/active-directory/develop/active-directory-enterprise-app-role-management).</span></span>

> [!NOTE] 
> <span data-ttu-id="6c5c0-201">Ao adicionar funções de aplicativo, não modifique as funções de aplicativo padrão msiam_access.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-201">When adding app roles, don't modify the default app roles msiam_access.</span></span> 

#### <a name="request"></a><span data-ttu-id="6c5c0-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c5c0-202">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6c5c0-203">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c5c0-203">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/serviceprincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e
Content-type: application/json

{
"appRoles": [
        {
            "allowedMemberTypes": [
                "User"
            ],
            "description": "msiam_access",
            "displayName": "msiam_access",
            "id": "7dfd756e-8c27-4472-b2b7-38c17fc5de5e",
            "isEnabled": true,
            "origin": "Application",
            "value": null
        },
        {
            "allowedMemberTypes": [
                "User"
            ],
            "description": "Admin,WAAD",
            "displayName": "Admin,WAAD",
            "id": "454dc4c2-8176-498e-99df-8c4efcde41ef",
            "isEnabled": true,
            "value": "arn:aws:iam::212743507312:role/accountname-aws-admin,arn:aws:iam::212743507312:saml-provider/WAAD"
        },
        {
            "allowedMemberTypes": [
                "User"
            ],
            "description": "Finance,WAAD",
            "displayName": "Finance,WAAD",
            "id": "8642d5fa-18a3-4245-ab8c-a96000c1a217",
            "isEnabled": true,
            "value": "arn:aws:iam::212743507312:role/accountname-aws-finance,arn:aws:iam::212743507312:saml-provider/WAAD"
        }
    ]

}
```
# <a name="c"></a>[<span data-ttu-id="6c5c0-204">C#</span><span class="sxs-lookup"><span data-stu-id="6c5c0-204">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c5c0-205">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c5c0-205">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c5c0-206">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c5c0-206">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6c5c0-207">Java</span><span class="sxs-lookup"><span data-stu-id="6c5c0-207">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipals-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6c5c0-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c5c0-208">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204
```

## <a name="step-3-configure-claims-mapping"></a><span data-ttu-id="6c5c0-209">3. Configurar mapeamento de declarações</span><span class="sxs-lookup"><span data-stu-id="6c5c0-209">Step 3: Configure claims mapping</span></span>

### <a name="create-claims-mapping-policy"></a><span data-ttu-id="6c5c0-210">Criar política de mapeamento de declarações</span><span class="sxs-lookup"><span data-stu-id="6c5c0-210">Create claims mapping policy</span></span>

<span data-ttu-id="6c5c0-211">Além das declarações básicas, configure as seguintes declarações para o Azure AD emitir no token SAML:</span><span class="sxs-lookup"><span data-stu-id="6c5c0-211">In addition to the basic claims, configure the following claims for Azure AD to emit in the SAML token:</span></span>

| <span data-ttu-id="6c5c0-212">Nome da declaração</span><span class="sxs-lookup"><span data-stu-id="6c5c0-212">Claim name</span></span> | <span data-ttu-id="6c5c0-213">Origem</span><span class="sxs-lookup"><span data-stu-id="6c5c0-213">Source</span></span>  |
|---------|---------|
| `https://aws.amazon.com/SAML/Attributes/Role` | <span data-ttu-id="6c5c0-214">assignedroles</span><span class="sxs-lookup"><span data-stu-id="6c5c0-214">assignedroles</span></span>| 
| `https://aws.amazon.com/SAML/Attributes/RoleSessionName` | <span data-ttu-id="6c5c0-215">userprincipalname</span><span class="sxs-lookup"><span data-stu-id="6c5c0-215">userprincipalname</span></span> |
| `https://aws.amazon.com/SAML/Attributes/SessionDuration` | <span data-ttu-id="6c5c0-216">"900"</span><span class="sxs-lookup"><span data-stu-id="6c5c0-216">"900"</span></span> |
| <span data-ttu-id="6c5c0-217">funções</span><span class="sxs-lookup"><span data-stu-id="6c5c0-217">roles</span></span> | <span data-ttu-id="6c5c0-218">assignedroles</span><span class="sxs-lookup"><span data-stu-id="6c5c0-218">assignedroles</span></span> |
| `http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier` | <span data-ttu-id="6c5c0-219">userprincipalname</span><span class="sxs-lookup"><span data-stu-id="6c5c0-219">userprincipalname</span></span> |

<span data-ttu-id="6c5c0-220">Para obter mais informações, confira [Personalizar as declarações emitidas no token](/azure/active-directory/develop/active-directory-claims-mapping).</span><span class="sxs-lookup"><span data-stu-id="6c5c0-220">For more information, see [Customize claims emitted in token](/azure/active-directory/develop/active-directory-claims-mapping).</span></span>

> [!NOTE]
> <span data-ttu-id="6c5c0-221">Algumas chaves na política de mapeamento de declarações são sensíveis a letras maiúsculas e minúsculas (por exemplo, "Version").</span><span class="sxs-lookup"><span data-stu-id="6c5c0-221">Some keys in the claims mapping policy are case sensitive (for example, "Version").</span></span> <span data-ttu-id="6c5c0-222">Se você receber uma mensagem de erro como "A propriedade tem um valor inválido", isso poderia ser um problema de diferenciação de maiúsculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-222">If you receive an error message such as "Property has an invalid value", it might be a case sensitive issue.</span></span>

#### <a name="request"></a><span data-ttu-id="6c5c0-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c5c0-223">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6c5c0-224">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c5c0-224">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies
Content-type: application/json

{
    "definition": [
        "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\", \"ClaimsSchema\": [{\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/Role\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/RoleSessionName\"}, {\"Value\":\"900\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/SessionDuration\"}, {\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"appRoles\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier\"}]}}"
    ],
    "displayName": "AWS Claims Policy",
    "isOrganizationDefault": false
}
```
# <a name="c"></a>[<span data-ttu-id="6c5c0-225">C#</span><span class="sxs-lookup"><span data-stu-id="6c5c0-225">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c5c0-226">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c5c0-226">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c5c0-227">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c5c0-227">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6c5c0-228">Java</span><span class="sxs-lookup"><span data-stu-id="6c5c0-228">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipals-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6c5c0-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c5c0-229">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicies",
  "isCollection": true
} -->

```http
HTTP/1.1 201 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/claimsMappingPolicies/$entity",
    "id": "a7b19e62-9adb-4edb-8521-cd35305f095d",
    "deletedDateTime": null,
    "definition": [
        "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\", \"ClaimsSchema\": [{\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/Role\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/RoleSessionName\"}, {\"Value\":\"900\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/SessionDuration\"}, {\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"appRoles\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier\"}]}}"
    ],
    "displayName": "AWS Claims Policy",
    "isOrganizationDefault": false
}
```

### <a name="assign-claims-mapping-policy-to-service-principal"></a><span data-ttu-id="6c5c0-230">Atribuir política de mapeamento de declarações à entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="6c5c0-230">Assign claims mapping policy to service principal</span></span>

#### <a name="request"></a><span data-ttu-id="6c5c0-231">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c5c0-231">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e/claimsMappingPolicies/$ref

Content-type: application/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/6b33aa8e-51f3-41a6-a0fd-d660d276197a"
}
```


#### <a name="response"></a><span data-ttu-id="6c5c0-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c5c0-232">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204
```

## <a name="step-4-configure-signing-certificate"></a><span data-ttu-id="6c5c0-233">Etapa 4. Configurar o certificado de autenticação</span><span class="sxs-lookup"><span data-stu-id="6c5c0-233">Step 4: Configure signing certificate</span></span>

<span data-ttu-id="6c5c0-234">Usar a API [applicationtemplate](/graph/api/resources/applicationtemplate?view=graph-rest-beta) não cria um certificado de autenticação por padrão.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-234">Using the [applicationTemplate](/graph/api/resources/applicationtemplate?view=graph-rest-beta) API doesn't create a signing certificate by default.</span></span> <span data-ttu-id="6c5c0-235">Crie seu certificado de assinatura personalizado e atribua-o ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-235">Create your custom signing cert and assign it to the application.</span></span> 

### <a name="create-a-custom-signing-certificate"></a><span data-ttu-id="6c5c0-236">Criar um certificado de autenticação personalizado</span><span class="sxs-lookup"><span data-stu-id="6c5c0-236">Create a custom signing certificate</span></span>

<span data-ttu-id="6c5c0-237">Para testar, use o seguinte comando do Windows PowerShell para obter um certificado autoassinado.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-237">To test, you can use the following PowerShell command to get a self-signed certificate.</span></span> <span data-ttu-id="6c5c0-238">Você precisará manipular e extrair os valores necessários manualmente usando outras ferramentas.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-238">You will then need to manipulate and pull the values you need manually using other tools.</span></span> <span data-ttu-id="6c5c0-239">Use a prática recomendada de segurança da sua empresa para criar um certificado de autenticação para produção.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-239">Use the best security practice from your company to create a signing certificate for production.</span></span>

```powershell
Param(
    [Parameter(Mandatory=$true)]
    [string]$fqdn,
    [Parameter(Mandatory=$true)]
    [string]$pwd,
    [Parameter(Mandatory=$true)]
    [string]$location
) 

if (!$PSBoundParameters.ContainsKey('location'))
{
    $location = "."
} 

$cert = New-SelfSignedCertificate -certstorelocation cert:\currentuser\my -DnsName $fqdn
$pwdSecure = ConvertTo-SecureString -String $pwd -Force -AsPlainText
$path = 'cert:\currentuser\my\' + $cert.Thumbprint
$cerFile = $location + "\\" + $fqdn + ".cer"
$pfxFile = $location + "\\" + $fqdn + ".pfx" 

Export-PfxCertificate -cert $path -FilePath $pfxFile -Password $pwdSecure
Export-Certificate -cert $path -FilePath $cerFile
```

<span data-ttu-id="6c5c0-240">Como alternativa, o seguinte aplicativo de console C# pode ser usado como Prova de Conceito para entender como os valores necessários podem ser obtidos.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-240">Alternatively, the following C# console app can be used as a Proof of Concept to understand how the required values can be obtained.</span></span> <span data-ttu-id="6c5c0-241">Observe que este código é para **aprendizado e referência APENAS** e não devem ser usados como estão na produção.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-241">Note that this code is for **learning and reference ONLY** and should not be used as-is in production.</span></span>

```csharp
using System;
using System.Security.Cryptography;
using System.Security.Cryptography.X509Certificates;
using System.Text;


/* CONSOLE APP - PROOF OF CONCEPT CODE ONLY!!
 * This code uses a self signed certificate and should not be used 
 * in production. This code is for reference and learning ONLY.
 */
namespace Self_signed_cert
{
    class Program
    {
        static void Main(string[] args)
        {
            // Generate a guid to use as a password and then create the cert.
            string password = Guid.NewGuid().ToString();
            var selfsignedCert = buildSelfSignedServerCertificate(password);

            // Print values so we can copy paste into the JSON fields.
            // Print out the private key in base64 format.
            Console.WriteLine("Private Key: {0}{1}", Convert.ToBase64String(selfsignedCert.Export(X509ContentType.Pfx, password)), Environment.NewLine);

            // Print out the start date in ISO 8601 format.
            DateTime startDate = DateTime.Parse(selfsignedCert.GetEffectiveDateString()).ToUniversalTime();
            Console.WriteLine("For All startDateTime: " + startDate.ToString("o"));

            // Print out the end date in ISO 8601 format.
            DateTime endDate = DateTime.Parse(selfsignedCert.GetExpirationDateString()).ToUniversalTime();
            Console.WriteLine("For All endDateTime: " + endDate.ToString("o"));

            // Print the GUID used for keyId
            string signAndPasswordGuid = Guid.NewGuid().ToString();
            string verifyGuid = Guid.NewGuid().ToString();
            Console.WriteLine("GUID to use for keyId for keyCredentials->Usage == Sign and passwordCredentials: " + signAndPasswordGuid);
            Console.WriteLine("GUID to use for keyId for keyCredentials->Usage == Verify: " + verifyGuid);

            // Print out the password.
            Console.WriteLine("Password is: {0}", password);

            // Print out a displayName to use as an example.
            Console.WriteLine("displayName to use: CN=Example");
            Console.WriteLine();

            // Print out the public key.
            Console.WriteLine("Public Key: {0}{1}", Convert.ToBase64String(selfsignedCert.Export(X509ContentType.Cert)), Environment.NewLine);
            Console.WriteLine();

            // Generate the customKeyIdentifier using hash of thumbprint.
            Console.WriteLine("You can generate the customKeyIdentifier by getting the SHA256 hash of the certs thumprint.\nThe certs thumbprint is: {0}{1}", selfsignedCert.Thumbprint, Environment.NewLine);
            Console.WriteLine("The hash of the thumbprint that we will use for customeKeyIdentifier is:");
            string keyIdentifier = GetSha256FromThumbprint(selfsignedCert.Thumbprint);
            Console.WriteLine(keyIdentifier);
        }

        // Generate a self-signed certificate.
        private static X509Certificate2 buildSelfSignedServerCertificate(string password)
        {
            const string CertificateName = @"Microsoft Azure Federated SSO Certificate TEST";
            DateTime certificateStartDate = DateTime.UtcNow;
            DateTime certificateEndDate = certificateStartDate.AddYears(2).ToUniversalTime();

            X500DistinguishedName distinguishedName = new X500DistinguishedName($"CN={CertificateName}");

            using (RSA rsa = RSA.Create(2048))
            {
                var request = new CertificateRequest(distinguishedName, rsa, HashAlgorithmName.SHA256, RSASignaturePadding.Pkcs1);

                request.CertificateExtensions.Add(
                    new X509KeyUsageExtension(X509KeyUsageFlags.DataEncipherment | X509KeyUsageFlags.KeyEncipherment | X509KeyUsageFlags.DigitalSignature, false));

                var certificate = request.CreateSelfSigned(new DateTimeOffset(certificateStartDate), new DateTimeOffset(certificateEndDate));
                certificate.FriendlyName = CertificateName;

                return new X509Certificate2(certificate.Export(X509ContentType.Pfx, password), password, X509KeyStorageFlags.Exportable);
            }
        }

        // Generate hash from thumbprint.
        public static string GetSha256FromThumbprint(string thumbprint)
        {
            var message = Encoding.ASCII.GetBytes(thumbprint);
            SHA256Managed hashString = new SHA256Managed();
            return Convert.ToBase64String(hashString.ComputeHash(message));
        }
    }
}
```

### <a name="add-a-custom-signing-key"></a><span data-ttu-id="6c5c0-242">Adicionar uma chave de assinatura personalizada</span><span class="sxs-lookup"><span data-stu-id="6c5c0-242">Add a custom signing key</span></span>

<span data-ttu-id="6c5c0-243">Adicione as seguintes informações à entidade de serviço:</span><span class="sxs-lookup"><span data-stu-id="6c5c0-243">Add the following information to the service principal:</span></span>

* <span data-ttu-id="6c5c0-244">Chave privada</span><span class="sxs-lookup"><span data-stu-id="6c5c0-244">Private key</span></span>
* <span data-ttu-id="6c5c0-245">Senha</span><span class="sxs-lookup"><span data-stu-id="6c5c0-245">Password</span></span>
* <span data-ttu-id="6c5c0-246">Chave pública</span><span class="sxs-lookup"><span data-stu-id="6c5c0-246">Public key</span></span> 

<span data-ttu-id="6c5c0-247">Extraia a chave pública e privada Base64 do arquivo PFX.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-247">Extract the private and public key Base64 encoded from the PFX file.</span></span> <span data-ttu-id="6c5c0-248">Para saber mais sobre as propriedades, confira [tipo de recurso de keyCredential](/graph/api/resources/keycredential?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="6c5c0-248">To learn more about the properties, see [keyCredential resource type](/graph/api/resources/keycredential?view=graph-rest-1.0).</span></span>

<span data-ttu-id="6c5c0-249">Certifique-se de que a keyId da keyCredential usada para "Assinar" corresponda à keyId da passwordCredential.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-249">Make sure that the keyId for the keyCredential used for "Sign" matches the keyId of the passwordCredential.</span></span> <span data-ttu-id="6c5c0-250">Você pode gerar o `customkeyIdentifier` ao obter o hash da impressão digital do certificado.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-250">You can generate the `customkeyIdentifier` by getting the hash of the cert's thumbprint.</span></span> <span data-ttu-id="6c5c0-251">Consulte o C# código de referência anterior.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-251">See the previous C# reference code.</span></span>

#### <a name="request"></a><span data-ttu-id="6c5c0-252">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c5c0-252">Request</span></span>

> [!NOTE]
> <span data-ttu-id="6c5c0-253">O valor "chave" na propriedade keyCredentials é reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-253">The "key" value in the keyCredentials property is shortened for readability.</span></span> <span data-ttu-id="6c5c0-254">O valor é base 64 codificado.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-254">The value is base 64 encoded.</span></span> <span data-ttu-id="6c5c0-255">Para a chave particular, a propriedade `usage` é "Assinar".</span><span class="sxs-lookup"><span data-stu-id="6c5c0-255">For the private key the property `usage` is "Sign".</span></span> <span data-ttu-id="6c5c0-256">Para a chave pública, a propriedade `usage` é "Verificar".</span><span class="sxs-lookup"><span data-stu-id="6c5c0-256">For the public key the property `usage` is "Verify".</span></span>

<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e

Content-type: application/json

{
    "keyCredentials":[
        {
            "customKeyIdentifier": "lY85bR8r6yWTW6jnciNEONwlVhDyiQjdVLgPDnkI5mA=",
            "endDateTime": "2021-04-22T22:10:13Z",
            "keyId": "4c266507-3e74-4b91-aeba-18a25b450f6e",
            "startDateTime": "2020-04-22T21:50:13Z",
            "type": "X509CertAndPassword",
            "usage": "Sign",
            "key":"MIIKIAIBAz.....HBgUrDgMCERE20nuTptI9MEFCh2Ih2jaaLZBZGeZBRFVNXeZmAAgIH0A==",
            "displayName": "CN=awsAPI"
        },
        {
            "customKeyIdentifier": "lY85bR8r6yWTW6jnciNEONwlVhDyiQjdVLgPDnkI5mA=",
            "endDateTime": "2021-04-22T22:10:13Z",
            "keyId": "e35a7d11-fef0-49ad-9f3e-aacbe0a42c42",
            "startDateTime": "2020-04-22T21:50:13Z",
            "type": "AsymmetricX509Cert",
            "usage": "Verify",
            "key": "MIIDJzCCAg+gAw......CTxQvJ/zN3bafeesMSueR83hlCSyg==",
            "displayName": "CN=awsAPI"
        }

    ],
    "passwordCredentials": [
        {
            "customKeyIdentifier": "lY85bR8r6yWTW6jnciNEONwlVhDyiQjdVLgPDnkI5mA=",
            "keyId": "4c266507-3e74-4b91-aeba-18a25b450f6e",
            "endDateTime": "2022-01-27T19:40:33Z",
            "startDateTime": "2020-04-20T19:40:33Z",
            "secretText": "61891f4ee44d"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="6c5c0-257">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c5c0-257">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204
```

### <a name="activate-the-custom-signing-key"></a><span data-ttu-id="6c5c0-258">Adicionar a chave de assinatura personalizada</span><span class="sxs-lookup"><span data-stu-id="6c5c0-258">Activate the custom signing key</span></span>

<span data-ttu-id="6c5c0-259">É necessário definir a propriedade `preferredTokenSigningKeyThumbprint` como a impressão digital do certificado que você deseja que o Azure AD use para assinar a resposta SAML.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-259">You need to set the `preferredTokenSigningKeyThumbprint` property to the thumbprint of the certificate you want Azure AD to use to sign the SAML response.</span></span> 

#### <a name="request"></a><span data-ttu-id="6c5c0-260">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c5c0-260">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e

Content-type: application/json

{
    "preferredTokenSigningKeyThumbprint": "AC09FEF18DDE6983EE2A164FBA3C4DD7518BD787"
}
```

#### <a name="response"></a><span data-ttu-id="6c5c0-261">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c5c0-261">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204
```
## <a name="step-5-assign-users"></a><span data-ttu-id="6c5c0-262">Etapa 5. Atribuir usuários</span><span class="sxs-lookup"><span data-stu-id="6c5c0-262">Step 5: Assign users</span></span>

### <a name="assign-users-and-groups-to-the-application"></a><span data-ttu-id="6c5c0-263">Atribuir usuários e grupos ao aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c5c0-263">Assign users and groups to the application</span></span>

<span data-ttu-id="6c5c0-264">Atribua o seguinte usuário à entidade de serviço e atribua o AWS_Role1.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-264">Assign the following user to the service principal and assign the AWS_Role1.</span></span> 

| <span data-ttu-id="6c5c0-265">Nome</span><span class="sxs-lookup"><span data-stu-id="6c5c0-265">Name</span></span>  | <span data-ttu-id="6c5c0-266">ID</span><span class="sxs-lookup"><span data-stu-id="6c5c0-266">ID</span></span>  |
|---------|---------|
| <span data-ttu-id="6c5c0-267">ID de usuário (principalId)</span><span class="sxs-lookup"><span data-stu-id="6c5c0-267">User ID (principalId)</span></span> | <span data-ttu-id="6c5c0-268">6cad4079-4e79-4a3f-9efb-ea30a14bdb26</span><span class="sxs-lookup"><span data-stu-id="6c5c0-268">6cad4079-4e79-4a3f-9efb-ea30a14bdb26</span></span> |
| <span data-ttu-id="6c5c0-269">Type (principalType)</span><span class="sxs-lookup"><span data-stu-id="6c5c0-269">Type (principalType)</span></span> | <span data-ttu-id="6c5c0-270">Usuário</span><span class="sxs-lookup"><span data-stu-id="6c5c0-270">User</span></span> |
| <span data-ttu-id="6c5c0-271">ID da função do aplicativo (appRoleId)</span><span class="sxs-lookup"><span data-stu-id="6c5c0-271">App role ID (appRoleId)</span></span> | <span data-ttu-id="6c5c0-272">454dc4c2-8176-498e-99df-8c4efcde41ef</span><span class="sxs-lookup"><span data-stu-id="6c5c0-272">454dc4c2-8176-498e-99df-8c4efcde41ef</span></span> |
| <span data-ttu-id="6c5c0-273">servicePrincipalID (resourceId)</span><span class="sxs-lookup"><span data-stu-id="6c5c0-273">servicePrincipalID (resourceId)</span></span> | <span data-ttu-id="6c5c0-274">f47a6776-bca7-4f2e-bc6c-eec59d058e3e</span><span class="sxs-lookup"><span data-stu-id="6c5c0-274">f47a6776-bca7-4f2e-bc6c-eec59d058e3e</span></span> |

#### <a name="request"></a><span data-ttu-id="6c5c0-275">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c5c0-275">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e/appRoleAssignments

Content-type: application/json

{
  "principalId": "6cad4079-4e79-4a3f-9efb-ea30a14bdb26",
  "principalType": "User",
  "appRoleId":"454dc4c2-8176-498e-99df-8c4efcde41ef",
  "resourceId":"f47a6776-bca7-4f2e-bc6c-eec59d058e3e"
}
```

#### <a name="response"></a><span data-ttu-id="6c5c0-276">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c5c0-276">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 201 
Content-type: application/json

{
    "id": "rq7hyzl4yECaNZleMrTpDV-OCe5TEl5Ao_o76XMrRFU",
    "creationTimestamp": "2020-04-23T17:38:13.2508567Z",
    "appRoleId": "454dc4c2-8176-498e-99df-8c4efcde41ef",
    "principalDisplayName": "User 1",
    "principalId": "6cad4079-4e79-4a3f-9efb-ea30a14bdb26",
    "principalType": "User",
    "resourceDisplayName": "AWS API Created",
    "resourceId": "f47a6776-bca7-4f2e-bc6c-eec59d058e3e"
}
```

<span data-ttu-id="6c5c0-277">Para saber mais, confira o [appRoleAssignment](/graph/api/resources/approleassignment?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="6c5c0-277">For more information, see [appRoleAssignment](/graph/api/resources/approleassignment?view=graph-rest-1.0).</span></span>

## <a name="step-6-configure-the-application-side"></a><span data-ttu-id="6c5c0-278">Etapa 6. Configurar o lado do aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c5c0-278">Step 6: Configure the application side</span></span>

### <a name="get-azure-ad-saml-metadata"></a><span data-ttu-id="6c5c0-279">Obter os metadados do SAML do Azure AD</span><span class="sxs-lookup"><span data-stu-id="6c5c0-279">Get Azure AD SAML metadata</span></span>

<span data-ttu-id="6c5c0-280">Use a URL a seguir para obter os metadados do SAML do Azure AD para o aplicativo específico configurado.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-280">Use the following URL to get the Azure AD SAML metadata for the specific configured application.</span></span> <span data-ttu-id="6c5c0-281">Os metadados contêm informações como o certificado de assinatura, o Azure AD entityID e o Azure AD SingleSignOnService, entre outras.</span><span class="sxs-lookup"><span data-stu-id="6c5c0-281">The metadata contains information such as the signing certificate, Azure AD entityID, and Azure AD SingleSignOnService, among others.</span></span>

`https://login.microsoftonline.com/{tenant-id}/federationmetadata/2007-06/federationmetadata.xml?appid={app-id}`

## <a name="next-steps"></a><span data-ttu-id="6c5c0-282">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="6c5c0-282">Next steps</span></span>
- [<span data-ttu-id="6c5c0-283">Use as APIs do Microsoft Graph para configurar o provisionamento de usuário</span><span class="sxs-lookup"><span data-stu-id="6c5c0-283">Use Microsoft Graph APIs to configure user provisioning</span></span>](/azure/active-directory/app-provisioning/application-provisioning-configure-api)
- [<span data-ttu-id="6c5c0-284">Use o relatório de atividade do aplicativo AD FS para migrar aplicativos para o Azure AD</span><span class="sxs-lookup"><span data-stu-id="6c5c0-284">Use the AD FS application activity report to migrate applications to Azure AD</span></span>](/azure/active-directory/manage-apps/migrate-adfs-application-activity)
