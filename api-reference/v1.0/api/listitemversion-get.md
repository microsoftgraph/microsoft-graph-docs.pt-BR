---
title: Obter um recurso ListItemVersion
description: Recuperar os metadados de uma versão específica de um ListItem.
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: apiPageType
ms.openlocfilehash: 4a7e10787b23ab422a64a30db7d0d921edfdfbcf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511674"
---
# <a name="get-a-listitemversion-resource"></a><span data-ttu-id="7db98-103">Obter um recurso ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="7db98-103">Get a ListItemVersion resource</span></span>

<span data-ttu-id="7db98-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7db98-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7db98-105">Recuperar os metadados de uma versão específica de um [ListItem](../resources/listitem.md).</span><span class="sxs-lookup"><span data-stu-id="7db98-105">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7db98-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7db98-106">Permissions</span></span>

<span data-ttu-id="7db98-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7db98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="7db98-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7db98-109">Permission type</span></span>             | <span data-ttu-id="7db98-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7db98-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="7db98-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7db98-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7db98-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7db98-112">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="7db98-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7db98-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7db98-114">n/d</span><span class="sxs-lookup"><span data-stu-id="7db98-114">n/a</span></span>                                         |
| <span data-ttu-id="7db98-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7db98-115">Application</span></span>                            | <span data-ttu-id="7db98-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7db98-116">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="7db98-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7db98-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="7db98-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="7db98-118">Response</span></span>

<span data-ttu-id="7db98-119">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ListItemVersion](../resources/listitemversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7db98-119">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="7db98-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7db98-120">Example</span></span>

<span data-ttu-id="7db98-121">Este exemplo recupera uma versão de um item de lista e expande o conjunto de campos para solicitar os valores dos campos no listItem.</span><span class="sxs-lookup"><span data-stu-id="7db98-121">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="7db98-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7db98-122">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="7db98-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="7db98-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read sites.read.all", "tags": "service.graph service.sharepoint" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}?expand=fields
```
# <a name="c"></a>[<span data-ttu-id="7db98-124">C#</span><span class="sxs-lookup"><span data-stu-id="7db98-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-single-version-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7db98-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7db98-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-single-version-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7db98-126">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7db98-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-single-version-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7db98-127">Java</span><span class="sxs-lookup"><span data-stu-id="7db98-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-single-version-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7db98-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7db98-128">Response</span></span>

<span data-ttu-id="7db98-129">Isso retornará uma coleção de versões:</span><span class="sxs-lookup"><span data-stu-id="7db98-129">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "1.0",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "fields": {  }
}
```

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
  ]
} -->
