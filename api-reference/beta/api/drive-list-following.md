---
author: chackman
ms.author: chackman
title: Listar itens visitados
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: df38a11a09f4ec86eb029f236030cc4565e5d939
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523306"
---
# <a name="list-followed-items"></a><span data-ttu-id="37127-102">Listar itens visitados</span><span class="sxs-lookup"><span data-stu-id="37127-102">List followed items</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37127-103">Lista os [itens](../resources/driveitem.md) que foram visitados pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="37127-103">List the [items](../resources/driveitem.md) that have been followed by the signed in user.</span></span>
<span data-ttu-id="37127-104">Esta coleção inclui itens que estão na unidade do usuário, bem como os itens que eles têm acesso a partir de outras unidades.</span><span class="sxs-lookup"><span data-stu-id="37127-104">This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="37127-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="37127-105">Permissions</span></span>

<span data-ttu-id="37127-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37127-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37127-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37127-108">Permission type</span></span>      | <span data-ttu-id="37127-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37127-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37127-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37127-110">Delegated (work or school account)</span></span> | <span data-ttu-id="37127-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37127-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="37127-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37127-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37127-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37127-113">Not supported.</span></span>    |
|<span data-ttu-id="37127-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37127-114">Application</span></span> | <span data-ttu-id="37127-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37127-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37127-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37127-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-followed-items", "scopes": "files.read" } -->

```http
GET /me/drive/following
```

## <a name="response"></a><span data-ttu-id="37127-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="37127-117">Response</span></span>

<span data-ttu-id="37127-118">Esse método retorna uma coleção de recursos de [driveItem](../resources/driveitem.md) para itens que o proprietário da unidade está seguindo.</span><span class="sxs-lookup"><span data-stu-id="37127-118">This method returns a collection of [driveItem](../resources/driveitem.md) resources for items which the owner of the drive is following.</span></span>
<span data-ttu-id="37127-119">Se nenhum item foi encontrado, uma coleção vazia é retornada.</span><span class="sxs-lookup"><span data-stu-id="37127-119">If no items were found, an empty collection is returned.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "1312abc!1231",
      "name": "March Proposal.docx",
      "size": 19121,
      "lastModifiedDateTime": "2017-12-12T10:40:59Z"
    },
    {
      "id": "1312def!9943",
      "name": "Vacation.jpg",
      "size": 37810,
      "lastModifiedDateTime": "2016-10-18T10:40:59Z"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "List the items a user is following.",
  "keywords": "drive,onedrive.drive,list followed items",
  "section": "documentation",
  "tocPath": "Drives/List followed items",
  "suppressions": [
    "Error: /api-reference/beta/api/drive-list-following.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
