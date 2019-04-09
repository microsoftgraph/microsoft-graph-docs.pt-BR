---
author: chackman
ms.author: chackman
title: Item da unidade não seguir
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 730bb02dda88f41bcac734b3ba282ad324267860
ms.sourcegitcommit: 9fd437a77da99d8436d6c852edd99a9ba873f8cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/09/2019
ms.locfileid: "31560105"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="adbde-102">Item da unidade não seguir</span><span class="sxs-lookup"><span data-stu-id="adbde-102">Unfollow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adbde-103">Não seguir um [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="adbde-103">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="adbde-104">**Observação:** Para seguir um item, consulte [follow item](driveitem-follow.md).</span><span class="sxs-lookup"><span data-stu-id="adbde-104">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="adbde-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="adbde-105">Permissions</span></span>

<span data-ttu-id="adbde-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adbde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adbde-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="adbde-108">Permission type</span></span>      | <span data-ttu-id="adbde-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="adbde-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="adbde-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="adbde-110">Delegated (work or school account)</span></span> | <span data-ttu-id="adbde-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adbde-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="adbde-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="adbde-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="adbde-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="adbde-113">Not supported.</span></span>    |
|<span data-ttu-id="adbde-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="adbde-114">Application</span></span> | <span data-ttu-id="adbde-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adbde-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="adbde-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="adbde-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id} 
DELETE /users/{user-id}/drive/following/{item-id}
```

## <a name="request-body"></a><span data-ttu-id="adbde-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="adbde-117">Request body</span></span>

<span data-ttu-id="adbde-118">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="adbde-118">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="adbde-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="adbde-119">Response</span></span>

<span data-ttu-id="adbde-120">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="adbde-120">If successful, the API call returns a `204 No Content`.</span></span> <span data-ttu-id="adbde-121">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="adbde-121">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adbde-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="adbde-122">Example</span></span>
### <a name="request"></a><span data-ttu-id="adbde-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="adbde-123">Request</span></span>
<span data-ttu-id="adbde-124">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="adbde-124">Here is an example of the request.</span></span>
<span data-ttu-id="adbde-125">Este exemplo não segue um item identificado por `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="adbde-125">This example unfollows an item identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/following/{item-id}
```
### <a name="response"></a><span data-ttu-id="adbde-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="adbde-126">Response</span></span>
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
    "Error: /api-reference/beta/api/driveitem-unfollow.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
