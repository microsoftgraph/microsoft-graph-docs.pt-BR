---
author: chackman
description: Siga um driveItem.
title: Seguir item de unidade
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 9ae595420a59f36596027cc1438df7e931350333
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957154"
---
# <a name="follow-drive-item"></a><span data-ttu-id="33a9d-103">Seguir item de unidade</span><span class="sxs-lookup"><span data-stu-id="33a9d-103">Follow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33a9d-104">Siga um [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="33a9d-104">Follow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="33a9d-105">**Observação:** Para desacompanhar um item, confira [inseguir item](driveitem-unfollow.md).</span><span class="sxs-lookup"><span data-stu-id="33a9d-105">**Note:** To unfollow an item, see [Unfollow item](driveitem-unfollow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="33a9d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="33a9d-106">Permissions</span></span>

<span data-ttu-id="33a9d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33a9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33a9d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33a9d-109">Permission type</span></span>      | <span data-ttu-id="33a9d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="33a9d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33a9d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33a9d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="33a9d-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33a9d-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="33a9d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33a9d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33a9d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33a9d-114">Not supported.</span></span>    |
|<span data-ttu-id="33a9d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33a9d-115">Application</span></span> | <span data-ttu-id="33a9d-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33a9d-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33a9d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33a9d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/follow
POST /groups/{group-id/drive/items/{item-id}/follow
POST /me/drive/items/{item-id}/follow
POST /sites/{site-id}/drive/items/{item-id}/follow
POST /users/{user-id}/drive/items/{item-id}/follow
```

## <a name="request-body"></a><span data-ttu-id="33a9d-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33a9d-118">Request body</span></span>

<span data-ttu-id="33a9d-119">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33a9d-119">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="33a9d-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="33a9d-120">Response</span></span>

<span data-ttu-id="33a9d-121">Este método retorna um [DriveItem](../resources/driveitem.md) para o item que está sendo seguido.</span><span class="sxs-lookup"><span data-stu-id="33a9d-121">This method returns a [DriveItem](../resources/driveitem.md) for the item being followed.</span></span>

## <a name="example"></a><span data-ttu-id="33a9d-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33a9d-122">Example</span></span>

<span data-ttu-id="33a9d-123">Este exemplo segue um item identificado por `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="33a9d-123">This example follows an item identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="33a9d-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="33a9d-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "follow-item", "scopes": "files.read", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/follow
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="33a9d-125">C#</span><span class="sxs-lookup"><span data-stu-id="33a9d-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/follow-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="33a9d-126">Javascript</span><span class="sxs-lookup"><span data-stu-id="33a9d-126">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/follow-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="33a9d-127">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="33a9d-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/follow-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="33a9d-128">Java</span><span class="sxs-lookup"><span data-stu-id="33a9d-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/follow-item-java-snippets.md)]
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
