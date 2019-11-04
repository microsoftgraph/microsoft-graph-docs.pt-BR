---
title: Obter aplicativo
description: Obtenha as propriedades e os relacionamentos de um objeto application
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b515fb45ad0329059a85102d42243b3e6fa7c202
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37934309"
---
# <a name="get-application"></a><span data-ttu-id="20959-103">Obter aplicativo</span><span class="sxs-lookup"><span data-stu-id="20959-103">Get application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20959-104">Obtenha as propriedades e os relacionamentos de um objeto [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="20959-104">Get the properties and relationships of a [group](../resources/application.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="20959-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="20959-105">Permissions</span></span>
<span data-ttu-id="20959-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20959-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20959-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20959-108">Permission type</span></span>      | <span data-ttu-id="20959-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20959-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20959-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20959-110">Delegated (work or school account)</span></span> | <span data-ttu-id="20959-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="20959-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="20959-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20959-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20959-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20959-113">Not supported.</span></span>    |
|<span data-ttu-id="20959-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20959-114">Application</span></span> | <span data-ttu-id="20959-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="20959-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20959-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20959-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="20959-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="20959-117">Optional query parameters</span></span>
<span data-ttu-id="20959-118">Este método dá suporte a [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="20959-118">This method supports the OData Query Parameters to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="20959-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20959-119">Request headers</span></span>
| <span data-ttu-id="20959-120">Nome</span><span class="sxs-lookup"><span data-stu-id="20959-120">Name</span></span>       | <span data-ttu-id="20959-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="20959-121">Type</span></span> | <span data-ttu-id="20959-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="20959-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="20959-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="20959-123">Authorization</span></span>  | <span data-ttu-id="20959-124">string</span><span class="sxs-lookup"><span data-stu-id="20959-124">string</span></span>  | <span data-ttu-id="20959-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20959-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="20959-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="20959-127">Content-type</span></span> | <span data-ttu-id="20959-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20959-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20959-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20959-130">Request body</span></span>
<span data-ttu-id="20959-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="20959-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20959-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="20959-132">Response</span></span>

<span data-ttu-id="20959-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [application](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20959-133">If successful, this method returns a `200 OK` response code and [application](../resources/application.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="20959-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="20959-134">Examples</span></span>
### <a name="request"></a><span data-ttu-id="20959-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20959-135">Request</span></span>
<span data-ttu-id="20959-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20959-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="20959-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="20959-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_application"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="20959-138">C#</span><span class="sxs-lookup"><span data-stu-id="20959-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="20959-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20959-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="20959-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20959-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="20959-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="20959-141">Response</span></span>
<span data-ttu-id="20959-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20959-142">Here is an example of the response.</span></span> 

><span data-ttu-id="20959-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20959-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#applications/$entity",
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
