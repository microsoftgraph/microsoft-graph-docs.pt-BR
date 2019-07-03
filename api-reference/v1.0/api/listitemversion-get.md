---
title: Obter um recurso ListItemVersion
description: Recuperar os metadados de uma versão específica de um ListItem.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c0c91c44b61b980da8a498b7f15ae6b71a42562e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460697"
---
# <a name="get-a-listitemversion-resource"></a><span data-ttu-id="160b1-103">Obter um recurso ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="160b1-103">Get a ListItemVersion resource</span></span>

<span data-ttu-id="160b1-104">Recuperar os metadados de uma versão específica de um [ListItem](../resources/listitem.md).</span><span class="sxs-lookup"><span data-stu-id="160b1-104">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="160b1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="160b1-105">Permissions</span></span>

<span data-ttu-id="160b1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="160b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="160b1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="160b1-108">Permission type</span></span>             | <span data-ttu-id="160b1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="160b1-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="160b1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="160b1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="160b1-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="160b1-111">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="160b1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="160b1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="160b1-113">n/d</span><span class="sxs-lookup"><span data-stu-id="160b1-113">n/a</span></span>                                         |
| <span data-ttu-id="160b1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="160b1-114">Application</span></span>                            | <span data-ttu-id="160b1-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="160b1-115">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="160b1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="160b1-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="160b1-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="160b1-117">Response</span></span>

<span data-ttu-id="160b1-118">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ListItemVersion](../resources/listitemversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="160b1-118">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="160b1-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="160b1-119">Example</span></span>

<span data-ttu-id="160b1-120">Este exemplo recupera uma versão de um item de lista e expande o conjunto de campos para solicitar os valores dos campos no listItem.</span><span class="sxs-lookup"><span data-stu-id="160b1-120">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="160b1-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="160b1-121">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="160b1-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="160b1-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read sites.read.all", "tags": "service.graph service.sharepoint" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}?expand=fields
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="160b1-123">C#</span><span class="sxs-lookup"><span data-stu-id="160b1-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-single-version-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="160b1-124">Javascript</span><span class="sxs-lookup"><span data-stu-id="160b1-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-single-version-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="160b1-125">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="160b1-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-single-version-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="160b1-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="160b1-126">Response</span></span>

<span data-ttu-id="160b1-127">Isso retornará uma coleção de versões:</span><span class="sxs-lookup"><span data-stu-id="160b1-127">This returns a collection of versions:</span></span>

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
