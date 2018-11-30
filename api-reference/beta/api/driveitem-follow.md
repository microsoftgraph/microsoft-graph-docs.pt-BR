---
author: chackman
ms.author: chackman
title: Siga o item de unidade
ms.openlocfilehash: dcfe05e445baa4d01b2968c417648b6b65a17296
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034261"
---
# <a name="follow-drive-item"></a><span data-ttu-id="2dde4-102">Siga o item de unidade</span><span class="sxs-lookup"><span data-stu-id="2dde4-102">Follow drive item</span></span>

> <span data-ttu-id="2dde4-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2dde4-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2dde4-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2dde4-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2dde4-105">Siga um [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="2dde4-105">Follow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="2dde4-106">**Observação:** Para parar de seguir um item, consulte [Unfollow item](driveitem-unfollow.md).</span><span class="sxs-lookup"><span data-stu-id="2dde4-106">**Note:** To unfollow an item, see [Unfollow item](driveitem-unfollow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2dde4-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="2dde4-107">Permissions</span></span>

<span data-ttu-id="2dde4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2dde4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2dde4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2dde4-110">Permission type</span></span>      | <span data-ttu-id="2dde4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2dde4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2dde4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2dde4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2dde4-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2dde4-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2dde4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2dde4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2dde4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2dde4-115">Not supported.</span></span>    |
|<span data-ttu-id="2dde4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2dde4-116">Application</span></span> | <span data-ttu-id="2dde4-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2dde4-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2dde4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2dde4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/follow
POST /groups/{group-id/drive/items/{item-id}/follow
POST /me/drive/items/{item-id}/follow
POST /sites/{site-id}/drive/items/{item-id}/follow
POST /users/{user-id}/drive/items/{item-id}/follow
```

## <a name="request-body"></a><span data-ttu-id="2dde4-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2dde4-119">Request body</span></span>

<span data-ttu-id="2dde4-120">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2dde4-120">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="2dde4-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="2dde4-121">Response</span></span>

<span data-ttu-id="2dde4-122">Esse método retorna um [DriveItem](../resources/driveitem.md) para o item sendo seguido.</span><span class="sxs-lookup"><span data-stu-id="2dde4-122">This method returns a [DriveItem](../resources/driveitem.md) for the item being followed.</span></span>

## <a name="example"></a><span data-ttu-id="2dde4-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2dde4-123">Example</span></span>

<span data-ttu-id="2dde4-124">Este exemplo segue um item identificado pela `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="2dde4-124">This example follows an item identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "follow-item", "scopes": "files.read", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/follow
```

<!-- {
  "type": "#page.annotation",
  "description": "Follow an item.",
  "keywords": "follow item",
  "section": "documentation",
  "tocPath": "Items/Follow"
} -->

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
