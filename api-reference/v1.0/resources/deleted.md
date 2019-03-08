---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
ms.openlocfilehash: d52ca0a9815e46ebc11a653be381ac65f3cd209e
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482179"
---
# <a name="deleted-facet"></a><span data-ttu-id="d9f69-102">Faceta Deleted</span><span class="sxs-lookup"><span data-stu-id="d9f69-102">Deleted facet</span></span>

<span data-ttu-id="d9f69-p101">O recurso **Deleted** indica que o item foi excluído. Nesta versão da API, a presença (não nulo) do valor do recurso indica que o arquivo foi excluído. Um valor nulo (ou faltante) indica que o arquivo não foi excluído.</span><span class="sxs-lookup"><span data-stu-id="d9f69-p101">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="d9f69-106">Consulte [exibir alterações de um item](../api/driveitem-delta.md) para saber mais sobre como acompanhar as alterações e localizar itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="d9f69-106">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9f69-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d9f69-107">JSON representation</span></span>

<span data-ttu-id="d9f69-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d9f69-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="d9f69-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d9f69-109">Properties</span></span>

| <span data-ttu-id="d9f69-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9f69-110">Property</span></span> | <span data-ttu-id="d9f69-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9f69-111">Type</span></span>   | <span data-ttu-id="d9f69-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9f69-112">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="d9f69-113">state</span><span class="sxs-lookup"><span data-stu-id="d9f69-113">state</span></span>    | <span data-ttu-id="d9f69-114">String</span><span class="sxs-lookup"><span data-stu-id="d9f69-114">String</span></span> | <span data-ttu-id="d9f69-115">Representa o estado do item excluído.</span><span class="sxs-lookup"><span data-stu-id="d9f69-115">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="d9f69-116">Comentários</span><span class="sxs-lookup"><span data-stu-id="d9f69-116">Remarks</span></span> 

<span data-ttu-id="d9f69-117">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="d9f69-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->
