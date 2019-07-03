---
author: chackman
ms.author: chackman
title: Seguir item de unidade
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1dc7cdd1f863687773236fee927b6c5a37cf82ea
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436421"
---
# <a name="follow-drive-item"></a><span data-ttu-id="a0d67-102">Seguir item de unidade</span><span class="sxs-lookup"><span data-stu-id="a0d67-102">Follow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0d67-103">Siga um [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="a0d67-103">Follow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="a0d67-104">**Observação:** Para desacompanhar um item, confira [inseguir item](driveitem-unfollow.md).</span><span class="sxs-lookup"><span data-stu-id="a0d67-104">**Note:** To unfollow an item, see [Unfollow item](driveitem-unfollow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a0d67-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0d67-105">Permissions</span></span>

<span data-ttu-id="a0d67-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0d67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0d67-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0d67-108">Permission type</span></span>      | <span data-ttu-id="a0d67-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a0d67-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0d67-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0d67-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a0d67-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0d67-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a0d67-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0d67-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0d67-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0d67-113">Not supported.</span></span>    |
|<span data-ttu-id="a0d67-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0d67-114">Application</span></span> | <span data-ttu-id="a0d67-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0d67-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0d67-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0d67-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/follow
POST /groups/{group-id/drive/items/{item-id}/follow
POST /me/drive/items/{item-id}/follow
POST /sites/{site-id}/drive/items/{item-id}/follow
POST /users/{user-id}/drive/items/{item-id}/follow
```

## <a name="request-body"></a><span data-ttu-id="a0d67-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0d67-117">Request body</span></span>

<span data-ttu-id="a0d67-118">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0d67-118">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="a0d67-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0d67-119">Response</span></span>

<span data-ttu-id="a0d67-120">Este método retorna um [DriveItem](../resources/driveitem.md) para o item que está sendo seguido.</span><span class="sxs-lookup"><span data-stu-id="a0d67-120">This method returns a [DriveItem](../resources/driveitem.md) for the item being followed.</span></span>

## <a name="example"></a><span data-ttu-id="a0d67-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0d67-121">Example</span></span>

<span data-ttu-id="a0d67-122">Este exemplo segue um item identificado por `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="a0d67-122">This example follows an item identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a0d67-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0d67-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "follow-item", "scopes": "files.read", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/follow
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a0d67-124">C#</span><span class="sxs-lookup"><span data-stu-id="a0d67-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/follow-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a0d67-125">Javascript</span><span class="sxs-lookup"><span data-stu-id="a0d67-125">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/follow-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a0d67-126">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a0d67-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/follow-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!--
{
  "type": "#page.annotation",
  "description": "Follow an item.",
  "keywords": "follow item",
  "section": "documentation",
  "tocPath": "Items/Follow",
  "suppressions": [
  ]
}
-->

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1312abc!1231",
  "name": "March Proposal.docx",
  "size": 19121,
  "lastModifiedDateTime": "2017-12-12T10:40:59Z"
}
```
