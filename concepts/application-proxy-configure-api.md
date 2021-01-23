---
title: Configurar o Proxy de Aplicativo usando as APIs do Microsoft Graph
description: Configure automaticamente o Proxy de Aplicativo usando as APIs do Microsoft Graph para fornecer acesso remoto e logon único a aplicativos locais.
author: davidmu1
ms.topic: conceptual
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 28bb376b094a648d246bba5401764952d5aec863
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49943679"
---
# <a name="automate-the-configuration-of-application-proxy-using-the-microsoft-graph-api"></a><span data-ttu-id="fb657-103">Automatizar a configuração do Proxy de aplicativo usando a API do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="fb657-103">Automate the configuration of Application Proxy using the Microsoft Graph API</span></span>

<span data-ttu-id="fb657-104">Neste artigo, você aprenderá a criar e configurar o [Proxy](/azure/active-directory/manage-apps/what-is-application-proxy) de aplicativo do Azure Active Directory (Azure AD) para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb657-104">In this article, you'll learn how to create and configure Azure Active Directory (Azure AD) [Application Proxy](/azure/active-directory/manage-apps/what-is-application-proxy) for an application.</span></span> <span data-ttu-id="fb657-105">O Proxy de Aplicativo fornece acesso remoto seguro e o single sign-on para aplicativos Web locais.</span><span class="sxs-lookup"><span data-stu-id="fb657-105">Application Proxy provides secure remote access and single sign-on to on-premises web applications.</span></span> <span data-ttu-id="fb657-106">Depois de configurar o Proxy de Aplicativo para um aplicativo, os usuários podem acessar seus aplicativos locais por meio de uma URL externa, o portal Meus Aplicativos ou outros portais de aplicativos internos.</span><span class="sxs-lookup"><span data-stu-id="fb657-106">After configuring Application Proxy for an application, users can access their on-premises applications through an external URL, the My Apps portal, or other internal application portals.</span></span>

<span data-ttu-id="fb657-107">Este artigo assume que você já instalou [](/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) um conector e concluiu os pré-requisitos para o Proxy de Aplicativo para que os conectores possam se comunicar com os serviços do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fb657-107">This article assumes you have already installed a connector and completed the [prerequisites](/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) for Application Proxy so that connectors can communicate with Azure AD services.</span></span>

<span data-ttu-id="fb657-108">Verifique se você tem as permissões correspondentes para chamar as seguintes APIs.</span><span class="sxs-lookup"><span data-stu-id="fb657-108">Make sure you have the corresponding permissions to call the following APIs.</span></span>

|<span data-ttu-id="fb657-109">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="fb657-109">Resource type</span></span> |<span data-ttu-id="fb657-110">Método</span><span class="sxs-lookup"><span data-stu-id="fb657-110">Method</span></span> |
|---------|---------|
|[<span data-ttu-id="fb657-111">aplicativos</span><span class="sxs-lookup"><span data-stu-id="fb657-111">applications</span></span>](/graph/api/resources/application?view=graph-rest-1.0)<br> [<span data-ttu-id="fb657-112">onPremisesPublishing</span><span class="sxs-lookup"><span data-stu-id="fb657-112">onPremisesPublishing</span></span>](/graph/api/resources/onpremisespublishing?view=graph-rest-beta)| [<span data-ttu-id="fb657-113">Criar aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb657-113">Create application</span></span>](/graph/api/application-post-applications?tabs=http&view=graph-rest-beta) <br> [<span data-ttu-id="fb657-114">Atualizar aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb657-114">Update application</span></span>](/graph/api/application-update?view=graph-rest-beta)<br> [<span data-ttu-id="fb657-115">Adicionar aplicativo ao connectorGroup</span><span class="sxs-lookup"><span data-stu-id="fb657-115">Add application to connectorGroup</span></span>](/graph/api/connectorgroup-post-applications?view=graph-rest-beta)|
|[<span data-ttu-id="fb657-116">connector</span><span class="sxs-lookup"><span data-stu-id="fb657-116">connector</span></span>](/graph/api/resources/connector?view=graph-rest-beta)| [<span data-ttu-id="fb657-117">Obter conectores</span><span class="sxs-lookup"><span data-stu-id="fb657-117">Get connectors</span></span>](/graph/api/connector-get?view=graph-rest-beta)
|[<span data-ttu-id="fb657-118">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="fb657-118">connectorGroup</span></span>](/graph/api/resources/connectorGroup?view=graph-rest-beta)| [<span data-ttu-id="fb657-119">Criar connectorGroup</span><span class="sxs-lookup"><span data-stu-id="fb657-119">Create connectorGroup</span></span>](/graph/api/resources/connectorgroup?view=graph-rest-beta) <br> [<span data-ttu-id="fb657-120">Adicionar conector a connectorGroup</span><span class="sxs-lookup"><span data-stu-id="fb657-120">Add connector to connectorGroup</span></span>](/graph/api/connector-post-memberof?view=graph-rest-beta) <br> |
|[<span data-ttu-id="fb657-121">servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="fb657-121">servicePrincipals</span></span>](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)|[<span data-ttu-id="fb657-122">Criar servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="fb657-122">Create servicePrincipal</span></span>](/graph/api/serviceprincipal-post-serviceprincipals?tabs=http&view=graph-rest-beta) <br> [<span data-ttu-id="fb657-123">Atualizar servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="fb657-123">Update servicePrincipal</span></span>](/graph/api/serviceprincipal-update?tabs=http&view=graph-rest-1.0) <br> [<span data-ttu-id="fb657-124">Criar appRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="fb657-124">Create appRoleAssignments</span></span>](/graph/api/serviceprincipal-post-approleassignments?view=graph-rest-beta)|

> [!NOTE]
> <span data-ttu-id="fb657-125">As solicitações mostradas neste artigo usam valores de exemplo.</span><span class="sxs-lookup"><span data-stu-id="fb657-125">The requests shown in this article use sample values.</span></span> <span data-ttu-id="fb657-126">Você precisará atualizá-los.</span><span class="sxs-lookup"><span data-stu-id="fb657-126">You will need update these.</span></span> <span data-ttu-id="fb657-127">Os objetos de resposta mostrados também podem ser reduzidos para maior leitura.</span><span class="sxs-lookup"><span data-stu-id="fb657-127">The response objects shown might also be shortened for readability.</span></span> 

## <a name="step-1-create-an-application"></a><span data-ttu-id="fb657-128">Etapa 1: Criar um aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb657-128">Step 1: Create an application</span></span>

### <a name="sign-in-to-microsoft-graph-explorer-recommended-postman-or-any-other-api-client-you-use"></a><span data-ttu-id="fb657-129">Entrar no Microsoft Graph Explorer (recomendado), no Postman ou em qualquer outro cliente de API que você usa</span><span class="sxs-lookup"><span data-stu-id="fb657-129">Sign in to Microsoft Graph Explorer (recommended), Postman, or any other API client you use</span></span>

1. <span data-ttu-id="fb657-130">Iniciar [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="fb657-130">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
2. <span data-ttu-id="fb657-131">Selecione **Entrar com a Microsoft** e entre usando o administrador global do Azure AD ou as credenciais de Administrador do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb657-131">Select **Sign-in with Microsoft** and sign in using Azure AD global administrator or App Admin credentials.</span></span>
3. <span data-ttu-id="fb657-132">Após entrar com êxito, você verá os detalhes da conta de usuário no painel esquerdo.</span><span class="sxs-lookup"><span data-stu-id="fb657-132">Upon successful sign in, you'll see the user account details in the left pane.</span></span>

> [!NOTE]
> <span data-ttu-id="fb657-133">Não há suporte para entrar usando uma entidade de serviço no momento.</span><span class="sxs-lookup"><span data-stu-id="fb657-133">Sign in using a service principal is not currently supported.</span></span> 

### <a name="create-an-application"></a><span data-ttu-id="fb657-134">Criar um aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb657-134">Create an application</span></span>

<span data-ttu-id="fb657-135">Para configurar o Proxy de Aplicativo para um aplicativo usando a API, crie um aplicativo, adicione uma entidade de serviço ao aplicativo e atualize a propriedade **onPremisesPublishing** do aplicativo para definir as configurações do Proxy de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb657-135">To configure Application Proxy for an app using the API, you create an application, add a service principal to the app, and then update the application's **onPremisesPublishing** property to configure the App Proxy settings.</span></span> <span data-ttu-id="fb657-136">Ao criar o aplicativo, de definida **signInAudience** do aplicativo como "AzureADMyOrg".</span><span class="sxs-lookup"><span data-stu-id="fb657-136">When creating the application, set the application's **signInAudience** to "AzureADMyOrg".</span></span>

#### <a name="request"></a><span data-ttu-id="fb657-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb657-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fb657-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb657-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="fb657-139">C#</span><span class="sxs-lookup"><span data-stu-id="fb657-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb657-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb657-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb657-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb657-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fb657-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb657-142">Response</span></span>

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

### <a name="retrieve-the-application-object-id-and-appid"></a><span data-ttu-id="fb657-143">Recuperar a ID do objeto do aplicativo e appId</span><span class="sxs-lookup"><span data-stu-id="fb657-143">Retrieve the application object ID and appId</span></span>
<span data-ttu-id="fb657-144">Use a resposta da chamada anterior para recuperar e salvar a ID do objeto do aplicativo e a ID do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb657-144">Use the response from the previous call to retrieve and save the application object ID and app ID.</span></span>
```
"application": {
  "id": "bf21f7e9-9d25-4da2-82ab-7fdd85049f83",
  "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b"
}
```
### <a name="create-a-serviceprincipal-for-the-application-and-add-required-tags"></a><span data-ttu-id="fb657-145">Criar um servicePrincipal para o aplicativo e adicionar as marcas necessárias</span><span class="sxs-lookup"><span data-stu-id="fb657-145">Create a servicePrincipal for the application and add required tags</span></span>
<span data-ttu-id="fb657-146">Use a **appId** para criar uma entidade de serviço para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb657-146">Use the **appId** to create a service principal for the application.</span></span> <span data-ttu-id="fb657-147">Em seguida, adicione as marcas necessárias para configurar o Proxy de Aplicativo para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb657-147">Then add the tags required for configuring Application Proxy for an app.</span></span>

#### <a name="request"></a><span data-ttu-id="fb657-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb657-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fb657-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb657-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="fb657-150">C#</span><span class="sxs-lookup"><span data-stu-id="fb657-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb657-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb657-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb657-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb657-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fb657-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb657-153">Response</span></span>
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

## <a name="step-2-configure-application-proxy-properties"></a><span data-ttu-id="fb657-154">Etapa 2: Configurar propriedades do Proxy de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb657-154">Step 2: Configure Application Proxy properties</span></span>

### <a name="set-the-onpremisespublishing-configuration"></a><span data-ttu-id="fb657-155">Definir a configuração onPremisesPublishing</span><span class="sxs-lookup"><span data-stu-id="fb657-155">Set the onPremisesPublishing configuration</span></span>

<span data-ttu-id="fb657-156">Use a ID de objeto do aplicativo da etapa anterior para configurar o Proxy de Aplicativo para o aplicativo e atualizar a propriedade **onPremisesPublishing** para a configuração desejada.</span><span class="sxs-lookup"><span data-stu-id="fb657-156">Use the application object ID from the previous step to configure Application Proxy for the app and update the **onPremisesPublishing** property to the desired configuration.</span></span> <span data-ttu-id="fb657-157">Neste exemplo, você está usando um aplicativo com a URL interna: e usando o domínio padrão `https://contosoiwaapp.com` para a URL externa: `https://contosoiwaapp-contoso.msappproxy.net` .</span><span class="sxs-lookup"><span data-stu-id="fb657-157">In this example, you're using an app with the internal URL: `https://contosoiwaapp.com` and using the default domain for the external URL: `https://contosoiwaapp-contoso.msappproxy.net`.</span></span> 

#### <a name="request"></a><span data-ttu-id="fb657-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb657-158">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fb657-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb657-159">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="fb657-160">C#</span><span class="sxs-lookup"><span data-stu-id="fb657-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb657-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb657-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb657-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb657-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fb657-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb657-163">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```
### <a name="complete-the-configuration-of-the-application"></a><span data-ttu-id="fb657-164">Concluir a configuração do aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb657-164">Complete the configuration of the application</span></span>
<span data-ttu-id="fb657-165">Atualize as propriedades **redirectUri**, **identifierUri** e **homepageUrl** do aplicativo para a UR externa configurada na **propriedade onPremisesPublishing.**</span><span class="sxs-lookup"><span data-stu-id="fb657-165">Update the application's **redirectUri**, **identifierUri**, and **homepageUrl** properties to the external UR configured in the **onPremisesPublishing** property.</span></span> <span data-ttu-id="fb657-166">Em seguida, [atualize implicitGrantSettings](/graph/api/resources/implicitgrantsettings?view=graph-rest-1.0) para `true` **enabledTokenIssuance** e `false` **enabledAccessTokenIssuance**.</span><span class="sxs-lookup"><span data-stu-id="fb657-166">Then update [implicitGrantSettings](/graph/api/resources/implicitgrantsettings?view=graph-rest-1.0) to `true` for **enabledTokenIssuance** and `false` for **enabledAccessTokenIssuance**.</span></span>

#### <a name="request"></a><span data-ttu-id="fb657-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb657-167">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="fb657-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb657-168">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-3-assign-the-connector-group-to-the-application"></a><span data-ttu-id="fb657-169">Etapa 3: Atribuir o grupo de conectores ao aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb657-169">Step 3: Assign the connector group to the application</span></span>

### <a name="get-connectors"></a><span data-ttu-id="fb657-170">Obter conectores</span><span class="sxs-lookup"><span data-stu-id="fb657-170">Get connectors</span></span>

<span data-ttu-id="fb657-171">Liste os conectores e use a resposta para recuperar e salvar a ID do objeto do conector.</span><span class="sxs-lookup"><span data-stu-id="fb657-171">List the connectors and use the response to retrieve and save the connector object ID.</span></span> <span data-ttu-id="fb657-172">A ID do objeto do conector será usada para atribuir o conector a um grupo de conectores.</span><span class="sxs-lookup"><span data-stu-id="fb657-172">The connector object ID will be used to assign the connector to a connector group.</span></span>

#### <a name="request"></a><span data-ttu-id="fb657-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb657-173">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fb657-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb657-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "connector"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors

```
# <a name="c"></a>[<span data-ttu-id="fb657-175">C#</span><span class="sxs-lookup"><span data-stu-id="fb657-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb657-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb657-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb657-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb657-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fb657-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb657-178">Response</span></span>

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

### <a name="create-a-connectorgroup"></a><span data-ttu-id="fb657-179">Criar um connectorGroup</span><span class="sxs-lookup"><span data-stu-id="fb657-179">Create a connectorGroup</span></span>
<span data-ttu-id="fb657-180">Para este exemplo, um novo connectorGroup é criado chamado "IWA Demo Connector Group" que é usado para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb657-180">For this example, a new connectorGroup is created named "IWA Demo Connector Group" that is used for the application.</span></span> <span data-ttu-id="fb657-181">Você também pode ignorar esta etapa se o conector já estiver atribuído ao connectorGroup apropriado.</span><span class="sxs-lookup"><span data-stu-id="fb657-181">You can also skip this step if your connector is already assigned to the appropriate connectorGroup.</span></span> <span data-ttu-id="fb657-182">Recupere e salve a ID do objeto connectorGroup a ser usada na próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="fb657-182">Retrieve and save the connectorGroup object ID to use in the next step.</span></span>

#### <a name="request"></a><span data-ttu-id="fb657-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb657-183">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="fb657-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb657-184">Response</span></span>

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

### <a name="assign-a-connector-to-the-connectorgroup"></a><span data-ttu-id="fb657-185">Atribuir um conector ao connectorGroup</span><span class="sxs-lookup"><span data-stu-id="fb657-185">Assign a connector to the connectorGroup</span></span>

#### <a name="request"></a><span data-ttu-id="fb657-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb657-186">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="fb657-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb657-187">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

### <a name="assign-the-application-to-the-connectorgroup"></a><span data-ttu-id="fb657-188">Atribuir o aplicativo ao connectorGroup</span><span class="sxs-lookup"><span data-stu-id="fb657-188">Assign the application to the connectorGroup</span></span>

#### <a name="request"></a><span data-ttu-id="fb657-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb657-189">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fb657-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb657-190">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="fb657-191">C#</span><span class="sxs-lookup"><span data-stu-id="fb657-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb657-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb657-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb657-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb657-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fb657-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb657-194">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-4-configure-single-sign-on"></a><span data-ttu-id="fb657-195">Etapa 4: Configurar o single sign-on</span><span class="sxs-lookup"><span data-stu-id="fb657-195">Step 4: Configure single sign-on</span></span>
<span data-ttu-id="fb657-196">Esse aplicativo usa a Autenticação Integrada do Windows (IWA).</span><span class="sxs-lookup"><span data-stu-id="fb657-196">This application uses Integrated Windows Authentication (IWA).</span></span> <span data-ttu-id="fb657-197">Para configurar o IWA, de definidas as propriedades de login único no tipo de recurso [singleSignOnSettings.](/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="fb657-197">To configure IWA, set the single sign-on properties in the [singleSignOnSettings](/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta) resource type.</span></span>

#### <a name="request"></a><span data-ttu-id="fb657-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb657-198">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="fb657-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb657-199">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-5-assign-users"></a><span data-ttu-id="fb657-200">Etapa 5. Atribuir usuários</span><span class="sxs-lookup"><span data-stu-id="fb657-200">Step 5: Assign users</span></span>
### <a name="retrieve-approle-for-the-applicaiton"></a><span data-ttu-id="fb657-201">Recuperar appRole para o aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb657-201">Retrieve appRole for the applicaiton</span></span>

#### <a name="request"></a><span data-ttu-id="fb657-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb657-202">Request</span></span>



# <a name="http"></a>[<span data-ttu-id="fb657-203">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb657-203">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/a8cac399-cde5-4516-a674-819503c61313/appRoles
```
# <a name="c"></a>[<span data-ttu-id="fb657-204">C#</span><span class="sxs-lookup"><span data-stu-id="fb657-204">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb657-205">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb657-205">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb657-206">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb657-206">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fb657-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb657-207">Response</span></span>

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

<span data-ttu-id="fb657-208">Use a resposta da chamada anterior para recuperar e salvar a ID do appRole a ser usada na próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="fb657-208">Use the response from the previous call to retrieve and save the appRole ID to use for the next step.</span></span>
```
      {
            "description": "User",
            "displayName": "User",
            "id": "18d14569-c3bd-439b-9a66-3a2aee01d14f"
        }
```

### <a name="assign-users-and-groups-to-the-application"></a><span data-ttu-id="fb657-209">Atribuir usuários e grupos ao aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb657-209">Assign users and groups to the application</span></span>

<span data-ttu-id="fb657-210">Use as propriedades a seguir para atribuir um usuário ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb657-210">Use the following properties to assign a user to the application.</span></span>

| <span data-ttu-id="fb657-211">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb657-211">Property</span></span>  | <span data-ttu-id="fb657-212">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb657-212">Description</span></span> |<span data-ttu-id="fb657-213">ID</span><span class="sxs-lookup"><span data-stu-id="fb657-213">ID</span></span>  |
|---------|---------|---------|
| <span data-ttu-id="fb657-214">principalId</span><span class="sxs-lookup"><span data-stu-id="fb657-214">principalId</span></span> | <span data-ttu-id="fb657-215">ID de usuário do usuário que será atribuído ao aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb657-215">User ID of the user that will be assigned to the app</span></span> | <span data-ttu-id="fb657-216">2fe96d23-5dc6-4f35-8222-0426a8c115c8</span><span class="sxs-lookup"><span data-stu-id="fb657-216">2fe96d23-5dc6-4f35-8222-0426a8c115c8</span></span> |
| <span data-ttu-id="fb657-217">principalType</span><span class="sxs-lookup"><span data-stu-id="fb657-217">principalType</span></span> | <span data-ttu-id="fb657-218">Tipo de usuário</span><span class="sxs-lookup"><span data-stu-id="fb657-218">Type of user</span></span> | <span data-ttu-id="fb657-219">Usuário</span><span class="sxs-lookup"><span data-stu-id="fb657-219">User</span></span> |
| <span data-ttu-id="fb657-220">appRoleId</span><span class="sxs-lookup"><span data-stu-id="fb657-220">appRoleId</span></span> |  <span data-ttu-id="fb657-221">A ID da função de aplicativo da função de aplicativo padrão do aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb657-221">The App role ID of the default app role of the app</span></span> | <span data-ttu-id="fb657-222">18d14569-c3bd-439b-9a66-3a2aee01d14f</span><span class="sxs-lookup"><span data-stu-id="fb657-222">18d14569-c3bd-439b-9a66-3a2aee01d14f</span></span> |
| <span data-ttu-id="fb657-223">resourceId</span><span class="sxs-lookup"><span data-stu-id="fb657-223">resourceId</span></span> | <span data-ttu-id="fb657-224">A ID do servicePrincipal do aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb657-224">The servicePrincipal ID of the app</span></span> | <span data-ttu-id="fb657-225">a8cac399-cde5-4516-a674-819503c61313</span><span class="sxs-lookup"><span data-stu-id="fb657-225">a8cac399-cde5-4516-a674-819503c61313</span></span> |

#### <a name="request"></a><span data-ttu-id="fb657-226">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb657-226">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="fb657-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb657-227">Response</span></span>

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

<span data-ttu-id="fb657-228">Para saber mais, confira o tipo de recurso [appRoleAssignment](/graph/api/resources/approleassignment?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="fb657-228">For more information, see [appRoleAssignment](/graph/api/resources/approleassignment?view=graph-rest-beta) resource type.</span></span>


## <a name="additional-steps"></a><span data-ttu-id="fb657-229">Etapas adicionais</span><span class="sxs-lookup"><span data-stu-id="fb657-229">Additional steps</span></span>
- [<span data-ttu-id="fb657-230">Automatizar a configuração usando exemplos do PowerShell para o Proxy de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb657-230">Automate configuration using PowerShell samples for Application Proxy</span></span>](/azure/active-directory/manage-apps/application-proxy-powershell-samples.md)
- [<span data-ttu-id="fb657-231">Automação da configuração do aplicativo de SSO baseado em SAML com a API do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="fb657-231">Automate SAML-based SSO app configuration with Microsoft Graph API</span></span>](/azure/active-directory/manage-apps/application-saml-sso-configure-api.md)
