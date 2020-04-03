---
author: learafa
description: Siga um driveItem.
title: Seguir item de unidade
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 86467b3acdd5e9ef70b393ecdbec2652341af5b2
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124354"
---
# <a name="follow-drive-item"></a><span data-ttu-id="66639-103">Seguir item de unidade</span><span class="sxs-lookup"><span data-stu-id="66639-103">Follow drive item</span></span>

<span data-ttu-id="66639-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66639-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="66639-105">Siga um [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="66639-105">Follow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="66639-106">**Observação:** Para desacompanhar um item, confira [inseguir item](driveitem-unfollow.md).</span><span class="sxs-lookup"><span data-stu-id="66639-106">**Note:** To unfollow an item, see [Unfollow item](driveitem-unfollow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="66639-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="66639-107">Permissions</span></span>

<span data-ttu-id="66639-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66639-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66639-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66639-110">Permission type</span></span>      | <span data-ttu-id="66639-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66639-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66639-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66639-112">Delegated (work or school account)</span></span> | <span data-ttu-id="66639-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66639-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="66639-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66639-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66639-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66639-115">Not supported.</span></span>    |
|<span data-ttu-id="66639-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66639-116">Application</span></span> | <span data-ttu-id="66639-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66639-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66639-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66639-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/follow
POST /groups/{group-id/drive/items/{item-id}/follow
POST /me/drive/items/{item-id}/follow
POST /sites/{site-id}/drive/items/{item-id}/follow
POST /users/{user-id}/drive/items/{item-id}/follow
```

## <a name="request-body"></a><span data-ttu-id="66639-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66639-119">Request body</span></span>

<span data-ttu-id="66639-120">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66639-120">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="66639-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="66639-121">Response</span></span>

<span data-ttu-id="66639-122">Este método retorna um [DriveItem](../resources/driveitem.md) para o item que está sendo seguido.</span><span class="sxs-lookup"><span data-stu-id="66639-122">This method returns a [DriveItem](../resources/driveitem.md) for the item being followed.</span></span>

## <a name="example"></a><span data-ttu-id="66639-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66639-123">Example</span></span>

<span data-ttu-id="66639-124">Este exemplo segue um item identificado por `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="66639-124">This example follows an item identified by `{item-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="66639-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="66639-125">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "follow-item", "scopes": "files.read", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/follow
```
# <a name="c"></a>[<span data-ttu-id="66639-126">C#</span><span class="sxs-lookup"><span data-stu-id="66639-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/follow-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66639-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66639-127">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/follow-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66639-128">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66639-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/follow-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="66639-129">Java</span><span class="sxs-lookup"><span data-stu-id="66639-129">Java</span></span>](#tab/java)
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
