---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Check-Out de arquivos
ms.openlocfilehash: c8b7cd9231150d9898ea21a15c4745791137cdba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034564"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="75c70-102">Fazer check-out do recurso DriveItem</span><span class="sxs-lookup"><span data-stu-id="75c70-102">Check-out a DriveItem resource</span></span>

> <span data-ttu-id="75c70-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="75c70-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75c70-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="75c70-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="75c70-105">Check-out de um recurso driveItem para impedir que outras pessoas editem o documento e que suas alterações fiquem visíveis até que o documento passe por [check-in](driveitem-checkin.md).</span><span class="sxs-lookup"><span data-stu-id="75c70-105">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="75c70-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="75c70-106">Permissions</span></span>

<span data-ttu-id="75c70-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75c70-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75c70-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75c70-109">Permission type</span></span>      | <span data-ttu-id="75c70-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="75c70-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75c70-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75c70-111">Delegated (work or school account)</span></span> | <span data-ttu-id="75c70-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75c70-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="75c70-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75c70-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75c70-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75c70-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="75c70-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75c70-115">Application</span></span> | <span data-ttu-id="75c70-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75c70-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="75c70-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75c70-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="75c70-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75c70-118">Request body</span></span>

<span data-ttu-id="75c70-119">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75c70-119">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="75c70-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75c70-120">Example</span></span>

<span data-ttu-id="75c70-121">Este exemplo faz check-out de um arquivo identificado por `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="75c70-121">This example checks out a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```

## <a name="response"></a><span data-ttu-id="75c70-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="75c70-122">Response</span></span>

<span data-ttu-id="75c70-123">Se tiver êxito, a chamada API retorna um código `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="75c70-123">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="75c70-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="75c70-124">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
