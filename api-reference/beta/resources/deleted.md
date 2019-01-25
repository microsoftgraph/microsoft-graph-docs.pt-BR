---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Excluído
localization_priority: Normal
ms.openlocfilehash: de832eb4ecdf36081b00b94679dcafe9b94fe007
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529436"
---
# <a name="deleted-facet"></a><span data-ttu-id="d35c9-102">Faceta Deleted</span><span class="sxs-lookup"><span data-stu-id="d35c9-102">Deleted facet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d35c9-p101">O recurso Deleted indica que o item foi excluído. Nesta versão da API, a presença (não nulo) do valor do recurso indica que o arquivo foi excluído. Um valor nulo (ou faltante) indica que o arquivo não foi excluído.</span><span class="sxs-lookup"><span data-stu-id="d35c9-p101">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="d35c9-106">Consulte [exibir alterações de um item](../api/driveitem-delta.md) para saber mais sobre como acompanhar as alterações e localizar itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="d35c9-106">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d35c9-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d35c9-107">JSON representation</span></span>

<span data-ttu-id="d35c9-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d35c9-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  "state"
  ],
  "@odata.type": "microsoft.graph.deleted"
}-->
```json
{
  "state": "string"
}
```
## <a name="properties"></a><span data-ttu-id="d35c9-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d35c9-109">Properties</span></span>

| <span data-ttu-id="d35c9-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d35c9-110">Property</span></span> | <span data-ttu-id="d35c9-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d35c9-111">Type</span></span>   | <span data-ttu-id="d35c9-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d35c9-112">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="d35c9-113">state</span><span class="sxs-lookup"><span data-stu-id="d35c9-113">state</span></span>    | <span data-ttu-id="d35c9-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d35c9-114">String</span></span> | <span data-ttu-id="d35c9-115">Representa o estado do item excluído.</span><span class="sxs-lookup"><span data-stu-id="d35c9-115">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="d35c9-116">Comentários</span><span class="sxs-lookup"><span data-stu-id="d35c9-116">Remarks</span></span> 

<span data-ttu-id="d35c9-117">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="d35c9-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted",
  "suppressions": [
    "Error: /api-reference/beta/resources/deleted.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
