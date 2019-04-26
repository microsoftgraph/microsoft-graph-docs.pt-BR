---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
ms.openlocfilehash: 06fe9835ef4b31d7a48bad955b17872142a94b2d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535282"
---
# <a name="deleted-facet"></a><span data-ttu-id="438fb-102">Faceta Deleted</span><span class="sxs-lookup"><span data-stu-id="438fb-102">Deleted facet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="438fb-p101">O recurso **Deleted** indica que o item foi excluído. Nesta versão da API, a presença (não nulo) do valor do recurso indica que o arquivo foi excluído. Um valor nulo (ou faltante) indica que o arquivo não foi excluído.</span><span class="sxs-lookup"><span data-stu-id="438fb-p101">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="438fb-106">Consulte [exibir alterações de um item](../api/driveitem-delta.md) para saber mais sobre como acompanhar as alterações e localizar itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="438fb-106">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="438fb-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="438fb-107">JSON representation</span></span>

<span data-ttu-id="438fb-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="438fb-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="438fb-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="438fb-109">Properties</span></span>

| <span data-ttu-id="438fb-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="438fb-110">Property</span></span> | <span data-ttu-id="438fb-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="438fb-111">Type</span></span>   | <span data-ttu-id="438fb-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="438fb-112">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="438fb-113">state</span><span class="sxs-lookup"><span data-stu-id="438fb-113">state</span></span>    | <span data-ttu-id="438fb-114">String</span><span class="sxs-lookup"><span data-stu-id="438fb-114">String</span></span> | <span data-ttu-id="438fb-115">Representa o estado do item excluído.</span><span class="sxs-lookup"><span data-stu-id="438fb-115">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="438fb-116">Comentários</span><span class="sxs-lookup"><span data-stu-id="438fb-116">Remarks</span></span> 

<span data-ttu-id="438fb-117">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="438fb-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted",
  "suppressions": []
}
-->
