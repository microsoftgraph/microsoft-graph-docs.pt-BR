---
author: chackman
ms.author: chackman
title: Seguir item de unidade
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b0c8835593ed7203cc6239485f1dcd4f17f24fe7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454402"
---
# <a name="follow-drive-item"></a><span data-ttu-id="32c8f-102">Seguir item de unidade</span><span class="sxs-lookup"><span data-stu-id="32c8f-102">Follow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32c8f-103">Siga um [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="32c8f-103">Follow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="32c8f-104">**Observação:** Para desacompanhar um item, confira [inseguir item](driveitem-unfollow.md).</span><span class="sxs-lookup"><span data-stu-id="32c8f-104">**Note:** To unfollow an item, see [Unfollow item](driveitem-unfollow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="32c8f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="32c8f-105">Permissions</span></span>

<span data-ttu-id="32c8f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32c8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32c8f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32c8f-108">Permission type</span></span>      | <span data-ttu-id="32c8f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="32c8f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32c8f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32c8f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="32c8f-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32c8f-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="32c8f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32c8f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32c8f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32c8f-113">Not supported.</span></span>    |
|<span data-ttu-id="32c8f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32c8f-114">Application</span></span> | <span data-ttu-id="32c8f-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32c8f-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="32c8f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32c8f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/follow
POST /groups/{group-id/drive/items/{item-id}/follow
POST /me/drive/items/{item-id}/follow
POST /sites/{site-id}/drive/items/{item-id}/follow
POST /users/{user-id}/drive/items/{item-id}/follow
```

## <a name="request-body"></a><span data-ttu-id="32c8f-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32c8f-117">Request body</span></span>

<span data-ttu-id="32c8f-118">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32c8f-118">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="32c8f-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="32c8f-119">Response</span></span>

<span data-ttu-id="32c8f-120">Este método retorna um [DriveItem](../resources/driveitem.md) para o item que está sendo seguido.</span><span class="sxs-lookup"><span data-stu-id="32c8f-120">This method returns a [DriveItem](../resources/driveitem.md) for the item being followed.</span></span>

## <a name="example"></a><span data-ttu-id="32c8f-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32c8f-121">Example</span></span>

<span data-ttu-id="32c8f-122">Este exemplo segue um item identificado por `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="32c8f-122">This example follows an item identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "follow-item", "scopes": "files.read", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/follow
```

<!--
{
  "type": "#page.annotation",
  "description": "Follow an item.",
  "keywords": "follow item",
  "section": "documentation",
  "tocPath": "Items/Follow",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-follow.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
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
