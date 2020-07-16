---
title: Configurar o proxy de aplicativo usando as APIs do Microsoft Graph
description: Configure automaticamente o proxy de aplicativo usando as APIs do Microsoft Graph para fornecer acesso remoto e logon único para aplicativos locais.
author: davidmu1
ms.topic: conceptual
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 065e7cdc84a353c4636fc4e7d13c32d22c7bce70
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142318"
---
# <a name="automate-the-configuration-of-application-proxy-using-the-microsoft-graph-api"></a><span data-ttu-id="7f9de-103">Automatizar a configuração do proxy de aplicativo usando a API do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7f9de-103">Automate the configuration of Application Proxy using the Microsoft Graph API</span></span>

<span data-ttu-id="7f9de-104">Neste artigo, você aprenderá a criar e configurar o [proxy de aplicativo](https://aka.ms/whyappproxy) do Azure Active Directory (Azure AD) para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7f9de-104">In this article, you'll learn how to create and configure Azure Active Directory (Azure AD) [Application Proxy](https://aka.ms/whyappproxy) for an application.</span></span> <span data-ttu-id="7f9de-105">O proxy de aplicativo fornece acesso remoto seguro e logon único em aplicativos Web no local.</span><span class="sxs-lookup"><span data-stu-id="7f9de-105">Application Proxy provides secure remote access and single sign-on to on-premises web applications.</span></span> <span data-ttu-id="7f9de-106">Depois de configurar o proxy de aplicativo para um aplicativo, os usuários podem acessar seus aplicativos locais por meio de uma URL externa, do portal de meus aplicativos ou de outros portais de aplicativos internos.</span><span class="sxs-lookup"><span data-stu-id="7f9de-106">After configuring Application Proxy for an application, users can access their on-premises applications through an external URL, the My Apps portal, or other internal application portals.</span></span>

<span data-ttu-id="7f9de-107">Este artigo pressupõe que você já instalou um conector e concluiu os [pré-requisitos](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) para o proxy de aplicativo para que os conectores possam se comunicar com os serviços do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7f9de-107">This article assumes you have already installed a connector and completed the [prerequisites](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) for Application Proxy so that connectors can communicate with Azure AD services.</span></span>

<span data-ttu-id="7f9de-108">Verifique se você tem as permissões correspondentes para chamar as seguintes APIs.</span><span class="sxs-lookup"><span data-stu-id="7f9de-108">Make sure you have the corresponding permissions to call the following APIs.</span></span>

|<span data-ttu-id="7f9de-109">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="7f9de-109">Resource type</span></span> |<span data-ttu-id="7f9de-110">Método</span><span class="sxs-lookup"><span data-stu-id="7f9de-110">Method</span></span> |
|---------|---------|
| [<span data-ttu-id="7f9de-111">applicationtemplate</span><span class="sxs-lookup"><span data-stu-id="7f9de-111">applicationTemplate</span></span>](https://docs.microsoft.com/graph/api/resources/applicationtemplate?view=graph-rest-beta)| [<span data-ttu-id="7f9de-112">Instanciar applicationtemplate</span><span class="sxs-lookup"><span data-stu-id="7f9de-112">Instantiate applicationTemplate</span></span>](https://docs.microsoft.com/graph/api/resources/applicationtemplate?view=graph-rest-beta) |
|[<span data-ttu-id="7f9de-113">Emprego</span><span class="sxs-lookup"><span data-stu-id="7f9de-113">applications</span></span>](https://docs.microsoft.com/graph/api/resources/application?view=graph-rest-1.0)<br> [<span data-ttu-id="7f9de-114">onPremisesPublishing</span><span class="sxs-lookup"><span data-stu-id="7f9de-114">onPremisesPublishing</span></span>](https://docs.microsoft.com/graph/api/resources/onpremisespublishing?view=graph-rest-beta)|[<span data-ttu-id="7f9de-115">Atualizar aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f9de-115">Update application</span></span>](https://docs.microsoft.com/graph/api/application-update?view=graph-rest-beta)<br> [<span data-ttu-id="7f9de-116">Adicionar aplicativo ao um conector</span><span class="sxs-lookup"><span data-stu-id="7f9de-116">Add application to connectorGroup</span></span>](https://docs.microsoft.com/graph/api/connectorgroup-post-applications?view=graph-rest-beta)|
|[<span data-ttu-id="7f9de-117">conector</span><span class="sxs-lookup"><span data-stu-id="7f9de-117">connector</span></span>](https://docs.microsoft.com/graph/api/resources/connector?view=graph-rest-beta)| [<span data-ttu-id="7f9de-118">Obter conectores</span><span class="sxs-lookup"><span data-stu-id="7f9de-118">Get connectors</span></span>](https://docs.microsoft.com/graph/api/connector-get?view=graph-rest-beta)
|[<span data-ttu-id="7f9de-119">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="7f9de-119">connectorGroup</span></span>](https://docs.microsoft.com/graph/api/resources/connectorGroup?view=graph-rest-beta)| [<span data-ttu-id="7f9de-120">Criar um conector</span><span class="sxs-lookup"><span data-stu-id="7f9de-120">Create connectorGroup</span></span>](https://docs.microsoft.com/graph/api/resources/connectorgroup?view=graph-rest-beta) <br> [<span data-ttu-id="7f9de-121">Adicionar conector ao conector</span><span class="sxs-lookup"><span data-stu-id="7f9de-121">Add connector to connectorGroup</span></span>](https://docs.microsoft.com/graph/api/connector-post-memberof?view=graph-rest-beta) <br> |
|[<span data-ttu-id="7f9de-122">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="7f9de-122">servicePrincipals</span></span>](https://docs.microsoft.com/graph/api/resources/serviceprincipal?view=graph-rest-1.0)|[<span data-ttu-id="7f9de-123">Atualizar o servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="7f9de-123">Update servicePrincipal</span></span>](https://docs.microsoft.com/graph/api/serviceprincipal-update?view=graph-rest-1.0&tabs=http) <br> [<span data-ttu-id="7f9de-124">Criar appRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="7f9de-124">Create appRoleAssignments</span></span>](https://docs.microsoft.com/graph/api/serviceprincipal-post-approleassignments?view=graph-rest-beta)|

>[!NOTE]
> <span data-ttu-id="7f9de-125">As solicitações mostradas neste artigo usam valores de amostra.</span><span class="sxs-lookup"><span data-stu-id="7f9de-125">The requests shown in this article uses sample values.</span></span> <span data-ttu-id="7f9de-126">Você precisará atualizá-los.</span><span class="sxs-lookup"><span data-stu-id="7f9de-126">You will need update these.</span></span> <span data-ttu-id="7f9de-127">Os objetos Response mostrados também podem ser reduzidos para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="7f9de-127">The response objects shown may also be shortened for readability.</span></span> <span data-ttu-id="7f9de-128">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f9de-128">All the properties will be returned from an actual call.</span></span>

## <a name="step-1-create-a-custom-application"></a><span data-ttu-id="7f9de-129">Etapa 1: criar um aplicativo personalizado</span><span class="sxs-lookup"><span data-stu-id="7f9de-129">Step 1: Create a custom application</span></span>

### <a name="sign-in-to-microsoft-graph-explorer-recommended-postman-or-any-other-api-client-you-use"></a><span data-ttu-id="7f9de-130">Entrar no Microsoft Graph Explorer (recomendado), postmaster ou qualquer outro cliente da API que você usa</span><span class="sxs-lookup"><span data-stu-id="7f9de-130">Sign in to Microsoft Graph Explorer (recommended), Postman, or any other API client you use</span></span>

1. <span data-ttu-id="7f9de-131">Inicie [o Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="7f9de-131">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
2. <span data-ttu-id="7f9de-132">Selecione **entrar com a Microsoft** e entre usando um administrador global do Azure ad ou credenciais de administrador de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="7f9de-132">Select **Sign-In with Microsoft** and sign in using an Azure AD global administrator or App Admin credentials.</span></span>
3. <span data-ttu-id="7f9de-133">Após entrar com êxito, você verá os detalhes da conta de usuário no painel esquerdo.</span><span class="sxs-lookup"><span data-stu-id="7f9de-133">Upon successful sign-in, you'll see the user account details in the left pane.</span></span>

### <a name="create-a-custom-application"></a><span data-ttu-id="7f9de-134">Criar um aplicativo personalizado</span><span class="sxs-lookup"><span data-stu-id="7f9de-134">Create a custom application</span></span>

<span data-ttu-id="7f9de-135">Para configurar o proxy de aplicativo para um aplicativo usando a API, você deve primeiro criar um aplicativo personalizado e, em seguida, atualizar a propriedade **onPremisesPublishing** do aplicativo para o aplicativo para definir as configurações de proxy de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7f9de-135">To configure Application Proxy for an app using the API, you must first create a custom application, then update the application's **onPremisesPublishing** property for the app to configure the App Proxy settings.</span></span>
<span data-ttu-id="7f9de-136">Use [instanciar applicationtemplate](https://docs.microsoft.com/graph/api/resources/applicationtemplate?view=graph-rest-beta) para criar uma instância de um aplicativo personalizado e uma entidade de serviço em seu locatário para gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="7f9de-136">Use [instantiate applicationTemplate](https://docs.microsoft.com/graph/api/resources/applicationtemplate?view=graph-rest-beta) to create an instance of a custom application and service principal in your tenant for management.</span></span> <span data-ttu-id="7f9de-137">A ID de modelo para um aplicativo personalizado é: `8adf8e6e-67b2-4cf2-a259-e3dc5476c621` .</span><span class="sxs-lookup"><span data-stu-id="7f9de-137">The template ID for a custom application is: `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span></span>

#### <a name="request"></a><span data-ttu-id="7f9de-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f9de-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7f9de-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f9de-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_applicationTemplate"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/applicationTemplates/8adf8e6e-67b2-4cf2-a259-e3dc5476c621/instantiate
Content-type: application/json

{
  "displayName": "Contoso IWA App"
}
```
# <a name="c"></a>[<span data-ttu-id="7f9de-140">C#</span><span class="sxs-lookup"><span data-stu-id="7f9de-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-applicationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f9de-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f9de-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-applicationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f9de-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f9de-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-applicationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="7f9de-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f9de-143">Response</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.applicationServicePrincipal",
    "application": {
        "objectId": "bf21f7e9-9d25-4da2-82ab-7fdd85049f83",
        "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b",
        "applicationTemplateId": "8adf8e6e-67b2-4cf2-a259-e3dc5476c621",
        "displayName": "Contoso IWA App",
        "homepage": "https://account.activedirectory.windowsazure.com:444/applications/default.aspx?metadata=customappsso|ISV9.1|primary|z",
        "identifierUris": [],
        "publicClient": null,
        "replyUrls": [],
        "logoutUrl": null,
        "samlMetadataUrl": null,
        "errorUrl": null,
        "groupMembershipClaims": null,
        "availableToOtherTenants": false
    },
    "servicePrincipal": {
        "objectId": "b00c693f-9658-4c06-bd1b-c402c4653dea",
        "deletionTimestamp": null,
        "accountEnabled": true,
        "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b",
        "appDisplayName": "Contoso API",
        "applicationTemplateId": "8adf8e6e-67b2-4cf2-a259-e3dc5476c621",
        "appRoleAssignmentRequired": true,
        "displayName": "Contoso API",
        "errorUrl": null,
        "logoutUrl": null,
        "homepage": "https://account.activedirectory.windowsazure.com:444/applications/default.aspx?metadata=customappsso|ISV9.1|primary|z",
        "samlMetadataUrl": null,
        "microsoftFirstParty": null,
        "publisherName": "f/128 Photography",
        "preferredTokenSigningKeyThumbprint": null,
        "replyUrls": [],
        "servicePrincipalNames": [
            "d7fbfe28-c60e-46d2-8335-841923950d3b"
        ],
        "tags": [
            "WindowsAzureActiveDirectoryIntegratedApp",
            "WindowsAzureActiveDirectoryCustomSingleSignOnApplication"
        ],
        "notificationEmailAddresses": [],
        "keyCredentials": [],
        "passwordCredentials": []
    }
}
```


### <a name="retrieve-app-object-id-and-service-principal-object-id"></a><span data-ttu-id="7f9de-144">Recuperar ID de objeto do aplicativo e ID de objeto da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="7f9de-144">Retrieve app object ID and service principal object ID</span></span>
<span data-ttu-id="7f9de-145">Use a resposta da chamada anterior para recuperar e salvar a ID de objeto de aplicativo e a ID de objeto de entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="7f9de-145">Use the response from the previous call to retrieve and save the application object ID and service principal object ID.</span></span>
```
"application": {
    "objectId": "bf21f7e9-9d25-4da2-82ab-7fdd85049f83"
    }
"servicePrincipal": {
    "objectId": "b00c693f-9658-4c06-bd1b-c402c4653dea"
    }
```

## <a name="step-2-configure-application-proxy-properties"></a><span data-ttu-id="7f9de-146">Etapa 2: configurar as propriedades do proxy de aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f9de-146">Step 2: Configure Application Proxy properties</span></span>

### <a name="set-the-onpremisespublishing-configuration"></a><span data-ttu-id="7f9de-147">Definir a configuração do onPremisesPublishing</span><span class="sxs-lookup"><span data-stu-id="7f9de-147">Set the onPremisesPublishing configuration</span></span>

<span data-ttu-id="7f9de-148">Use o applicationId da etapa anterior para configurar o proxy de aplicativo para o aplicativo e atualizar a propriedade **onPremisesPublishing** para a configuração desejada.</span><span class="sxs-lookup"><span data-stu-id="7f9de-148">Use the applicationId from the previous step to configure Application Proxy for the app and update the **onPremisesPublishing** property to the desired configuration.</span></span> <span data-ttu-id="7f9de-149">Neste exemplo, você está usando um aplicativo com a URL interna: `https://contosoiwaapp.com` e usando o domínio padrão para a URL externa: `https://contosoiwaapp-contoso.msappproxy.net` .</span><span class="sxs-lookup"><span data-stu-id="7f9de-149">In this example, you're using an app with the internal url: `https://contosoiwaapp.com` and using the default domain for the external url: `https://contosoiwaapp-contoso.msappproxy.net`.</span></span> 

#### <a name="request"></a><span data-ttu-id="7f9de-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f9de-150">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7f9de-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f9de-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7f9de-152">C#</span><span class="sxs-lookup"><span data-stu-id="7f9de-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f9de-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f9de-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f9de-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f9de-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7f9de-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f9de-155">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```
### <a name="set-the-redirecturi-identifieruri-and-homepageurl-properties"></a><span data-ttu-id="7f9de-156">Definir as propriedades redirectUri, identifierUri e homepageUrl</span><span class="sxs-lookup"><span data-stu-id="7f9de-156">Set the redirectUri, identifierUri, and homepageUrl properties</span></span>
<span data-ttu-id="7f9de-157">Atualize as propriedades **redirectUri**, **identifierUri**e **HOMEPAGEURL** do aplicativo para a URL externa.</span><span class="sxs-lookup"><span data-stu-id="7f9de-157">Update the application's **redirectUri**, **identifierUri**, and **homepageUrl** propertes to the external URL.</span></span>

#### <a name="request"></a><span data-ttu-id="7f9de-158">Solicitar</span><span class="sxs-lookup"><span data-stu-id="7f9de-158">Request</span></span>

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
      "homePageUrl": "https://contosoiwaapp-contoso.msappproxy.net"
   }
}
```
#### <a name="response"></a><span data-ttu-id="7f9de-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f9de-159">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-3-assign-the-connector-group-to-the-application"></a><span data-ttu-id="7f9de-160">Etapa 3: atribuir o grupo de conectores ao aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f9de-160">Step 3: Assign the connector group to the application</span></span>

### <a name="get-connectors"></a><span data-ttu-id="7f9de-161">Obter conectores</span><span class="sxs-lookup"><span data-stu-id="7f9de-161">Get connectors</span></span>

<span data-ttu-id="7f9de-162">Liste os conectores e use a resposta para recuperar e salvar a ID de objeto do conector.</span><span class="sxs-lookup"><span data-stu-id="7f9de-162">List the connectors and use the response to retrieve and save the connector object ID.</span></span> <span data-ttu-id="7f9de-163">A ID do objeto Connector será usada para atribuir o conector a um grupo de conectores.</span><span class="sxs-lookup"><span data-stu-id="7f9de-163">The connector object ID will be used to assign the connector to a connector group.</span></span>

#### <a name="request"></a><span data-ttu-id="7f9de-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f9de-164">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7f9de-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f9de-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "connector"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors

```
# <a name="c"></a>[<span data-ttu-id="7f9de-166">C#</span><span class="sxs-lookup"><span data-stu-id="7f9de-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f9de-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f9de-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f9de-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f9de-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7f9de-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f9de-169">Response</span></span>

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

### <a name="create-a-connectorgroup"></a><span data-ttu-id="7f9de-170">Criar um um dos conectores</span><span class="sxs-lookup"><span data-stu-id="7f9de-170">Create a connectorGroup</span></span>
<span data-ttu-id="7f9de-171">Para este exemplo, um novo grupo de conectores é criado com o nome "grupo de conectores de demonstração do IWA" que é usado para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7f9de-171">For this example, a new connectorGroup is created named "IWA Demo Connector Group" that is used for the application.</span></span> <span data-ttu-id="7f9de-172">Você também pode ignorar esta etapa se o seu conector já estiver atribuído ao conector apropriado.</span><span class="sxs-lookup"><span data-stu-id="7f9de-172">You can also skip this step if your connector is already assigned to the appropriate connectorGroup.</span></span> <span data-ttu-id="7f9de-173">Recupere e salve a ID de objeto do The Connector para usar na próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="7f9de-173">Retrieve and save the connectorGroup object ID to use in the next step.</span></span>

#### <a name="request"></a><span data-ttu-id="7f9de-174">Solicitar</span><span class="sxs-lookup"><span data-stu-id="7f9de-174">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="7f9de-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f9de-175">Response</span></span>

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

### <a name="assign-a-connector-to-the-connectorgroup"></a><span data-ttu-id="7f9de-176">Atribuir um conector ao conector</span><span class="sxs-lookup"><span data-stu-id="7f9de-176">Assign a connector to the connectorGroup</span></span>

#### <a name="request"></a><span data-ttu-id="7f9de-177">Solicitar</span><span class="sxs-lookup"><span data-stu-id="7f9de-177">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="7f9de-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f9de-178">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

### <a name="assign-the-application-to-the-connectorgroup"></a><span data-ttu-id="7f9de-179">Atribuir o aplicativo ao conector</span><span class="sxs-lookup"><span data-stu-id="7f9de-179">Assign the application to the connectorGroup</span></span>

#### <a name="request"></a><span data-ttu-id="7f9de-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f9de-180">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7f9de-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f9de-181">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7f9de-182">C#</span><span class="sxs-lookup"><span data-stu-id="7f9de-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f9de-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f9de-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f9de-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f9de-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7f9de-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f9de-185">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-4-configure-single-sign-on"></a><span data-ttu-id="7f9de-186">Etapa 4: configurar o logon único</span><span class="sxs-lookup"><span data-stu-id="7f9de-186">Step 4: Configure single sign-on</span></span>
<span data-ttu-id="7f9de-187">Este aplicativo usa a autenticação integrada do Windows (IWA).</span><span class="sxs-lookup"><span data-stu-id="7f9de-187">This application uses Integrated Windows Authentication (IWA).</span></span> <span data-ttu-id="7f9de-188">Para configurar o IWA, defina as propriedades de logon único no tipo de recurso [singleSignOnSettings](https://docs.microsoft.com/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta) .</span><span class="sxs-lookup"><span data-stu-id="7f9de-188">To configure IWA, set the single sign-on properties in the [singleSignOnSettings](https://docs.microsoft.com/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta) resource type.</span></span>


#### <a name="request"></a><span data-ttu-id="7f9de-189">Solicitar</span><span class="sxs-lookup"><span data-stu-id="7f9de-189">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="7f9de-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f9de-190">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-5-assign-users"></a><span data-ttu-id="7f9de-191">Etapa 5: atribuir usuários</span><span class="sxs-lookup"><span data-stu-id="7f9de-191">Step 5: Assign users</span></span>
### <a name="retrieve-approle-for-the-applicaiton"></a><span data-ttu-id="7f9de-192">Recuperar appRole para o aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f9de-192">Retrieve appRole for the applicaiton</span></span>

#### <a name="request"></a><span data-ttu-id="7f9de-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f9de-193">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7f9de-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f9de-194">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/b00c693f-9658-4c06-bd1b-c402c4653dea/appRoles
```
# <a name="c"></a>[<span data-ttu-id="7f9de-195">C#</span><span class="sxs-lookup"><span data-stu-id="7f9de-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f9de-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f9de-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f9de-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f9de-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7f9de-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f9de-198">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 200
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals('b00c693f-9658-4c06-bd1b-c402c4653dea')/appRoles",
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

<span data-ttu-id="7f9de-199">Use a resposta da chamada anterior para recuperar e salvar a ID de appRole a ser usada para a próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="7f9de-199">Use the response from the previous call to retrieve and save the appRole ID to use for the next step.</span></span>
```
      {
            "description": "User",
            "displayName": "User",
            "id": "18d14569-c3bd-439b-9a66-3a2aee01d14f"
        }
```

### <a name="assign-users-and-groups-to-the-application"></a><span data-ttu-id="7f9de-200">Atribuir usuários e grupos ao aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f9de-200">Assign users and groups to the application</span></span>

<span data-ttu-id="7f9de-201">Use as propriedades a seguir para atribuir um usuário ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7f9de-201">Use the following properties to assign a user to the application.</span></span>

| <span data-ttu-id="7f9de-202">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f9de-202">Property</span></span>  | <span data-ttu-id="7f9de-203">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f9de-203">Description</span></span> |<span data-ttu-id="7f9de-204">ID</span><span class="sxs-lookup"><span data-stu-id="7f9de-204">ID</span></span>  |
|---------|---------|---------|
| <span data-ttu-id="7f9de-205">principalId</span><span class="sxs-lookup"><span data-stu-id="7f9de-205">principalId</span></span> | <span data-ttu-id="7f9de-206">ID de usuário do usuário que será atribuído ao aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f9de-206">User ID of the user that will be assigned to the app</span></span> | <span data-ttu-id="7f9de-207">2fe96d23-5dc6-4f35-8222-0426a8c115c8</span><span class="sxs-lookup"><span data-stu-id="7f9de-207">2fe96d23-5dc6-4f35-8222-0426a8c115c8</span></span> |
| <span data-ttu-id="7f9de-208">principalType</span><span class="sxs-lookup"><span data-stu-id="7f9de-208">principalType</span></span> | <span data-ttu-id="7f9de-209">Tipo de usuário</span><span class="sxs-lookup"><span data-stu-id="7f9de-209">Type of user</span></span> | <span data-ttu-id="7f9de-210">Usuário</span><span class="sxs-lookup"><span data-stu-id="7f9de-210">User</span></span> |
| <span data-ttu-id="7f9de-211">appRoleId</span><span class="sxs-lookup"><span data-stu-id="7f9de-211">appRoleId</span></span> |  <span data-ttu-id="7f9de-212">A ID de função de aplicativo da função de aplicativo padrão do aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f9de-212">The App role ID of the default app role of the app</span></span> | <span data-ttu-id="7f9de-213">18d14569-c3bd-439b-9a66-3a2aee01d14f</span><span class="sxs-lookup"><span data-stu-id="7f9de-213">18d14569-c3bd-439b-9a66-3a2aee01d14f</span></span> |
| <span data-ttu-id="7f9de-214">resourceId</span><span class="sxs-lookup"><span data-stu-id="7f9de-214">resourceId</span></span> | <span data-ttu-id="7f9de-215">A ID de servicePrincipalName do aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f9de-215">The servicePrincipal ID of the app</span></span> | <span data-ttu-id="7f9de-216">b00c693f-9658-4c06-bd1b-c402c4653dea</span><span class="sxs-lookup"><span data-stu-id="7f9de-216">b00c693f-9658-4c06-bd1b-c402c4653dea</span></span> |

#### <a name="request"></a><span data-ttu-id="7f9de-217">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f9de-217">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/servicePrincipals/b00c693f-9658-4c06-bd1b-c402c4653dea/appRoleAssignments

Content-type: appRoleAssignments/json

{
  "principalId": "2fe96d23-5dc6-4f35-8222-0426a8c115c8",
  "principalType": "User",
  "appRoleId":"18d14569-c3bd-439b-9a66-3a2aee01d14f",
  "resourceId":"b00c693f-9658-4c06-bd1b-c402c4653dea"
}
```
#### <a name="response"></a><span data-ttu-id="7f9de-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f9de-218">Response</span></span>

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
    "resourceId": "b00c693f-9658-4c06-bd1b-c402c4653dea"
}
```

<span data-ttu-id="7f9de-219">Para obter mais informações, consulte tipo de recurso [appRoleAssignment](https://docs.microsoft.com/graph/api/resources/approleassignment?view=graph-rest-beta) .</span><span class="sxs-lookup"><span data-stu-id="7f9de-219">For more information, see [appRoleAssignment](https://docs.microsoft.com/graph/api/resources/approleassignment?view=graph-rest-beta) resource type.</span></span>



## <a name="additional-steps"></a><span data-ttu-id="7f9de-220">Etapas adicionais</span><span class="sxs-lookup"><span data-stu-id="7f9de-220">Additional steps</span></span>
- [<span data-ttu-id="7f9de-221">Configuração automatizada usando exemplos do PowerShell para o proxy de aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f9de-221">Automate configuration using PowerShell samples for Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-powershell-samples.md)
- [<span data-ttu-id="7f9de-222">Automatizar a configuração do aplicativo SSO baseado em SAML com a API do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7f9de-222">Automate SAML-based SSO app configuration with Microsoft Graph API</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-saml-sso-configure-api.md)
