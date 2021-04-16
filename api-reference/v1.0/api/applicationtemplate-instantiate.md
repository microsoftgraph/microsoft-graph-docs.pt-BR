---
title: 'applicationTemplate: instaurá-lo'
description: Adicione uma instância de um aplicativo da galeria de aplicativos do Azure AD ao diretório.
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 34fe3ae80b34497cfe3313031cd1d3e2f5f7a91c
ms.sourcegitcommit: be09568fa07ab793cd1db500f537ca94ca9e5b4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836958"
---
# <a name="applicationtemplate-instantiate"></a><span data-ttu-id="58b55-103">applicationTemplate: instaurá-lo</span><span class="sxs-lookup"><span data-stu-id="58b55-103">applicationTemplate: instantiate</span></span>

<span data-ttu-id="58b55-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58b55-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="58b55-105">Adicione uma instância de um aplicativo da galeria de aplicativos do Azure AD ao diretório.</span><span class="sxs-lookup"><span data-stu-id="58b55-105">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="58b55-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="58b55-106">Permissions</span></span>

<span data-ttu-id="58b55-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58b55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="58b55-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58b55-109">Permission type</span></span>                        | <span data-ttu-id="58b55-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="58b55-110">Permissions (from least to most privileged)</span></span>        |
| :------------------------------------- | :------------------------------------------------- |
| <span data-ttu-id="58b55-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58b55-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="58b55-112">Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58b55-112">Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="58b55-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58b55-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58b55-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58b55-114">Not supported.</span></span>                                     |
| <span data-ttu-id="58b55-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58b55-115">Application</span></span>                            | <span data-ttu-id="58b55-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58b55-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="58b55-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58b55-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{id}/instantiate
```

## <a name="request-headers"></a><span data-ttu-id="58b55-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58b55-118">Request headers</span></span>

| <span data-ttu-id="58b55-119">Nome</span><span class="sxs-lookup"><span data-stu-id="58b55-119">Name</span></span>          | <span data-ttu-id="58b55-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="58b55-120">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="58b55-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="58b55-121">Authorization</span></span> | <span data-ttu-id="58b55-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="58b55-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="58b55-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58b55-123">Request body</span></span>

<span data-ttu-id="58b55-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58b55-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="58b55-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="58b55-125">Parameter</span></span>   | <span data-ttu-id="58b55-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="58b55-126">Type</span></span>   | <span data-ttu-id="58b55-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="58b55-127">Description</span></span>                    |
| :---------- | :----- | :----------------------------- |
| <span data-ttu-id="58b55-128">displayName</span><span class="sxs-lookup"><span data-stu-id="58b55-128">displayName</span></span> | <span data-ttu-id="58b55-129">String</span><span class="sxs-lookup"><span data-stu-id="58b55-129">String</span></span> | <span data-ttu-id="58b55-130">Nome personalizado do aplicativo</span><span class="sxs-lookup"><span data-stu-id="58b55-130">Custom name of the application</span></span> |

## <a name="response"></a><span data-ttu-id="58b55-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="58b55-131">Response</span></span>

<span data-ttu-id="58b55-132">Se tiver êxito, este método retornará um código de resposta e um `201 OK` novo [objeto applicationServicePrincipal](../resources/applicationserviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58b55-132">If successful, this method returns a `201 OK` response code and a new [applicationServicePrincipal](../resources/applicationserviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="58b55-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="58b55-133">Examples</span></span>

<span data-ttu-id="58b55-134">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="58b55-134">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="58b55-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58b55-135">Request</span></span>

<span data-ttu-id="58b55-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="58b55-136">The following is an example of the request.</span></span>

> <span data-ttu-id="58b55-137">Você pode usar essa API para insinuar [aplicativos que não são da galeria.](/azure/active-directory/manage-apps/add-non-gallery-app)</span><span class="sxs-lookup"><span data-stu-id="58b55-137">You can use this API to instantiate [non-gallery apps](/azure/active-directory/manage-apps/add-non-gallery-app).</span></span> <span data-ttu-id="58b55-138">Use a ID a seguir para **applicationTemplate**: `8adf8e6e-67b2-4cf2-a259-e3dc5476c621` .</span><span class="sxs-lookup"><span data-stu-id="58b55-138">Use the following ID for **applicationTemplate**: `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span></span>


# <a name="http"></a>[<span data-ttu-id="58b55-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="58b55-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "applicationtemplate_instantiate"
}-->

```http
POST https://graph.microsoft.com/v1.0/applicationTemplates/{id}/instantiate
Content-type: application/json

{
  "displayName": "My custom name"
}
```
# <a name="c"></a>[<span data-ttu-id="58b55-140">C#</span><span class="sxs-lookup"><span data-stu-id="58b55-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="58b55-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58b55-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="58b55-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58b55-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="58b55-143">Java</span><span class="sxs-lookup"><span data-stu-id="58b55-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/applicationtemplate-instantiate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="58b55-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="58b55-144">Response</span></span>

<span data-ttu-id="58b55-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="58b55-145">The following is an example of the response.</span></span>

> <span data-ttu-id="58b55-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="58b55-146">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationServicePrincipal"
} -->

```http
HTTP/1.1 201 OK
Content-type: application/json

{
   "servicePrincipal":{
      "accountEnabled":true,
      "addIns":[],
      "alternativeNames":[
         "http://contoso/a7770d29-4321-41a6-b863-ca11d6639448"
      ],
      "appDisplayName":"appDisplayName-value",
      "appId":"appId-value",
      "appOwnerOrganizationId":"appOwnerOrganizationId-value",
      "appRoleAssignmentRequired":true,
      "appRoles":[],
      "displayName":"Display name",
      "endpoints":[],
      "homepage":null,
      "id":"id-value",
      "info":{
         "termsOfServiceUrl":null,
         "supportUrl":null,
         "privacyStatementUrl":null,
         "marketingUrl":null,
         "logoUrl":null
      },
      "keyCredentials":[],
      "logoutUrl":null,
      "oauth2PermissionScopes":[],
      "passwordCredentials":[],
      "publisherName":null,
      "replyUrls":[],
      "servicePrincipalNames":[],
      "servicePrincipalType":null,
      "tags":[],
      "tokenEncryptionKeyId":null
   },
   "application":{
      "id":"id-value",
      "isFallbackPublicClient":null,
      "appId":"appId-value",
      "applicationTemplateId":null,
      "identifierUris":[],
      "createdDateTime":"2019-09-17T19:10:35.2742618Z",
      "displayName":"Display name",
      "isDeviceOnlyAuthSupported":null,
      "groupMembershipClaims":null,
      "optionalClaims":null,
      "addIns":[],
      "publisherDomain":"contoso.onmicrosoft.com",
      "signInAudience":"AzureADMyOrg",
      "tags":[],
      "tokenEncryptionKeyId":null,
      "api":{
         "requestedAccessTokenVersion":2,
         "acceptMappedClaims":null,
         "knownClientApplications":[],
         "oauth2PermissionScopes":[],
         "preAuthorizedApplications":[]
      },
      "appRoles":[],
      "publicClient":{
         "redirectUris":[]
      },
      "info":{
         "termsOfServiceUrl":null,
         "supportUrl":null,
         "privacyStatementUrl":null,
         "marketingUrl":null,
         "logoUrl":null
      },
      "keyCredentials":[],
      "parentalControlSettings":{
         "countriesBlockedForMinors":[],
         "legalAgeGroupRule":"Allow"
      },
      "passwordCredentials":[],
      "requiredResourceAccess":[ ],
      "web":{
         "redirectUris":[],
         "homePageUrl":null,
         "logoutUrl":null,
         "implicitGrantSettings":{
            "enableIdTokenIssuance":false,
            "enableAccessTokenIssuance":false
         }
      }
   }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationTemplate: instantiate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
