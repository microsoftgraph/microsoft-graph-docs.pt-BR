---
author: JeremyKelley
description: O recurso Deleted indica que o item foi excluído.
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: b3c1a7a4c9a7c290ba71a21ba288e6195334377b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507265"
---
# <a name="deleted-facet"></a><span data-ttu-id="dab32-103">Faceta Deleted</span><span class="sxs-lookup"><span data-stu-id="dab32-103">Deleted facet</span></span>

<span data-ttu-id="dab32-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dab32-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dab32-p101">O recurso **Deleted** indica que o item foi excluído. Nesta versão da API, a presença (não nulo) do valor do recurso indica que o arquivo foi excluído. Um valor nulo (ou faltante) indica que o arquivo não foi excluído.</span><span class="sxs-lookup"><span data-stu-id="dab32-p101">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="dab32-108">Consulte [exibir alterações de um item](../api/driveitem-delta.md) para saber mais sobre como acompanhar as alterações e localizar itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="dab32-108">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dab32-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dab32-109">JSON representation</span></span>

<span data-ttu-id="dab32-110">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dab32-110">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="dab32-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dab32-111">Properties</span></span>

| <span data-ttu-id="dab32-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dab32-112">Property</span></span> | <span data-ttu-id="dab32-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="dab32-113">Type</span></span>   | <span data-ttu-id="dab32-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="dab32-114">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="dab32-115">state</span><span class="sxs-lookup"><span data-stu-id="dab32-115">state</span></span>    | <span data-ttu-id="dab32-116">String</span><span class="sxs-lookup"><span data-stu-id="dab32-116">String</span></span> | <span data-ttu-id="dab32-117">Representa o estado do item excluído.</span><span class="sxs-lookup"><span data-stu-id="dab32-117">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="dab32-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="dab32-118">Remarks</span></span> 

<span data-ttu-id="dab32-119">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="dab32-119">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


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
