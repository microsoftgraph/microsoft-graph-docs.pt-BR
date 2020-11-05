---
title: Configurar o proxy de aplicativo usando as APIs do Microsoft Graph
description: Configure automaticamente o proxy de aplicativo usando as APIs do Microsoft Graph para fornecer acesso remoto e logon único para aplicativos locais.
author: davidmu1
ms.topic: conceptual
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5052555b16b81170d8a6aa04f1c26c13fcd8d320
ms.sourcegitcommit: 366178d3fc37439791061082da80a63fba2c27df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2020
ms.locfileid: "48921792"
---
# <a name="automate-the-configuration-of-application-proxy-using-the-microsoft-graph-api"></a><span data-ttu-id="ddebd-103">Automatizar a configuração do Proxy de aplicativo usando a API do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ddebd-103">Automate the configuration of Application Proxy using the Microsoft Graph API</span></span>

<span data-ttu-id="ddebd-104">Neste artigo, você aprenderá a criar e configurar o [proxy de aplicativo](/azure/active-directory/manage-apps/what-is-application-proxy) do Azure Active Directory (Azure AD) para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ddebd-104">In this article, you'll learn how to create and configure Azure Active Directory (Azure AD) [Application Proxy](/azure/active-directory/manage-apps/what-is-application-proxy) for an application.</span></span> <span data-ttu-id="ddebd-105">O proxy de aplicativo fornece acesso remoto seguro e logon único em aplicativos Web no local.</span><span class="sxs-lookup"><span data-stu-id="ddebd-105">Application Proxy provides secure remote access and single sign-on to on-premises web applications.</span></span> <span data-ttu-id="ddebd-106">Depois de configurar o proxy de aplicativo para um aplicativo, os usuários podem acessar seus aplicativos locais por meio de uma URL externa, do portal de meus aplicativos ou de outros portais de aplicativos internos.</span><span class="sxs-lookup"><span data-stu-id="ddebd-106">After configuring Application Proxy for an application, users can access their on-premises applications through an external URL, the My Apps portal, or other internal application portals.</span></span>

<span data-ttu-id="ddebd-107">Este artigo pressupõe que você já instalou um conector e concluiu os [pré-requisitos](/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) para o proxy de aplicativo para que os conectores possam se comunicar com os serviços do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ddebd-107">This article assumes you have already installed a connector and completed the [prerequisites](/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) for Application Proxy so that connectors can communicate with Azure AD services.</span></span>

<span data-ttu-id="ddebd-108">Verifique se você tem as permissões correspondentes para chamar as seguintes APIs.</span><span class="sxs-lookup"><span data-stu-id="ddebd-108">Make sure you have the corresponding permissions to call the following APIs.</span></span>

|<span data-ttu-id="ddebd-109">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="ddebd-109">Resource type</span></span> |<span data-ttu-id="ddebd-110">Método</span><span class="sxs-lookup"><span data-stu-id="ddebd-110">Method</span></span> |
|---------|---------|
|[<span data-ttu-id="ddebd-111">aplicativos</span><span class="sxs-lookup"><span data-stu-id="ddebd-111">applications</span></span>](/graph/api/resources/application?view=graph-rest-1.0)<br> [<span data-ttu-id="ddebd-112">onPremisesPublishing</span><span class="sxs-lookup"><span data-stu-id="ddebd-112">onPremisesPublishing</span></span>](/graph/api/resources/onpremisespublishing?view=graph-rest-beta)| [<span data-ttu-id="ddebd-113">Criar aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddebd-113">Create application</span></span>](/graph/api/application-post-applications?tabs=http&view=graph-rest-beta) <br> [<span data-ttu-id="ddebd-114">Atualizar aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddebd-114">Update application</span></span>](/graph/api/application-update?view=graph-rest-beta)<br> [<span data-ttu-id="ddebd-115">Adicionar aplicativo ao um conector</span><span class="sxs-lookup"><span data-stu-id="ddebd-115">Add application to connectorGroup</span></span>](/graph/api/connectorgroup-post-applications?view=graph-rest-beta)|
|[<span data-ttu-id="ddebd-116">connector</span><span class="sxs-lookup"><span data-stu-id="ddebd-116">connector</span></span>](/graph/api/resources/connector?view=graph-rest-beta)| [<span data-ttu-id="ddebd-117">Obter conectores</span><span class="sxs-lookup"><span data-stu-id="ddebd-117">Get connectors</span></span>](/graph/api/connector-get?view=graph-rest-beta)
|[<span data-ttu-id="ddebd-118">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="ddebd-118">connectorGroup</span></span>](/graph/api/resources/connectorGroup?view=graph-rest-beta)| [<span data-ttu-id="ddebd-119">Criar connectorGroup</span><span class="sxs-lookup"><span data-stu-id="ddebd-119">Create connectorGroup</span></span>](/graph/api/resources/connectorgroup?view=graph-rest-beta) <br> [<span data-ttu-id="ddebd-120">Adicionar conector a connectorGroup</span><span class="sxs-lookup"><span data-stu-id="ddebd-120">Add connector to connectorGroup</span></span>](/graph/api/connector-post-memberof?view=graph-rest-beta) <br> |
|[<span data-ttu-id="ddebd-121">servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="ddebd-121">servicePrincipals</span></span>](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)|[<span data-ttu-id="ddebd-122">Criar servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="ddebd-122">Create servicePrincipal</span></span>](/graph/api/serviceprincipal-post-serviceprincipals?tabs=http&view=graph-rest-beta) <br> [<span data-ttu-id="ddebd-123">Atualizar servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="ddebd-123">Update servicePrincipal</span></span>](/graph/api/serviceprincipal-update?tabs=http&view=graph-rest-1.0) <br> [<span data-ttu-id="ddebd-124">Criar appRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="ddebd-124">Create appRoleAssignments</span></span>](/graph/api/serviceprincipal-post-approleassignments?view=graph-rest-beta)|

> [!NOTE]
> <span data-ttu-id="ddebd-125">As solicitações mostradas neste artigo usam valores de amostra.</span><span class="sxs-lookup"><span data-stu-id="ddebd-125">The requests shown in this article use sample values.</span></span> <span data-ttu-id="ddebd-126">Você precisará atualizá-los.</span><span class="sxs-lookup"><span data-stu-id="ddebd-126">You will need update these.</span></span> <span data-ttu-id="ddebd-127">Os objetos Response mostrados também podem ser reduzidos para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="ddebd-127">The response objects shown might also be shortened for readability.</span></span> 

## <a name="step-1-create-an-application"></a><span data-ttu-id="ddebd-128">Etapa 1: criar um aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddebd-128">Step 1: Create an application</span></span>

### <a name="sign-in-to-microsoft-graph-explorer-recommended-postman-or-any-other-api-client-you-use"></a><span data-ttu-id="ddebd-129">Entrar no Microsoft Graph Explorer (recomendado), no Postman ou em qualquer outro cliente de API que você usa</span><span class="sxs-lookup"><span data-stu-id="ddebd-129">Sign in to Microsoft Graph Explorer (recommended), Postman, or any other API client you use</span></span>

1. <span data-ttu-id="ddebd-130">Iniciar [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="ddebd-130">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
2. <span data-ttu-id="ddebd-131">Selecione **entrar com a Microsoft** e entre usando um administrador global do Azure ad ou credenciais de administrador de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="ddebd-131">Select **Sign-in with Microsoft** and sign in using an Azure AD global administrator or App Admin credentials.</span></span>
3. <span data-ttu-id="ddebd-132">Após entrar com êxito, você verá os detalhes da conta de usuário no painel esquerdo.</span><span class="sxs-lookup"><span data-stu-id="ddebd-132">Upon successful sign in, you'll see the user account details in the left pane.</span></span>

### <a name="create-an-application"></a><span data-ttu-id="ddebd-133">Criar um aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddebd-133">Create an application</span></span>

<span data-ttu-id="ddebd-134">Para configurar o proxy de aplicativo para um aplicativo usando a API, você cria um aplicativo, adiciona uma entidade de serviço ao aplicativo e, em seguida, atualiza a propriedade **onPremisesPublishing** do aplicativo para definir as configurações de proxy de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ddebd-134">To configure Application Proxy for an app using the API, you create an application, add a service principal to the app, and then update the application's **onPremisesPublishing** property to configure the App Proxy settings.</span></span> <span data-ttu-id="ddebd-135">Ao criar o aplicativo, defina o **signInAudience** do aplicativo como "AzureADMyOrg".</span><span class="sxs-lookup"><span data-stu-id="ddebd-135">When creating the application, set the application's **signInAudience** to "AzureADMyOrg".</span></span>

#### <a name="request"></a><span data-ttu-id="ddebd-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddebd-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ddebd-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddebd-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_application"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/applications
Content-type: application/json

{
  "displayName": "Contoso IWA App",
  "signInAudience":"AzureADMyOrg"
}
```
# <a name="c"></a>[<span data-ttu-id="ddebd-138">C#</span><span class="sxs-lookup"><span data-stu-id="ddebd-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ddebd-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddebd-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ddebd-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddebd-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ddebd-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddebd-141">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->

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

### <a name="retrieve-the-application-object-id-and-appid"></a><span data-ttu-id="ddebd-142">Recuperar a ID de objeto de aplicativo e appId</span><span class="sxs-lookup"><span data-stu-id="ddebd-142">Retrieve the application object ID and appId</span></span>
<span data-ttu-id="ddebd-143">Use a resposta da chamada anterior para recuperar e salvar a ID do objeto de aplicativo e a ID do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ddebd-143">Use the response from the previous call to retrieve and save the application object ID and app ID.</span></span>
```
"application": {
  "id": "bf21f7e9-9d25-4da2-82ab-7fdd85049f83",
  "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b"
}
```
### <a name="create-a-serviceprincipal-for-the-application-and-add-required-tags"></a><span data-ttu-id="ddebd-144">Criar um servicePrincipalName para o aplicativo e adicionar marcas necessárias</span><span class="sxs-lookup"><span data-stu-id="ddebd-144">Create a servicePrincipal for the application and add required tags</span></span>
<span data-ttu-id="ddebd-145">Use a **AppID** para criar uma entidade de serviço para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ddebd-145">Use the **appId** to create a service principal for the application.</span></span> <span data-ttu-id="ddebd-146">Em seguida, adicione as marcas necessárias para configurar o proxy de aplicativo para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ddebd-146">Then add the tags required for configuring Application Proxy for an app.</span></span>

#### <a name="request"></a><span data-ttu-id="ddebd-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddebd-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ddebd-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddebd-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_servicePrincipal"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/serviceprincipals
Content-type: appplication/json

{
  "appId":"d7fbfe28-c60e-46d2-8335-841923950d3b",
  "tags": [
    "WindowsAzureActiveDirectoryIntegratedApp",
    "WindowsAzureActiveDirectoryOnPremApp"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="ddebd-149">C#</span><span class="sxs-lookup"><span data-stu-id="ddebd-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ddebd-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddebd-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ddebd-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddebd-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ddebd-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddebd-152">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals/$entity",
  "id": "a8cac399-cde5-4516-a674-819503c61313",
  "deletedDateTime": null,
  "accountEnabled": true,
  "alternativeNames": [],
  "createdDateTime": null,
  "deviceManagementAppType": null,
  "appDescription": null,
  "appDisplayName": "Contoso IWA App",
  "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b",
  "applicationTemplateId": null,
  "appOwnerOrganizationId": "7918d4b5-0442-4a97-be2d-36f9f9962ece",
  "appRoleAssignmentRequired": false,
  "description": null,
  "displayName": "vtestapi2",
  "errorUrl": null,
  "homepage": null,
  "isAuthorizationServiceEnabled": false,
  "loginUrl": null,
  "logoutUrl": null,
  "notes": null,
  "notificationEmailAddresses": [],
  "preferredSingleSignOnMode": null,
  "preferredTokenSigningKeyEndDateTime": null,
  "preferredTokenSigningKeyThumbprint": null,
  "publisherName": "f/128 Photography",
  "replyUrls": [],
  "samlMetadataUrl": null,
  "samlSingleSignOnSettings": null,
  "servicePrincipalNames": [
      "b92b92d4-3874-46a5-b715-a00ea01cff93"
  ],
  "servicePrincipalType": "Application",
}
```

## <a name="step-2-configure-application-proxy-properties"></a><span data-ttu-id="ddebd-153">Etapa 2: configurar as propriedades do proxy de aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddebd-153">Step 2: Configure Application Proxy properties</span></span>

### <a name="set-the-onpremisespublishing-configuration"></a><span data-ttu-id="ddebd-154">Definir a configuração do onPremisesPublishing</span><span class="sxs-lookup"><span data-stu-id="ddebd-154">Set the onPremisesPublishing configuration</span></span>

<span data-ttu-id="ddebd-155">Use a ID de objeto de aplicativo da etapa anterior para configurar o proxy de aplicativo para o aplicativo e atualizar a propriedade **onPremisesPublishing** para a configuração desejada.</span><span class="sxs-lookup"><span data-stu-id="ddebd-155">Use the application object ID from the previous step to configure Application Proxy for the app and update the **onPremisesPublishing** property to the desired configuration.</span></span> <span data-ttu-id="ddebd-156">Neste exemplo, você está usando um aplicativo com a URL interna: `https://contosoiwaapp.com` e usando o domínio padrão para a URL externa: `https://contosoiwaapp-contoso.msappproxy.net` .</span><span class="sxs-lookup"><span data-stu-id="ddebd-156">In this example, you're using an app with the internal URL: `https://contosoiwaapp.com` and using the default domain for the external URL: `https://contosoiwaapp-contoso.msappproxy.net`.</span></span> 

#### <a name="request"></a><span data-ttu-id="ddebd-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddebd-157">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ddebd-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddebd-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_application"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83
Content-type: appplication/json

{
    "onPremisesPublishing": {
        "externalAuthenticationType": "aadPreAuthentication",
        "internalUrl": "https://contosoiwaapp.com",
        "externalUrl": "https://contosoiwaapp-contoso.msappproxy.net"
    }
}
```
# <a name="c"></a>[<span data-ttu-id="ddebd-159">C#</span><span class="sxs-lookup"><span data-stu-id="ddebd-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ddebd-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddebd-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ddebd-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddebd-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ddebd-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddebd-162">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```
### <a name="complete-the-configuration-of-the-application"></a><span data-ttu-id="ddebd-163">Concluir a configuração do aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddebd-163">Complete the configuration of the application</span></span>
<span data-ttu-id="ddebd-164">Atualize as propriedades **redirectUri** , **identifierUri** e **HOMEPAGEURL** do aplicativo para a ur externa configurada na propriedade **onPremisesPublishing** .</span><span class="sxs-lookup"><span data-stu-id="ddebd-164">Update the application's **redirectUri** , **identifierUri** , and **homepageUrl** properties to the external UR configured in the **onPremisesPublishing** property.</span></span> <span data-ttu-id="ddebd-165">Em seguida, atualize o [implicitGrantSettings](/graph/api/resources/implicitgrantsettings?view=graph-rest-1.0) para o `true` **EnabledTokenIssuance** e `false` para o **enabledAccessTokenIssuance**.</span><span class="sxs-lookup"><span data-stu-id="ddebd-165">Then update [implicitGrantSettings](/graph/api/resources/implicitgrantsettings?view=graph-rest-1.0) to `true` for **enabledTokenIssuance** and `false` for **enabledAccessTokenIssuance**.</span></span>

#### <a name="request"></a><span data-ttu-id="ddebd-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddebd-166">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_application"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83
Content-type: appplication/json

{
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

#### <a name="response"></a><span data-ttu-id="ddebd-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddebd-167">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-3-assign-the-connector-group-to-the-application"></a><span data-ttu-id="ddebd-168">Etapa 3: atribuir o grupo de conectores ao aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddebd-168">Step 3: Assign the connector group to the application</span></span>

### <a name="get-connectors"></a><span data-ttu-id="ddebd-169">Obter conectores</span><span class="sxs-lookup"><span data-stu-id="ddebd-169">Get connectors</span></span>

<span data-ttu-id="ddebd-170">Liste os conectores e use a resposta para recuperar e salvar a ID de objeto do conector.</span><span class="sxs-lookup"><span data-stu-id="ddebd-170">List the connectors and use the response to retrieve and save the connector object ID.</span></span> <span data-ttu-id="ddebd-171">A ID do objeto Connector será usada para atribuir o conector a um grupo de conectores.</span><span class="sxs-lookup"><span data-stu-id="ddebd-171">The connector object ID will be used to assign the connector to a connector group.</span></span>

#### <a name="request"></a><span data-ttu-id="ddebd-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddebd-172">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ddebd-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddebd-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "connector"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors

```
# <a name="c"></a>[<span data-ttu-id="ddebd-174">C#</span><span class="sxs-lookup"><span data-stu-id="ddebd-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ddebd-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddebd-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ddebd-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddebd-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ddebd-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddebd-177">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectors",
  "isCollection": true
} -->

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
        },
        {
            "id": "8555cc3c-5c8b-48a8-a8b2-5e97c32ef907",
            "machineName": "connectorC.contoso.com",
            "externalIp": "40.78.66.161",
            "status": "active"
        }
    ]
}
```

### <a name="create-a-connectorgroup"></a><span data-ttu-id="ddebd-178">Criar um um dos conectores</span><span class="sxs-lookup"><span data-stu-id="ddebd-178">Create a connectorGroup</span></span>
<span data-ttu-id="ddebd-179">Para este exemplo, um novo grupo de conectores é criado com o nome "grupo de conectores de demonstração do IWA" que é usado para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ddebd-179">For this example, a new connectorGroup is created named "IWA Demo Connector Group" that is used for the application.</span></span> <span data-ttu-id="ddebd-180">Você também pode ignorar esta etapa se o seu conector já estiver atribuído ao conector apropriado.</span><span class="sxs-lookup"><span data-stu-id="ddebd-180">You can also skip this step if your connector is already assigned to the appropriate connectorGroup.</span></span> <span data-ttu-id="ddebd-181">Recupere e salve a ID de objeto do The Connector para usar na próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="ddebd-181">Retrieve and save the connectorGroup object ID to use in the next step.</span></span>

#### <a name="request"></a><span data-ttu-id="ddebd-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddebd-182">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "connectorGroup"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups

Content-type: application/json
{
   "name": "IWA Demo Connector Group"
}
```

#### <a name="response"></a><span data-ttu-id="ddebd-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddebd-183">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

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

### <a name="assign-a-connector-to-the-connectorgroup"></a><span data-ttu-id="ddebd-184">Atribuir um conector ao conector</span><span class="sxs-lookup"><span data-stu-id="ddebd-184">Assign a connector to the connectorGroup</span></span>

#### <a name="request"></a><span data-ttu-id="ddebd-185">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddebd-185">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "connectorGroup"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/8555cc3c-5c8b-48a8-a8b2-5e97c32ef907/memberOf/$ref

Content-type: application/json
{
  "@odata.id":"https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/3e6f4c35-a04b-4d03-b98a-66fff89b72e6"
}
```

#### <a name="response"></a><span data-ttu-id="ddebd-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddebd-186">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

### <a name="assign-the-application-to-the-connectorgroup"></a><span data-ttu-id="ddebd-187">Atribuir o aplicativo ao conector</span><span class="sxs-lookup"><span data-stu-id="ddebd-187">Assign the application to the connectorGroup</span></span>

#### <a name="request"></a><span data-ttu-id="ddebd-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddebd-188">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ddebd-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddebd-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "connectorGroup"
}-->

```msgraph-interactive
PUT https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83/connectorGroup/$ref
Content-type: application/json

{
"@odata.id":"https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/3e6f4c35-a04b-4d03-b98a-66fff89b72e6"
}
```
# <a name="c"></a>[<span data-ttu-id="ddebd-190">C#</span><span class="sxs-lookup"><span data-stu-id="ddebd-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ddebd-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddebd-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ddebd-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddebd-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ddebd-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddebd-193">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-4-configure-single-sign-on"></a><span data-ttu-id="ddebd-194">Etapa 4: configurar o logon único</span><span class="sxs-lookup"><span data-stu-id="ddebd-194">Step 4: Configure single sign-on</span></span>
<span data-ttu-id="ddebd-195">Este aplicativo usa a autenticação integrada do Windows (IWA).</span><span class="sxs-lookup"><span data-stu-id="ddebd-195">This application uses Integrated Windows Authentication (IWA).</span></span> <span data-ttu-id="ddebd-196">Para configurar o IWA, defina as propriedades de logon único no tipo de recurso [singleSignOnSettings](/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta) .</span><span class="sxs-lookup"><span data-stu-id="ddebd-196">To configure IWA, set the single sign-on properties in the [singleSignOnSettings](/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta) resource type.</span></span>

#### <a name="request"></a><span data-ttu-id="ddebd-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddebd-197">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_application"
}-->

```msgraph-interactive
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

#### <a name="response"></a><span data-ttu-id="ddebd-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddebd-198">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-5-assign-users"></a><span data-ttu-id="ddebd-199">Etapa 5. Atribuir usuários</span><span class="sxs-lookup"><span data-stu-id="ddebd-199">Step 5: Assign users</span></span>
### <a name="retrieve-approle-for-the-applicaiton"></a><span data-ttu-id="ddebd-200">Recuperar appRole para o aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddebd-200">Retrieve appRole for the applicaiton</span></span>

#### <a name="request"></a><span data-ttu-id="ddebd-201">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddebd-201">Request</span></span>



# <a name="http"></a>[<span data-ttu-id="ddebd-202">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddebd-202">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/a8cac399-cde5-4516-a674-819503c61313/appRoles
```
# <a name="c"></a>[<span data-ttu-id="ddebd-203">C#</span><span class="sxs-lookup"><span data-stu-id="ddebd-203">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ddebd-204">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddebd-204">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ddebd-205">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddebd-205">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ddebd-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddebd-206">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
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
        {
            "allowedMemberTypes": [
                "User"
            ],
            "description": "msiam_access",
            "displayName": "msiam_access",
            "id": "b9632174-c057-4f7e-951b-be3adc52bfe6",
            "isEnabled": true,
            "origin": "Application",
            "value": null
        }
    ]
}
```

<span data-ttu-id="ddebd-207">Use a resposta da chamada anterior para recuperar e salvar a ID de appRole a ser usada para a próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="ddebd-207">Use the response from the previous call to retrieve and save the appRole ID to use for the next step.</span></span>
```
      {
            "description": "User",
            "displayName": "User",
            "id": "18d14569-c3bd-439b-9a66-3a2aee01d14f"
        }
```

### <a name="assign-users-and-groups-to-the-application"></a><span data-ttu-id="ddebd-208">Atribuir usuários e grupos ao aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddebd-208">Assign users and groups to the application</span></span>

<span data-ttu-id="ddebd-209">Use as propriedades a seguir para atribuir um usuário ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ddebd-209">Use the following properties to assign a user to the application.</span></span>

| <span data-ttu-id="ddebd-210">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ddebd-210">Property</span></span>  | <span data-ttu-id="ddebd-211">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddebd-211">Description</span></span> |<span data-ttu-id="ddebd-212">ID</span><span class="sxs-lookup"><span data-stu-id="ddebd-212">ID</span></span>  |
|---------|---------|---------|
| <span data-ttu-id="ddebd-213">principalId</span><span class="sxs-lookup"><span data-stu-id="ddebd-213">principalId</span></span> | <span data-ttu-id="ddebd-214">ID de usuário do usuário que será atribuído ao aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddebd-214">User ID of the user that will be assigned to the app</span></span> | <span data-ttu-id="ddebd-215">2fe96d23-5dc6-4f35-8222-0426a8c115c8</span><span class="sxs-lookup"><span data-stu-id="ddebd-215">2fe96d23-5dc6-4f35-8222-0426a8c115c8</span></span> |
| <span data-ttu-id="ddebd-216">principalType</span><span class="sxs-lookup"><span data-stu-id="ddebd-216">principalType</span></span> | <span data-ttu-id="ddebd-217">Tipo de usuário</span><span class="sxs-lookup"><span data-stu-id="ddebd-217">Type of user</span></span> | <span data-ttu-id="ddebd-218">Usuário</span><span class="sxs-lookup"><span data-stu-id="ddebd-218">User</span></span> |
| <span data-ttu-id="ddebd-219">appRoleId</span><span class="sxs-lookup"><span data-stu-id="ddebd-219">appRoleId</span></span> |  <span data-ttu-id="ddebd-220">A ID de função de aplicativo da função de aplicativo padrão do aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddebd-220">The App role ID of the default app role of the app</span></span> | <span data-ttu-id="ddebd-221">18d14569-c3bd-439b-9a66-3a2aee01d14f</span><span class="sxs-lookup"><span data-stu-id="ddebd-221">18d14569-c3bd-439b-9a66-3a2aee01d14f</span></span> |
| <span data-ttu-id="ddebd-222">resourceId</span><span class="sxs-lookup"><span data-stu-id="ddebd-222">resourceId</span></span> | <span data-ttu-id="ddebd-223">A ID de servicePrincipalName do aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddebd-223">The servicePrincipal ID of the app</span></span> | <span data-ttu-id="ddebd-224">a8cac399-cde5-4516-a674-819503c61313</span><span class="sxs-lookup"><span data-stu-id="ddebd-224">a8cac399-cde5-4516-a674-819503c61313</span></span> |

#### <a name="request"></a><span data-ttu-id="ddebd-225">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddebd-225">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/servicePrincipals/b00c693f-9658-4c06-bd1b-c402c4653dea/appRoleAssignments

Content-type: appRoleAssignments/json

{
  "principalId": "2fe96d23-5dc6-4f35-8222-0426a8c115c8",
  "principalType": "User",
  "appRoleId":"18d14569-c3bd-439b-9a66-3a2aee01d14f",
  "resourceId":"a8cac399-cde5-4516-a674-819503c61313"
}
```

#### <a name="response"></a><span data-ttu-id="ddebd-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddebd-226">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 200
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appRoleAssignments/$entity",
    "id": "I23pL8ZdNU-CIgQmqMEVyLJ0E6fx0ixEo92az8MnhtU",
    "creationTimestamp": "2020-06-09T00:06:07.5129268Z",
    "appRoleId": "18d14569-c3bd-439b-9a66-3a2aee01d14f",
    "principalDisplayName": "Jean Green",
    "principalId": "2fe96d23-5dc6-4f35-8222-0426a8c115c8",
    "principalType": "User",
    "resourceDisplayName": "Contoso IWA App",
    "resourceId": "a8cac399-cde5-4516-a674-819503c61313"
}
```

<span data-ttu-id="ddebd-227">Para saber mais, confira o tipo de recurso [appRoleAssignment](/graph/api/resources/approleassignment?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="ddebd-227">For more information, see [appRoleAssignment](/graph/api/resources/approleassignment?view=graph-rest-beta) resource type.</span></span>


## <a name="additional-steps"></a><span data-ttu-id="ddebd-228">Etapas adicionais</span><span class="sxs-lookup"><span data-stu-id="ddebd-228">Additional steps</span></span>
- [<span data-ttu-id="ddebd-229">Configuração automatizada usando exemplos do PowerShell para o proxy de aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddebd-229">Automate configuration using PowerShell samples for Application Proxy</span></span>](/azure/active-directory/manage-apps/application-proxy-powershell-samples.md)
- [<span data-ttu-id="ddebd-230">Automação da configuração do aplicativo de SSO baseado em SAML com a API do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ddebd-230">Automate SAML-based SSO app configuration with Microsoft Graph API</span></span>](/azure/active-directory/manage-apps/application-saml-sso-configure-api.md)