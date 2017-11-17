---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "Excluído"
ms.openlocfilehash: 1d45219b2ef26bdc96c46e386d66d91874f9bc0b
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="deleted-facet"></a><span data-ttu-id="079f4-102">Faceta Deleted</span><span class="sxs-lookup"><span data-stu-id="079f4-102">Deleted facet</span></span>

<span data-ttu-id="079f4-103">O recurso **Deleted** indica que o item foi excluído.</span><span class="sxs-lookup"><span data-stu-id="079f4-103">The **Deleted** resource indicates that the item has been deleted.</span></span>
<span data-ttu-id="079f4-104">Nesta versão da API, a presença (não nulo) do valor do recurso indica que o arquivo foi excluído.</span><span class="sxs-lookup"><span data-stu-id="079f4-104">The Deleted resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>
<span data-ttu-id="079f4-105">Um valor nulo (ou faltante) indica que o arquivo não foi excluído.</span><span class="sxs-lookup"><span data-stu-id="079f4-105">A null (or missing) value indicates the driveItem is not the root..</span></span>

<span data-ttu-id="079f4-106">Confira [exibir alterações de um item](../api/driveitem_delta.md) para saber mais sobre como acompanhar as alterações e localizar itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="079f4-106">See [view changes for an item](../api/driveitem_delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="079f4-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="079f4-107">JSON representation</span></span>

<span data-ttu-id="079f4-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="079f4-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="079f4-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="079f4-109">Properties</span></span>

| <span data-ttu-id="079f4-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="079f4-110">Property</span></span> | <span data-ttu-id="079f4-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="079f4-111">Type</span></span>   | <span data-ttu-id="079f4-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="079f4-112">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="079f4-113">state</span><span class="sxs-lookup"><span data-stu-id="079f4-113">state</span></span>    | <span data-ttu-id="079f4-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="079f4-114">String</span></span> | <span data-ttu-id="079f4-115">Representa o estado do item excluído.</span><span class="sxs-lookup"><span data-stu-id="079f4-115">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="079f4-116">Comentários</span><span class="sxs-lookup"><span data-stu-id="079f4-116">Remarks</span></span> 

<span data-ttu-id="079f4-117">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="079f4-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->
