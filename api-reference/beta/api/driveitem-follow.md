---
author: chackman
ms.author: chackman
title: Siga o item de unidade
localization_priority: Normal
ms.openlocfilehash: 5ba37773f552015b6c762b2b10d801b40670a03c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875030"
---
# <a name="follow-drive-item"></a><span data-ttu-id="20e17-102">Siga o item de unidade</span><span class="sxs-lookup"><span data-stu-id="20e17-102">Follow drive item</span></span>

> <span data-ttu-id="20e17-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="20e17-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20e17-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="20e17-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="20e17-105">Siga um [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="20e17-105">Follow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="20e17-106">**Observação:** Para parar de seguir um item, consulte [Unfollow item](driveitem-unfollow.md).</span><span class="sxs-lookup"><span data-stu-id="20e17-106">**Note:** To unfollow an item, see [Unfollow item](driveitem-unfollow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="20e17-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="20e17-107">Permissions</span></span>

<span data-ttu-id="20e17-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20e17-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20e17-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20e17-110">Permission type</span></span>      | <span data-ttu-id="20e17-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20e17-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20e17-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20e17-112">Delegated (work or school account)</span></span> | <span data-ttu-id="20e17-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20e17-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="20e17-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20e17-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20e17-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20e17-115">Not supported.</span></span>    |
|<span data-ttu-id="20e17-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20e17-116">Application</span></span> | <span data-ttu-id="20e17-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20e17-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20e17-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20e17-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/follow
POST /groups/{group-id/drive/items/{item-id}/follow
POST /me/drive/items/{item-id}/follow
POST /sites/{site-id}/drive/items/{item-id}/follow
POST /users/{user-id}/drive/items/{item-id}/follow
```

## <a name="request-body"></a><span data-ttu-id="20e17-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20e17-119">Request body</span></span>

<span data-ttu-id="20e17-120">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20e17-120">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="20e17-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="20e17-121">Response</span></span>

<span data-ttu-id="20e17-122">Esse método retorna um [DriveItem](../resources/driveitem.md) para o item sendo seguido.</span><span class="sxs-lookup"><span data-stu-id="20e17-122">This method returns a [DriveItem](../resources/driveitem.md) for the item being followed.</span></span>

## <a name="example"></a><span data-ttu-id="20e17-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20e17-123">Example</span></span>

<span data-ttu-id="20e17-124">Este exemplo segue um item identificado pela `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="20e17-124">This example follows an item identified by `{item-id}`.</span></span>

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
