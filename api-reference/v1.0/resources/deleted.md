---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
description: O recurso Deleted indica que o item foi excluído.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d1f5c07c60c8de4890a2a4ac334df04a59b7339c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029516"
---
# <a name="deleted-facet"></a><span data-ttu-id="e378a-103">Faceta Deleted</span><span class="sxs-lookup"><span data-stu-id="e378a-103">Deleted facet</span></span>

<span data-ttu-id="e378a-p101">O recurso **Deleted** indica que o item foi excluído. Nesta versão da API, a presença (não nulo) do valor do recurso indica que o arquivo foi excluído. Um valor nulo (ou faltante) indica que o arquivo não foi excluído.</span><span class="sxs-lookup"><span data-stu-id="e378a-p101">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="e378a-107">Consulte [exibir alterações de um item](../api/driveitem-delta.md) para saber mais sobre como acompanhar as alterações e localizar itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="e378a-107">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e378a-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e378a-108">JSON representation</span></span>

<span data-ttu-id="e378a-109">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e378a-109">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="e378a-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e378a-110">Properties</span></span>

| <span data-ttu-id="e378a-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e378a-111">Property</span></span> | <span data-ttu-id="e378a-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="e378a-112">Type</span></span>   | <span data-ttu-id="e378a-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="e378a-113">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="e378a-114">state</span><span class="sxs-lookup"><span data-stu-id="e378a-114">state</span></span>    | <span data-ttu-id="e378a-115">String</span><span class="sxs-lookup"><span data-stu-id="e378a-115">String</span></span> | <span data-ttu-id="e378a-116">Representa o estado do item excluído.</span><span class="sxs-lookup"><span data-stu-id="e378a-116">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="e378a-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="e378a-117">Remarks</span></span> 

<span data-ttu-id="e378a-118">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="e378a-118">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->
