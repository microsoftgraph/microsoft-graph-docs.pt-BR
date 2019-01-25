---
author: chackman
ms.author: chackman
title: Item de unidade de parar de seguir
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 064ab2d5ad86df5341a0f2f5a46fe7c227ff35fb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513106"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="0b1fc-102">Item de unidade de parar de seguir</span><span class="sxs-lookup"><span data-stu-id="0b1fc-102">Unfollow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b1fc-103">Parar de seguir um [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="0b1fc-103">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="0b1fc-104">**Observação:** Para seguir um item, consulte [Siga Item](driveitem-follow.md).</span><span class="sxs-lookup"><span data-stu-id="0b1fc-104">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0b1fc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0b1fc-105">Permissions</span></span>

<span data-ttu-id="0b1fc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b1fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b1fc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b1fc-108">Permission type</span></span>      | <span data-ttu-id="0b1fc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0b1fc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b1fc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b1fc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0b1fc-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b1fc-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0b1fc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b1fc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b1fc-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b1fc-113">Not supported.</span></span>    |
|<span data-ttu-id="0b1fc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b1fc-114">Application</span></span> | <span data-ttu-id="0b1fc-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b1fc-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b1fc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b1fc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id} 
DELETE /users/{user-id}/drive/following/{item-id}
```

## <a name="request-body"></a><span data-ttu-id="0b1fc-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b1fc-117">Request body</span></span>

<span data-ttu-id="0b1fc-118">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b1fc-118">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="0b1fc-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b1fc-119">Response</span></span>

<span data-ttu-id="0b1fc-120">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0b1fc-120">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="0b1fc-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b1fc-121">Example</span></span>

<span data-ttu-id="0b1fc-122">Este exemplo unfollows um item identificado pela `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="0b1fc-122">This example unfollows an item identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/following/{item-id}
```


<!--
{
  "type": "#page.annotation",
  "description": "Unfollow an item that the user is following.",
  "keywords": "unfollow item",
  "section": "documentation",
  "tocPath": "Items/Unfollow",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-unfollow.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
