---
author: chackman
ms.author: chackman
title: Item da unidade não seguir
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e3ab51d5aaa4074837a0cd7126ac6548b09d4acd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860896"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="0ac12-102">Item da unidade não seguir</span><span class="sxs-lookup"><span data-stu-id="0ac12-102">Unfollow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ac12-103">Não seguir um [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="0ac12-103">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="0ac12-104">**Observação:** Para seguir um item, consulte [follow item](driveitem-follow.md).</span><span class="sxs-lookup"><span data-stu-id="0ac12-104">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0ac12-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0ac12-105">Permissions</span></span>

<span data-ttu-id="0ac12-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ac12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ac12-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ac12-108">Permission type</span></span>      | <span data-ttu-id="0ac12-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0ac12-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ac12-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ac12-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0ac12-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ac12-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0ac12-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ac12-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ac12-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ac12-113">Not supported.</span></span>    |
|<span data-ttu-id="0ac12-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ac12-114">Application</span></span> | <span data-ttu-id="0ac12-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ac12-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ac12-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ac12-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id} 
DELETE /users/{user-id}/drive/following/{item-id}
```

## <a name="request-body"></a><span data-ttu-id="0ac12-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ac12-117">Request body</span></span>

<span data-ttu-id="0ac12-118">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ac12-118">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="0ac12-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ac12-119">Response</span></span>

<span data-ttu-id="0ac12-120">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0ac12-120">If successful, the API call returns a `204 No Content`.</span></span> <span data-ttu-id="0ac12-121">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ac12-121">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ac12-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ac12-122">Example</span></span>
### <a name="request"></a><span data-ttu-id="0ac12-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ac12-123">Request</span></span>
<span data-ttu-id="0ac12-124">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ac12-124">Here is an example of the request.</span></span>
<span data-ttu-id="0ac12-125">Este exemplo não segue um item identificado por `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="0ac12-125">This example unfollows an item identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0ac12-126">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ac12-126">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/following/{item-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0ac12-127">C#</span><span class="sxs-lookup"><span data-stu-id="0ac12-127">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unfollow-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0ac12-128">Javascript</span><span class="sxs-lookup"><span data-stu-id="0ac12-128">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unfollow-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0ac12-129">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0ac12-129">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unfollow-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0ac12-130">Java</span><span class="sxs-lookup"><span data-stu-id="0ac12-130">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unfollow-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="0ac12-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ac12-131">Response</span></span>
<!-- { 
    "blockType": "response", 
    "truncated": true 
} -->
```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "description": "Unfollow an item that the user is following.",
  "keywords": "unfollow item",
  "section": "documentation",
  "tocPath": "Items/Unfollow",
  "suppressions": [
  ]
}
-->
