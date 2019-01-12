---
author: chackman
ms.author: chackman
title: Item de unidade de parar de seguir
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a42f740b3ea6f706529a5353e9cbb846bb7a4e6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945948"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="c0d5c-102">Item de unidade de parar de seguir</span><span class="sxs-lookup"><span data-stu-id="c0d5c-102">Unfollow drive item</span></span>

> <span data-ttu-id="c0d5c-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c0d5c-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0d5c-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c0d5c-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c0d5c-105">Parar de seguir um [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="c0d5c-105">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="c0d5c-106">**Observação:** Para seguir um item, consulte [Siga Item](driveitem-follow.md).</span><span class="sxs-lookup"><span data-stu-id="c0d5c-106">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c0d5c-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="c0d5c-107">Permissions</span></span>

<span data-ttu-id="c0d5c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0d5c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0d5c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0d5c-110">Permission type</span></span>      | <span data-ttu-id="c0d5c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0d5c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0d5c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0d5c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c0d5c-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0d5c-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c0d5c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0d5c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0d5c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0d5c-115">Not supported.</span></span>    |
|<span data-ttu-id="c0d5c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0d5c-116">Application</span></span> | <span data-ttu-id="c0d5c-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0d5c-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0d5c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0d5c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id} 
DELETE /users/{user-id}/drive/following/{item-id}
```

## <a name="request-body"></a><span data-ttu-id="c0d5c-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0d5c-119">Request body</span></span>

<span data-ttu-id="c0d5c-120">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0d5c-120">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="c0d5c-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0d5c-121">Response</span></span>

<span data-ttu-id="c0d5c-122">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c0d5c-122">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="c0d5c-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0d5c-123">Example</span></span>

<span data-ttu-id="c0d5c-124">Este exemplo unfollows um item identificado pela `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="c0d5c-124">This example unfollows an item identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/following/{item-id}
```


<!-- {
  "type": "#page.annotation",
  "description": "Unfollow an item that the user is following.",
  "keywords": "unfollow item",
  "section": "documentation",
  "tocPath": "Items/Unfollow"
} -->
