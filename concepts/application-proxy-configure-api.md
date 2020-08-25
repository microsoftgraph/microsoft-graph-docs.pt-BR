---
title: Configurar o proxy de aplicativo usando as APIs do Microsoft Graph
description: Configure automaticamente o proxy de aplicativo usando as APIs do Microsoft Graph para fornecer acesso remoto e logon único para aplicativos locais.
author: davidmu1
ms.topic: conceptual
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cc99857905a0a308f49ddc41bf22da993ca8f1b4
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873101"
---
# <a name="automate-the-configuration-of-application-proxy-using-the-microsoft-graph-api"></a><span data-ttu-id="75a0e-103">Automatizar a configuração do proxy de aplicativo usando a API do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="75a0e-103">Automate the configuration of Application Proxy using the Microsoft Graph API</span></span>

<span data-ttu-id="75a0e-104">Neste artigo, você aprenderá a criar e configurar o [proxy de aplicativo](https://aka.ms/whyappproxy) do Azure Active Directory (Azure AD) para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="75a0e-104">In this article, you'll learn how to create and configure Azure Active Directory (Azure AD) [Application Proxy](https://aka.ms/whyappproxy) for an application.</span></span> <span data-ttu-id="75a0e-105">O proxy de aplicativo fornece acesso remoto seguro e logon único em aplicativos Web no local.</span><span class="sxs-lookup"><span data-stu-id="75a0e-105">Application Proxy provides secure remote access and single sign-on to on-premises web applications.</span></span> <span data-ttu-id="75a0e-106">Depois de configurar o proxy de aplicativo para um aplicativo, os usuários podem acessar seus aplicativos locais por meio de uma URL externa, do portal de meus aplicativos ou de outros portais de aplicativos internos.</span><span class="sxs-lookup"><span data-stu-id="75a0e-106">After configuring Application Proxy for an application, users can access their on-premises applications through an external URL, the My Apps portal, or other internal application portals.</span></span>

<span data-ttu-id="75a0e-107">Este artigo pressupõe que você já instalou um conector e concluiu os [pré-requisitos](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) para o proxy de aplicativo para que os conectores possam se comunicar com os serviços do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="75a0e-107">This article assumes you have already installed a connector and completed the [prerequisites](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) for Application Proxy so that connectors can communicate with Azure AD services.</span></span>

<span data-ttu-id="75a0e-108">Verifique se você tem as permissões correspondentes para chamar as seguintes APIs.</span><span class="sxs-lookup"><span data-stu-id="75a0e-108">Make sure you have the corresponding permissions to call the following APIs.</span></span>

|<span data-ttu-id="75a0e-109">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="75a0e-109">Resource type</span></span> |<span data-ttu-id="75a0e-110">Método</span><span class="sxs-lookup"><span data-stu-id="75a0e-110">Method</span></span> |
|---------|---------|
|[<span data-ttu-id="75a0e-111">aplicativos</span><span class="sxs-lookup"><span data-stu-id="75a0e-111">applications</span></span>](https://docs.microsoft.com/graph/api/resources/application?view=graph-rest-1.0)<br> [<span data-ttu-id="75a0e-112">onPremisesPublishing</span><span class="sxs-lookup"><span data-stu-id="75a0e-112">onPremisesPublishing</span></span>](https://docs.microsoft.com/graph/api/resources/onpremisespublishing?view=graph-rest-beta)| [<span data-ttu-id="75a0e-113">Criar aplicativo</span><span class="sxs-lookup"><span data-stu-id="75a0e-113">Create application</span></span>](https://docs.microsoft.com/graph/api/application-post-applications?view=graph-rest-beta&tabs=http) <br> [<span data-ttu-id="75a0e-114">Atualizar aplicativo</span><span class="sxs-lookup"><span data-stu-id="75a0e-114">Update application</span></span>](https://docs.microsoft.com/graph/api/application-update?view=graph-rest-beta)<br> [<span data-ttu-id="75a0e-115">Adicionar aplicativo ao um conector</span><span class="sxs-lookup"><span data-stu-id="75a0e-115">Add application to connectorGroup</span></span>](https://docs.microsoft.com/graph/api/connectorgroup-post-applications?view=graph-rest-beta)|
|[<span data-ttu-id="75a0e-116">conector</span><span class="sxs-lookup"><span data-stu-id="75a0e-116">connector</span></span>](https://docs.microsoft.com/graph/api/resources/connector?view=graph-rest-beta)| [<span data-ttu-id="75a0e-117">Obter conectores</span><span class="sxs-lookup"><span data-stu-id="75a0e-117">Get connectors</span></span>](https://docs.microsoft.com/graph/api/connector-get?view=graph-rest-beta)
|[<span data-ttu-id="75a0e-118">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="75a0e-118">connectorGroup</span></span>](https://docs.microsoft.com/graph/api/resources/connectorGroup?view=graph-rest-beta)| [<span data-ttu-id="75a0e-119">Criar connectorGroup</span><span class="sxs-lookup"><span data-stu-id="75a0e-119">Create connectorGroup</span></span>](https://docs.microsoft.com/graph/api/resources/connectorgroup?view=graph-rest-beta) <br> [<span data-ttu-id="75a0e-120">Adicionar conector a connectorGroup</span><span class="sxs-lookup"><span data-stu-id="75a0e-120">Add connector to connectorGroup</span></span>](https://docs.microsoft.com/graph/api/connector-post-memberof?view=graph-rest-beta) <br> |
|[<span data-ttu-id="75a0e-121">servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="75a0e-121">servicePrincipals</span></span>](https://docs.microsoft.com/graph/api/resources/serviceprincipal?view=graph-rest-1.0)|[<span data-ttu-id="75a0e-122">Criar servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="75a0e-122">Create servicePrincipal</span></span>](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals?view=graph-rest-beta&tabs=http) <br> [<span data-ttu-id="75a0e-123">Atualizar servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="75a0e-123">Update servicePrincipal</span></span>](https://docs.microsoft.com/graph/api/serviceprincipal-update?view=graph-rest-1.0&tabs=http) <br> [<span data-ttu-id="75a0e-124">Criar appRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="75a0e-124">Create appRoleAssignments</span></span>](https://docs.microsoft.com/graph/api/serviceprincipal-post-approleassignments?view=graph-rest-beta)|

> [!NOTE]
> <span data-ttu-id="75a0e-125">As solicitações mostradas neste artigo usam valores de amostra.</span><span class="sxs-lookup"><span data-stu-id="75a0e-125">The requests shown in this article use sample values.</span></span> <span data-ttu-id="75a0e-126">Você precisará atualizá-los.</span><span class="sxs-lookup"><span data-stu-id="75a0e-126">You will need update these.</span></span> <span data-ttu-id="75a0e-127">Os objetos Response mostrados também podem ser reduzidos para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="75a0e-127">The response objects shown might also be shortened for readability.</span></span> 

## <a name="step-1-create-an-application"></a><span data-ttu-id="75a0e-128">Etapa 1: criar um aplicativo</span><span class="sxs-lookup"><span data-stu-id="75a0e-128">Step 1: Create an application</span></span>

### <a name="sign-in-to-microsoft-graph-explorer-recommended-postman-or-any-other-api-client-you-use"></a><span data-ttu-id="75a0e-129">Entrar no Microsoft Graph Explorer (recomendado), no Postman ou em qualquer outro cliente de API que você usa</span><span class="sxs-lookup"><span data-stu-id="75a0e-129">Sign in to Microsoft Graph Explorer (recommended), Postman, or any other API client you use</span></span>

1. <span data-ttu-id="75a0e-130">Iniciar [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="75a0e-130">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
2. <span data-ttu-id="75a0e-131">Selecione **entrar com a Microsoft** e entre usando um administrador global do Azure ad ou credenciais de administrador de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="75a0e-131">Select **Sign-in with Microsoft** and sign in using an Azure AD global administrator or App Admin credentials.</span></span>
3. <span data-ttu-id="75a0e-132">Após entrar com êxito, você verá os detalhes da conta de usuário no painel esquerdo.</span><span class="sxs-lookup"><span data-stu-id="75a0e-132">Upon successful sign in, you'll see the user account details in the left pane.</span></span>

### <a name="create-an-application"></a><span data-ttu-id="75a0e-133">Criar um aplicativo</span><span class="sxs-lookup"><span data-stu-id="75a0e-133">Create an application</span></span>

<span data-ttu-id="75a0e-134">Para configurar o proxy de aplicativo para um aplicativo usando a API, você cria um aplicativo, adiciona uma entidade de serviço ao aplicativo e, em seguida, atualiza a propriedade **onPremisesPublishing** do aplicativo para definir as configurações de proxy de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="75a0e-134">To configure Application Proxy for an app using the API, you create an application, add a service principal to the app, and then update the application's **onPremisesPublishing** property to configure the App Proxy settings.</span></span> <span data-ttu-id="75a0e-135">Ao criar o aplicativo, defina o **signInAudience** do aplicativo como "AzureADMyOrg".</span><span class="sxs-lookup"><span data-stu-id="75a0e-135">When creating the application, set the application's **signInAudience** to "AzureADMyOrg".</span></span>

#### <a name="request"></a><span data-ttu-id="75a0e-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75a0e-136">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="75a0e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="75a0e-137">Response</span></span>

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

### <a name="retrieve-the-application-object-id-and-appid"></a><span data-ttu-id="75a0e-138">Recuperar a ID de objeto de aplicativo e appId</span><span class="sxs-lookup"><span data-stu-id="75a0e-138">Retrieve the application object ID and appId</span></span>
<span data-ttu-id="75a0e-139">Use a resposta da chamada anterior para recuperar e salvar a ID do objeto de aplicativo e a ID do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="75a0e-139">Use the response from the previous call to retrieve and save the application object ID and app ID.</span></span>
```
"application": {
  "id": "bf21f7e9-9d25-4da2-82ab-7fdd85049f83",
  "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b"
}
```
### <a name="create-a-serviceprincipal-for-the-application-and-add-required-tags"></a><span data-ttu-id="75a0e-140">Criar um servicePrincipalName para o aplicativo e adicionar marcas necessárias</span><span class="sxs-lookup"><span data-stu-id="75a0e-140">Create a servicePrincipal for the application and add required tags</span></span>
<span data-ttu-id="75a0e-141">Use a **AppID** para criar uma entidade de serviço para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="75a0e-141">Use the **appId** to create a service principal for the application.</span></span> <span data-ttu-id="75a0e-142">Em seguida, adicione as marcas necessárias para configurar o proxy de aplicativo para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="75a0e-142">Then add the tags required for configuring Application Proxy for an app.</span></span>

#### <a name="request"></a><span data-ttu-id="75a0e-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75a0e-143">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="75a0e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="75a0e-144">Response</span></span>
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

## <a name="step-2-configure-application-proxy-properties"></a><span data-ttu-id="75a0e-145">Etapa 2: configurar as propriedades do proxy de aplicativo</span><span class="sxs-lookup"><span data-stu-id="75a0e-145">Step 2: Configure Application Proxy properties</span></span>

### <a name="set-the-onpremisespublishing-configuration"></a><span data-ttu-id="75a0e-146">Definir a configuração do onPremisesPublishing</span><span class="sxs-lookup"><span data-stu-id="75a0e-146">Set the onPremisesPublishing configuration</span></span>

<span data-ttu-id="75a0e-147">Use a ID de objeto de aplicativo da etapa anterior para configurar o proxy de aplicativo para o aplicativo e atualizar a propriedade **onPremisesPublishing** para a configuração desejada.</span><span class="sxs-lookup"><span data-stu-id="75a0e-147">Use the application object ID from the previous step to configure Application Proxy for the app and update the **onPremisesPublishing** property to the desired configuration.</span></span> <span data-ttu-id="75a0e-148">Neste exemplo, você está usando um aplicativo com a URL interna: `https://contosoiwaapp.com` e usando o domínio padrão para a URL externa: `https://contosoiwaapp-contoso.msappproxy.net` .</span><span class="sxs-lookup"><span data-stu-id="75a0e-148">In this example, you're using an app with the internal URL: `https://contosoiwaapp.com` and using the default domain for the external URL: `https://contosoiwaapp-contoso.msappproxy.net`.</span></span> 

#### <a name="request"></a><span data-ttu-id="75a0e-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75a0e-149">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="75a0e-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="75a0e-150">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```
### <a name="complete-the-configuration-of-the-application"></a><span data-ttu-id="75a0e-151">Concluir a configuração do aplicativo</span><span class="sxs-lookup"><span data-stu-id="75a0e-151">Complete the configuration of the application</span></span>
<span data-ttu-id="75a0e-152">Atualize as propriedades **redirectUri**, **identifierUri**e **HOMEPAGEURL** do aplicativo para a ur externa configurada na propriedade **onPremisesPublishing** .</span><span class="sxs-lookup"><span data-stu-id="75a0e-152">Update the application's **redirectUri**, **identifierUri**, and **homepageUrl** properties to the external UR configured in the **onPremisesPublishing** property.</span></span> <span data-ttu-id="75a0e-153">Em seguida, atualize o [implicitGrantSettings](https://docs.microsoft.com/graph/api/resources/implicitgrantsettings?view=graph-rest-1.0) para o `true` **EnabledTokenIssuance** e `false` para o **enabledAccessTokenIssuance**.</span><span class="sxs-lookup"><span data-stu-id="75a0e-153">Then update [implicitGrantSettings](https://docs.microsoft.com/graph/api/resources/implicitgrantsettings?view=graph-rest-1.0) to `true` for **enabledTokenIssuance** and `false` for **enabledAccessTokenIssuance**.</span></span>

#### <a name="request"></a><span data-ttu-id="75a0e-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75a0e-154">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="75a0e-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="75a0e-155">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-3-assign-the-connector-group-to-the-application"></a><span data-ttu-id="75a0e-156">Etapa 3: atribuir o grupo de conectores ao aplicativo</span><span class="sxs-lookup"><span data-stu-id="75a0e-156">Step 3: Assign the connector group to the application</span></span>

### <a name="get-connectors"></a><span data-ttu-id="75a0e-157">Obter conectores</span><span class="sxs-lookup"><span data-stu-id="75a0e-157">Get connectors</span></span>

<span data-ttu-id="75a0e-158">Liste os conectores e use a resposta para recuperar e salvar a ID de objeto do conector.</span><span class="sxs-lookup"><span data-stu-id="75a0e-158">List the connectors and use the response to retrieve and save the connector object ID.</span></span> <span data-ttu-id="75a0e-159">A ID do objeto Connector será usada para atribuir o conector a um grupo de conectores.</span><span class="sxs-lookup"><span data-stu-id="75a0e-159">The connector object ID will be used to assign the connector to a connector group.</span></span>

#### <a name="request"></a><span data-ttu-id="75a0e-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75a0e-160">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "connector"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors

```

#### <a name="response"></a><span data-ttu-id="75a0e-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="75a0e-161">Response</span></span>

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

### <a name="create-a-connectorgroup"></a><span data-ttu-id="75a0e-162">Criar um um dos conectores</span><span class="sxs-lookup"><span data-stu-id="75a0e-162">Create a connectorGroup</span></span>
<span data-ttu-id="75a0e-163">Para este exemplo, um novo grupo de conectores é criado com o nome "grupo de conectores de demonstração do IWA" que é usado para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="75a0e-163">For this example, a new connectorGroup is created named "IWA Demo Connector Group" that is used for the application.</span></span> <span data-ttu-id="75a0e-164">Você também pode ignorar esta etapa se o seu conector já estiver atribuído ao conector apropriado.</span><span class="sxs-lookup"><span data-stu-id="75a0e-164">You can also skip this step if your connector is already assigned to the appropriate connectorGroup.</span></span> <span data-ttu-id="75a0e-165">Recupere e salve a ID de objeto do The Connector para usar na próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="75a0e-165">Retrieve and save the connectorGroup object ID to use in the next step.</span></span>

#### <a name="request"></a><span data-ttu-id="75a0e-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75a0e-166">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="75a0e-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="75a0e-167">Response</span></span>

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

### <a name="assign-a-connector-to-the-connectorgroup"></a><span data-ttu-id="75a0e-168">Atribuir um conector ao conector</span><span class="sxs-lookup"><span data-stu-id="75a0e-168">Assign a connector to the connectorGroup</span></span>

#### <a name="request"></a><span data-ttu-id="75a0e-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75a0e-169">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="75a0e-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="75a0e-170">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

### <a name="assign-the-application-to-the-connectorgroup"></a><span data-ttu-id="75a0e-171">Atribuir o aplicativo ao conector</span><span class="sxs-lookup"><span data-stu-id="75a0e-171">Assign the application to the connectorGroup</span></span>

#### <a name="request"></a><span data-ttu-id="75a0e-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75a0e-172">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="75a0e-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="75a0e-173">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-4-configure-single-sign-on"></a><span data-ttu-id="75a0e-174">Etapa 4: configurar o logon único</span><span class="sxs-lookup"><span data-stu-id="75a0e-174">Step 4: Configure single sign-on</span></span>
<span data-ttu-id="75a0e-175">Este aplicativo usa a autenticação integrada do Windows (IWA).</span><span class="sxs-lookup"><span data-stu-id="75a0e-175">This application uses Integrated Windows Authentication (IWA).</span></span> <span data-ttu-id="75a0e-176">Para configurar o IWA, defina as propriedades de logon único no tipo de recurso [singleSignOnSettings](https://docs.microsoft.com/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta) .</span><span class="sxs-lookup"><span data-stu-id="75a0e-176">To configure IWA, set the single sign-on properties in the [singleSignOnSettings](https://docs.microsoft.com/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta) resource type.</span></span>

#### <a name="request"></a><span data-ttu-id="75a0e-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75a0e-177">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="75a0e-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="75a0e-178">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-5-assign-users"></a><span data-ttu-id="75a0e-179">Etapa 5. Atribuir usuários</span><span class="sxs-lookup"><span data-stu-id="75a0e-179">Step 5: Assign users</span></span>
### <a name="retrieve-approle-for-the-applicaiton"></a><span data-ttu-id="75a0e-180">Recuperar appRole para o aplicativo</span><span class="sxs-lookup"><span data-stu-id="75a0e-180">Retrieve appRole for the applicaiton</span></span>

#### <a name="request"></a><span data-ttu-id="75a0e-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75a0e-181">Request</span></span>


<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/a8cac399-cde5-4516-a674-819503c61313/appRoles
```

#### <a name="response"></a><span data-ttu-id="75a0e-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="75a0e-182">Response</span></span>

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

<span data-ttu-id="75a0e-183">Use a resposta da chamada anterior para recuperar e salvar a ID de appRole a ser usada para a próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="75a0e-183">Use the response from the previous call to retrieve and save the appRole ID to use for the next step.</span></span>
```
      {
            "description": "User",
            "displayName": "User",
            "id": "18d14569-c3bd-439b-9a66-3a2aee01d14f"
        }
```

### <a name="assign-users-and-groups-to-the-application"></a><span data-ttu-id="75a0e-184">Atribuir usuários e grupos ao aplicativo</span><span class="sxs-lookup"><span data-stu-id="75a0e-184">Assign users and groups to the application</span></span>

<span data-ttu-id="75a0e-185">Use as propriedades a seguir para atribuir um usuário ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="75a0e-185">Use the following properties to assign a user to the application.</span></span>

| <span data-ttu-id="75a0e-186">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75a0e-186">Property</span></span>  | <span data-ttu-id="75a0e-187">Descrição</span><span class="sxs-lookup"><span data-stu-id="75a0e-187">Description</span></span> |<span data-ttu-id="75a0e-188">ID</span><span class="sxs-lookup"><span data-stu-id="75a0e-188">ID</span></span>  |
|---------|---------|---------|
| <span data-ttu-id="75a0e-189">principalId</span><span class="sxs-lookup"><span data-stu-id="75a0e-189">principalId</span></span> | <span data-ttu-id="75a0e-190">ID de usuário do usuário que será atribuído ao aplicativo</span><span class="sxs-lookup"><span data-stu-id="75a0e-190">User ID of the user that will be assigned to the app</span></span> | <span data-ttu-id="75a0e-191">2fe96d23-5dc6-4f35-8222-0426a8c115c8</span><span class="sxs-lookup"><span data-stu-id="75a0e-191">2fe96d23-5dc6-4f35-8222-0426a8c115c8</span></span> |
| <span data-ttu-id="75a0e-192">principalType</span><span class="sxs-lookup"><span data-stu-id="75a0e-192">principalType</span></span> | <span data-ttu-id="75a0e-193">Tipo de usuário</span><span class="sxs-lookup"><span data-stu-id="75a0e-193">Type of user</span></span> | <span data-ttu-id="75a0e-194">Usuário</span><span class="sxs-lookup"><span data-stu-id="75a0e-194">User</span></span> |
| <span data-ttu-id="75a0e-195">appRoleId</span><span class="sxs-lookup"><span data-stu-id="75a0e-195">appRoleId</span></span> |  <span data-ttu-id="75a0e-196">A ID de função de aplicativo da função de aplicativo padrão do aplicativo</span><span class="sxs-lookup"><span data-stu-id="75a0e-196">The App role ID of the default app role of the app</span></span> | <span data-ttu-id="75a0e-197">18d14569-c3bd-439b-9a66-3a2aee01d14f</span><span class="sxs-lookup"><span data-stu-id="75a0e-197">18d14569-c3bd-439b-9a66-3a2aee01d14f</span></span> |
| <span data-ttu-id="75a0e-198">resourceId</span><span class="sxs-lookup"><span data-stu-id="75a0e-198">resourceId</span></span> | <span data-ttu-id="75a0e-199">A ID de servicePrincipalName do aplicativo</span><span class="sxs-lookup"><span data-stu-id="75a0e-199">The servicePrincipal ID of the app</span></span> | <span data-ttu-id="75a0e-200">a8cac399-cde5-4516-a674-819503c61313</span><span class="sxs-lookup"><span data-stu-id="75a0e-200">a8cac399-cde5-4516-a674-819503c61313</span></span> |

#### <a name="request"></a><span data-ttu-id="75a0e-201">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75a0e-201">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="75a0e-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="75a0e-202">Response</span></span>

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

<span data-ttu-id="75a0e-203">Para saber mais, confira o tipo de recurso [appRoleAssignment](https://docs.microsoft.com/graph/api/resources/approleassignment?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="75a0e-203">For more information, see [appRoleAssignment](https://docs.microsoft.com/graph/api/resources/approleassignment?view=graph-rest-beta) resource type.</span></span>


## <a name="additional-steps"></a><span data-ttu-id="75a0e-204">Etapas adicionais</span><span class="sxs-lookup"><span data-stu-id="75a0e-204">Additional steps</span></span>
- [<span data-ttu-id="75a0e-205">Configuração automatizada usando exemplos do PowerShell para o proxy de aplicativo</span><span class="sxs-lookup"><span data-stu-id="75a0e-205">Automate configuration using PowerShell samples for Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-powershell-samples.md)
- [<span data-ttu-id="75a0e-206">Automação da configuração do aplicativo de SSO baseado em SAML com o Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="75a0e-206">Automate SAML-based SSO app configuration with Microsoft Graph API</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-saml-sso-configure-api.md)
