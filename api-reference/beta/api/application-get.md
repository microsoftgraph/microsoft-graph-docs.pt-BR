---
title: Obter aplicativo
description: Obtenha as propriedades e os relacionamentos de um objeto application.
author: sureshja
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ea72329f42f3c15f6b522433ec82565543536949
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962157"
---
# <a name="get-application"></a><span data-ttu-id="2c6d4-103">Obter aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c6d4-103">Get application</span></span>

<span data-ttu-id="2c6d4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c6d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c6d4-105">Obtenha as propriedades e os relacionamentos de um objeto [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="2c6d4-105">Get the properties and relationships of an [application](../resources/application.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c6d4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2c6d4-106">Permissions</span></span>
<span data-ttu-id="2c6d4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c6d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c6d4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c6d4-109">Permission type</span></span>      | <span data-ttu-id="2c6d4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2c6d4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c6d4-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c6d4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2c6d4-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2c6d4-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2c6d4-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c6d4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c6d4-114">Application.Read.All, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c6d4-114">Application.Read.All, Application.ReadWrite.All</span></span>    |
|<span data-ttu-id="2c6d4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c6d4-115">Application</span></span> | <span data-ttu-id="2c6d4-116">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy,  Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c6d4-116">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy,  Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c6d4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c6d4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2c6d4-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2c6d4-118">Optional query parameters</span></span>
<span data-ttu-id="2c6d4-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2c6d4-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2c6d4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c6d4-120">Request headers</span></span>
| <span data-ttu-id="2c6d4-121">Nome</span><span class="sxs-lookup"><span data-stu-id="2c6d4-121">Name</span></span>           | <span data-ttu-id="2c6d4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c6d4-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="2c6d4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c6d4-123">Authorization</span></span>  | <span data-ttu-id="2c6d4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c6d4-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2c6d4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c6d4-126">Request body</span></span>
<span data-ttu-id="2c6d4-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2c6d4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c6d4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c6d4-128">Response</span></span>

<span data-ttu-id="2c6d4-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [application](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c6d4-129">If successful, this method returns a `200 OK` response code and an [application](../resources/application.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="2c6d4-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2c6d4-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="2c6d4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c6d4-131">Request</span></span>
<span data-ttu-id="2c6d4-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c6d4-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2c6d4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c6d4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_application"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}
```
# <a name="c"></a>[<span data-ttu-id="2c6d4-134">C#</span><span class="sxs-lookup"><span data-stu-id="2c6d4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c6d4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c6d4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c6d4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c6d4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c6d4-137">Java</span><span class="sxs-lookup"><span data-stu-id="2c6d4-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="2c6d4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c6d4-138">Response</span></span>
<span data-ttu-id="2c6d4-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c6d4-139">Here is an example of the response.</span></span> 

><span data-ttu-id="2c6d4-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2c6d4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


