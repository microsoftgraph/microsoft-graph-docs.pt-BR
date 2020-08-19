---
title: Listando versões de um ListItem
description: O SharePoint pode ser configurado para manter o histórico para itens da lista.
localization_priority: Normal
ms.prod: sharepoint
author: JeremyKelley
doc_type: apiPageType
ms.openlocfilehash: b0466116acaa447d5a45e1ecede1137a93eee965
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812727"
---
# <a name="listing-versions-of-a-listitem"></a><span data-ttu-id="14858-103">Listando versões de um ListItem</span><span class="sxs-lookup"><span data-stu-id="14858-103">Listing versions of a ListItem</span></span>

<span data-ttu-id="14858-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14858-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="14858-105">O SharePoint pode ser configurado para manter o histórico para itens da lista.</span><span class="sxs-lookup"><span data-stu-id="14858-105">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="14858-106">Versões anteriores podem ser mantidas por um determinado período dependendo das configurações de administração que podem ser exclusivas por usuário ou local.</span><span class="sxs-lookup"><span data-stu-id="14858-106">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="14858-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="14858-107">Permissions</span></span>

<span data-ttu-id="14858-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14858-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="14858-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14858-110">Permission type</span></span>             | <span data-ttu-id="14858-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="14858-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="14858-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14858-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="14858-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14858-113">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="14858-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14858-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14858-115">n/d</span><span class="sxs-lookup"><span data-stu-id="14858-115">n/a</span></span>                                         |
| <span data-ttu-id="14858-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14858-116">Application</span></span>                            | <span data-ttu-id="14858-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14858-117">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="14858-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14858-118">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="14858-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="14858-119">Response</span></span>

<span data-ttu-id="14858-120">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ListItemVersion](../resources/listitemversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14858-120">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="14858-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14858-121">Example</span></span>

<span data-ttu-id="14858-122">Este exemplo recupera as versões de um listItem em uma lista do SharePoint:</span><span class="sxs-lookup"><span data-stu-id="14858-122">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="14858-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14858-123">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="14858-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="14858-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read sites.read.all" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```
# <a name="c"></a>[<span data-ttu-id="14858-125">C#</span><span class="sxs-lookup"><span data-stu-id="14858-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-previous-versions-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14858-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14858-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-previous-versions-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14858-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14858-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-previous-versions-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14858-128">Java</span><span class="sxs-lookup"><span data-stu-id="14858-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-previous-versions-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="14858-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="14858-129">Response</span></span>

<span data-ttu-id="14858-130">Isso retornará uma coleção de versões:</span><span class="sxs-lookup"><span data-stu-id="14858-130">This returns a collection of versions:</span></span>

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
