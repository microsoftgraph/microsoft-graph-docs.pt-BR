---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Fazer check-out de arquivos
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5da9dba96ca19d94bd0eec8a8039e752ec28b894
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325351"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="18862-102">Fazer check-out do recurso DriveItem</span><span class="sxs-lookup"><span data-stu-id="18862-102">Check-out a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18862-103">Check-out de um recurso driveItem para impedir que outras pessoas editem o documento e que suas alterações fiquem visíveis até que o documento passe por [check-in](driveitem-checkin.md).</span><span class="sxs-lookup"><span data-stu-id="18862-103">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="18862-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="18862-104">Permissions</span></span>

<span data-ttu-id="18862-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18862-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18862-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18862-107">Permission type</span></span>      | <span data-ttu-id="18862-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18862-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18862-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18862-109">Delegated (work or school account)</span></span> | <span data-ttu-id="18862-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18862-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="18862-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18862-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18862-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18862-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="18862-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18862-113">Application</span></span> | <span data-ttu-id="18862-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18862-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18862-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18862-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="18862-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18862-116">Request body</span></span>

<span data-ttu-id="18862-117">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18862-117">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="18862-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18862-118">Example</span></span>

<span data-ttu-id="18862-119">Este exemplo faz check-out de um arquivo identificado por `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="18862-119">This example checks out a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```

## <a name="response"></a><span data-ttu-id="18862-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="18862-120">Response</span></span>

<span data-ttu-id="18862-121">Se tiver êxito, a chamada API retorna um código `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="18862-121">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="18862-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="18862-122">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": []
}
-->
