---
author: chackman
ms.author: chackman
title: Item da unidade não seguir
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 67438469beceeff50d067c7507318a0e0df5e543
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33588233"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="1be78-102">Item da unidade não seguir</span><span class="sxs-lookup"><span data-stu-id="1be78-102">Unfollow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1be78-103">Não seguir um [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="1be78-103">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="1be78-104">**Observação:** Para seguir um item, consulte [follow item](driveitem-follow.md).</span><span class="sxs-lookup"><span data-stu-id="1be78-104">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1be78-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1be78-105">Permissions</span></span>

<span data-ttu-id="1be78-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1be78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1be78-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1be78-108">Permission type</span></span>      | <span data-ttu-id="1be78-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1be78-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1be78-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1be78-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1be78-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1be78-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1be78-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1be78-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1be78-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1be78-113">Not supported.</span></span>    |
|<span data-ttu-id="1be78-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1be78-114">Application</span></span> | <span data-ttu-id="1be78-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1be78-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1be78-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1be78-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id} 
DELETE /users/{user-id}/drive/following/{item-id}
```

## <a name="request-body"></a><span data-ttu-id="1be78-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1be78-117">Request body</span></span>

<span data-ttu-id="1be78-118">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1be78-118">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="1be78-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="1be78-119">Response</span></span>

<span data-ttu-id="1be78-120">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1be78-120">If successful, the API call returns a `204 No Content`.</span></span> <span data-ttu-id="1be78-121">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1be78-121">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1be78-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1be78-122">Example</span></span>
### <a name="request"></a><span data-ttu-id="1be78-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1be78-123">Request</span></span>
<span data-ttu-id="1be78-124">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1be78-124">Here is an example of the request.</span></span>
<span data-ttu-id="1be78-125">Este exemplo não segue um item identificado por `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="1be78-125">This example unfollows an item identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/following/{item-id}
```
### <a name="response"></a><span data-ttu-id="1be78-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="1be78-126">Response</span></span>
<!-- { 
    "blockType": "response", 
    "truncated": true 
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1be78-127">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="1be78-127">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1be78-128">Basic</span><span class="sxs-lookup"><span data-stu-id="1be78-128">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/unfollow-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1be78-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1be78-129">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/unfollow-item-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!--
{
  "type": "#page.annotation",
  "description": "Unfollow an item that the user is following.",
  "keywords": "unfollow item",
  "section": "documentation",
  "tocPath": "Items/Unfollow",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-unfollow.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-unfollow.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
