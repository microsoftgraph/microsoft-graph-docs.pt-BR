---
title: Obter um recurso ListItemVersion
description: Recuperar os metadados de uma versão específica de um ListItem.
localization_priority: Normal
ms.prod: sharepoint
author: JeremyKelley
doc_type: apiPageType
ms.openlocfilehash: 474ce406f39eb1b43324677d9e48ed844e2d78df
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057247"
---
# <a name="get-a-listitemversion-resource"></a><span data-ttu-id="93618-103">Obter um recurso ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="93618-103">Get a ListItemVersion resource</span></span>

<span data-ttu-id="93618-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93618-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="93618-105">Recuperar os metadados de uma versão específica de um [ListItem](../resources/listitem.md).</span><span class="sxs-lookup"><span data-stu-id="93618-105">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="93618-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="93618-106">Permissions</span></span>

<span data-ttu-id="93618-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93618-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="93618-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93618-109">Permission type</span></span>             | <span data-ttu-id="93618-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="93618-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="93618-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93618-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="93618-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93618-112">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="93618-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93618-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93618-114">n/d</span><span class="sxs-lookup"><span data-stu-id="93618-114">n/a</span></span>                                         |
| <span data-ttu-id="93618-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93618-115">Application</span></span>                            | <span data-ttu-id="93618-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93618-116">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="93618-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93618-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="93618-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="93618-118">Response</span></span>

<span data-ttu-id="93618-119">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ListItemVersion](../resources/listitemversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93618-119">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="93618-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93618-120">Example</span></span>

<span data-ttu-id="93618-121">Este exemplo recupera uma versão de um item de lista e expande o conjunto de campos para solicitar os valores dos campos no listItem.</span><span class="sxs-lookup"><span data-stu-id="93618-121">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="93618-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93618-122">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="93618-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="93618-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read sites.read.all", "tags": "service.graph service.sharepoint" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}?expand=fields
```
# <a name="c"></a>[<span data-ttu-id="93618-124">C#</span><span class="sxs-lookup"><span data-stu-id="93618-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-single-version-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93618-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93618-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-single-version-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93618-126">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93618-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-single-version-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="93618-127">Java</span><span class="sxs-lookup"><span data-stu-id="93618-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-single-version-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="93618-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="93618-128">Response</span></span>

<span data-ttu-id="93618-129">Isso retornará uma coleção de versões:</span><span class="sxs-lookup"><span data-stu-id="93618-129">This returns a collection of versions:</span></span>

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

