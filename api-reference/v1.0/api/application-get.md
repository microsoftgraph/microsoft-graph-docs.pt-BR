---
title: Obter aplicativo
description: Obtenha as propriedades e os relacionamentos de um objeto application.
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d7bc7993ef5bc14e2d3879f25920441efa5d3727
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998999"
---
# <a name="get-application"></a><span data-ttu-id="178a9-103">Obter aplicativo</span><span class="sxs-lookup"><span data-stu-id="178a9-103">Get application</span></span>

<span data-ttu-id="178a9-104">Obtenha as propriedades e os relacionamentos de um objeto [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="178a9-104">Get the properties and relationships of an [application](../resources/application.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="178a9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="178a9-105">Permissions</span></span>
<span data-ttu-id="178a9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="178a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="178a9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="178a9-108">Permission type</span></span>      | <span data-ttu-id="178a9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="178a9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="178a9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="178a9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="178a9-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="178a9-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="178a9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="178a9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="178a9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="178a9-113">Not supported.</span></span>    |
|<span data-ttu-id="178a9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="178a9-114">Application</span></span> | <span data-ttu-id="178a9-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="178a9-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="178a9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="178a9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="178a9-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="178a9-117">Optional query parameters</span></span>
<span data-ttu-id="178a9-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="178a9-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="178a9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="178a9-119">Request headers</span></span>
| <span data-ttu-id="178a9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="178a9-120">Name</span></span>       | <span data-ttu-id="178a9-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="178a9-121">Type</span></span> | <span data-ttu-id="178a9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="178a9-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="178a9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="178a9-123">Authorization</span></span>  | <span data-ttu-id="178a9-124">string</span><span class="sxs-lookup"><span data-stu-id="178a9-124">string</span></span>  | <span data-ttu-id="178a9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="178a9-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="178a9-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="178a9-127">Content-type</span></span> | <span data-ttu-id="178a9-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="178a9-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="178a9-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="178a9-130">Request body</span></span>
<span data-ttu-id="178a9-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="178a9-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="178a9-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="178a9-132">Response</span></span>

<span data-ttu-id="178a9-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [application](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="178a9-133">If successful, this method returns a `200 OK` response code and an [application](../resources/application.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="178a9-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="178a9-134">Examples</span></span>
### <a name="request"></a><span data-ttu-id="178a9-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="178a9-135">Request</span></span>
<span data-ttu-id="178a9-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="178a9-136">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="178a9-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="178a9-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_application"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="178a9-138">C#</span><span class="sxs-lookup"><span data-stu-id="178a9-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="178a9-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="178a9-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="178a9-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="178a9-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="178a9-141">Java</span><span class="sxs-lookup"><span data-stu-id="178a9-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="178a9-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="178a9-142">Response</span></span>
<span data-ttu-id="178a9-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="178a9-143">Here is an example of the response.</span></span> 

><span data-ttu-id="178a9-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="178a9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1044

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#applications/$entity",
    "id": "03ef14b0-ca33-4840-8f4f-d6e91916010e",
    "deletedDateTime": null,
    "isFallbackPublicClient": null,
    "appId": "631a96bc-a705-4eda-9f99-fdaf9f54f6a2",
    "applicationTemplateId": null,
    "identifierUris": [],
    "createdDateTime": "2019-09-17T19:10:35.2742618Z",
    "displayName": "Display name",
    "isDeviceOnlyAuthSupported": null,
    "groupMembershipClaims": null,
    "optionalClaims": null,
    "addIns": [],
    "publisherDomain": "contoso.onmicrosoft.com",
    "signInAudience": "AzureADandPersonalMicrosoftAccount",
    "tags": [],
    "tokenEncryptionKeyId": null,
    "api": {
        "requestedAccessTokenVersion": 2,
        "acceptMappedClaims": null,
        "knownClientApplications": [],
        "oauth2PermissionScopes": [],
        "preAuthorizedApplications": []
    },
    "appRoles": [],
    "publicClient": {
        "redirectUris": []
    },
    "info": {
        "termsOfServiceUrl": null,
        "supportUrl": null,
        "privacyStatementUrl": null,
        "marketingUrl": null,
        "logoUrl": null
    },
    "keyCredentials": [],
    "parentalControlSettings": {
        "countriesBlockedForMinors": [],
        "legalAgeGroupRule": "Allow"
    },
    "passwordCredentials": [],
    "requiredResourceAccess": [],
    "web": {
        "redirectUris": [],
        "homePageUrl": null,
        "logoutUrl": null,
        "implicitGrantSettings": {
            "enableIdTokenIssuance": false,
            "enableAccessTokenIssuance": false
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
