---
title: Obter um recurso ListItemVersion
description: Recuperar os metadados de uma versão específica de um ListItem.
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: apiPageType
ms.openlocfilehash: 4012b58864715741800276e0ca2e16f8ae765de5
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728780"
---
# <a name="get-a-listitemversion-resource"></a><span data-ttu-id="91fd6-103">Obter um recurso ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="91fd6-103">Get a ListItemVersion resource</span></span>

<span data-ttu-id="91fd6-104">Recuperar os metadados de uma versão específica de um [ListItem](../resources/listitem.md).</span><span class="sxs-lookup"><span data-stu-id="91fd6-104">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="91fd6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="91fd6-105">Permissions</span></span>

<span data-ttu-id="91fd6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91fd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="91fd6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91fd6-108">Permission type</span></span>             | <span data-ttu-id="91fd6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91fd6-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="91fd6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91fd6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="91fd6-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91fd6-111">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="91fd6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91fd6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91fd6-113">n/d</span><span class="sxs-lookup"><span data-stu-id="91fd6-113">n/a</span></span>                                         |
| <span data-ttu-id="91fd6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91fd6-114">Application</span></span>                            | <span data-ttu-id="91fd6-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91fd6-115">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="91fd6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91fd6-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="91fd6-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="91fd6-117">Response</span></span>

<span data-ttu-id="91fd6-118">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ListItemVersion](../resources/listitemversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91fd6-118">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="91fd6-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91fd6-119">Example</span></span>

<span data-ttu-id="91fd6-120">Este exemplo recupera uma versão de um item de lista e expande o conjunto de campos para solicitar os valores dos campos no listItem.</span><span class="sxs-lookup"><span data-stu-id="91fd6-120">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="91fd6-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91fd6-121">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="91fd6-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="91fd6-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read sites.read.all", "tags": "service.graph service.sharepoint" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}?expand=fields
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="91fd6-123">C#</span><span class="sxs-lookup"><span data-stu-id="91fd6-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-single-version-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="91fd6-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91fd6-124">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-single-version-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="91fd6-125">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="91fd6-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-single-version-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="91fd6-126">Java</span><span class="sxs-lookup"><span data-stu-id="91fd6-126">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-single-version-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="91fd6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="91fd6-127">Response</span></span>

<span data-ttu-id="91fd6-128">Isso retornará uma coleção de versões:</span><span class="sxs-lookup"><span data-stu-id="91fd6-128">This returns a collection of versions:</span></span>

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
