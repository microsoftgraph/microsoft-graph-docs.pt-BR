---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
description: O recurso Deleted indica que o item foi excluído.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c81c2623d49d40f1a4619c7f964ba9b7f0b94cf2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531682"
---
# <a name="deleted-facet"></a><span data-ttu-id="e3453-103">Faceta Deleted</span><span class="sxs-lookup"><span data-stu-id="e3453-103">Deleted facet</span></span>

<span data-ttu-id="e3453-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3453-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e3453-p101">O recurso **Deleted** indica que o item foi excluído. Nesta versão da API, a presença (não nulo) do valor do recurso indica que o arquivo foi excluído. Um valor nulo (ou faltante) indica que o arquivo não foi excluído.</span><span class="sxs-lookup"><span data-stu-id="e3453-p101">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="e3453-108">Consulte [exibir alterações de um item](../api/driveitem-delta.md) para saber mais sobre como acompanhar as alterações e localizar itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="e3453-108">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3453-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e3453-109">JSON representation</span></span>

<span data-ttu-id="e3453-110">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e3453-110">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="e3453-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e3453-111">Properties</span></span>

| <span data-ttu-id="e3453-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3453-112">Property</span></span> | <span data-ttu-id="e3453-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3453-113">Type</span></span>   | <span data-ttu-id="e3453-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3453-114">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="e3453-115">state</span><span class="sxs-lookup"><span data-stu-id="e3453-115">state</span></span>    | <span data-ttu-id="e3453-116">String</span><span class="sxs-lookup"><span data-stu-id="e3453-116">String</span></span> | <span data-ttu-id="e3453-117">Representa o estado do item excluído.</span><span class="sxs-lookup"><span data-stu-id="e3453-117">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="e3453-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="e3453-118">Remarks</span></span> 

<span data-ttu-id="e3453-119">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="e3453-119">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->
