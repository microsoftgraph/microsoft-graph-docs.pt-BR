---
title: Listando versões de um ListItem
description: O SharePoint pode ser configurado para manter o histórico para itens da lista.
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: apiPageType
ms.openlocfilehash: 55c0ebce4055ea481e0bfeed63cb0b850b4ebad2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023138"
---
# <a name="listing-versions-of-a-listitem"></a><span data-ttu-id="d51f5-103">Listando versões de um ListItem</span><span class="sxs-lookup"><span data-stu-id="d51f5-103">Listing versions of a ListItem</span></span>

<span data-ttu-id="d51f5-104">O SharePoint pode ser configurado para manter o histórico para itens da lista.</span><span class="sxs-lookup"><span data-stu-id="d51f5-104">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="d51f5-105">Versões anteriores podem ser mantidas por um determinado período dependendo das configurações de administração que podem ser exclusivas por usuário ou local.</span><span class="sxs-lookup"><span data-stu-id="d51f5-105">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="d51f5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d51f5-106">Permissions</span></span>

<span data-ttu-id="d51f5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d51f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="d51f5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d51f5-109">Permission type</span></span>             | <span data-ttu-id="d51f5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d51f5-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="d51f5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d51f5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d51f5-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d51f5-112">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="d51f5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d51f5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d51f5-114">n/d</span><span class="sxs-lookup"><span data-stu-id="d51f5-114">n/a</span></span>                                         |
| <span data-ttu-id="d51f5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d51f5-115">Application</span></span>                            | <span data-ttu-id="d51f5-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d51f5-116">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="d51f5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d51f5-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="d51f5-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="d51f5-118">Response</span></span>

<span data-ttu-id="d51f5-119">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ListItemVersion](../resources/listitemversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d51f5-119">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="d51f5-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d51f5-120">Example</span></span>

<span data-ttu-id="d51f5-121">Este exemplo recupera as versões de um listItem em uma lista do SharePoint:</span><span class="sxs-lookup"><span data-stu-id="d51f5-121">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="d51f5-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d51f5-122">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d51f5-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="d51f5-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d51f5-124">C#</span><span class="sxs-lookup"><span data-stu-id="d51f5-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-previous-versions-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d51f5-125">Javascript</span><span class="sxs-lookup"><span data-stu-id="d51f5-125">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-previous-versions-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d51f5-126">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d51f5-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-previous-versions-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d51f5-127">Java</span><span class="sxs-lookup"><span data-stu-id="d51f5-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-previous-versions-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d51f5-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d51f5-128">Response</span></span>

<span data-ttu-id="d51f5-129">Isso retornará uma coleção de versões:</span><span class="sxs-lookup"><span data-stu-id="d51f5-129">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.listItemVersion)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value":
  [
    {
      "id": "3.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-14T12:34:53.912Z"
    },
    {
      "id": "2.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-11T10:21:03.000Z"
    },
    {
      "id": "1.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-10T15:20:01.125Z"
    }
  ]
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
