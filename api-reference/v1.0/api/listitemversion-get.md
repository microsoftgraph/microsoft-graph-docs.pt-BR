---
title: Obter um recurso ListItemVersion
description: Recuperar os metadados de uma versão específica de um ListItem.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: d36c09c62cd802c8514781df26f5cac076f107df
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613460"
---
# <a name="get-a-listitemversion-resource"></a><span data-ttu-id="527c2-103">Obter um recurso ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="527c2-103">Get a ListItemVersion resource</span></span>

<span data-ttu-id="527c2-104">Recuperar os metadados de uma versão específica de um [ListItem](../resources/listitem.md).</span><span class="sxs-lookup"><span data-stu-id="527c2-104">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="527c2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="527c2-105">Permissions</span></span>

<span data-ttu-id="527c2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="527c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="527c2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="527c2-108">Permission type</span></span>             | <span data-ttu-id="527c2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="527c2-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="527c2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="527c2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="527c2-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="527c2-111">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="527c2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="527c2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="527c2-113">n/d</span><span class="sxs-lookup"><span data-stu-id="527c2-113">n/a</span></span>                                         |
| <span data-ttu-id="527c2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="527c2-114">Application</span></span>                            | <span data-ttu-id="527c2-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="527c2-115">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="527c2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="527c2-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="527c2-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="527c2-117">Response</span></span>

<span data-ttu-id="527c2-118">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ListItemVersion](../resources/listitemversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="527c2-118">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="527c2-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="527c2-119">Example</span></span>

<span data-ttu-id="527c2-120">Este exemplo recupera uma versão de um item de lista e expande o conjunto de campos para solicitar os valores dos campos no listItem.</span><span class="sxs-lookup"><span data-stu-id="527c2-120">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="527c2-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="527c2-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read sites.read.all", "tags": "service.graph service.sharepoint" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="527c2-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="527c2-122">Response</span></span>

<span data-ttu-id="527c2-123">Isso retornará uma coleção de versões:</span><span class="sxs-lookup"><span data-stu-id="527c2-123">This returns a collection of versions:</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="527c2-124">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="527c2-124">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="527c2-125">Basic</span><span class="sxs-lookup"><span data-stu-id="527c2-125">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-single-version-listItem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="527c2-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="527c2-126">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-single-version-listItem-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitemversion-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitemversion-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
