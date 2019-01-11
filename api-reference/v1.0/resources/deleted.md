---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Excluído
localization_priority: Normal
ms.openlocfilehash: a35bc781555486603c0319c819aa019704e362d9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886139"
---
# <a name="deleted-facet"></a><span data-ttu-id="2c4f8-102">Faceta Deleted</span><span class="sxs-lookup"><span data-stu-id="2c4f8-102">Deleted facet</span></span>

<span data-ttu-id="2c4f8-p101">O recurso **Deleted** indica que o item foi excluído. Nesta versão da API, a presença (não nulo) do valor do recurso indica que o arquivo foi excluído. Um valor nulo (ou faltante) indica que o arquivo não foi excluído.</span><span class="sxs-lookup"><span data-stu-id="2c4f8-p101">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="2c4f8-106">Consulte [exibir alterações de um item](../api/driveitem-delta.md) para saber mais sobre como acompanhar as alterações e localizar itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="2c4f8-106">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c4f8-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c4f8-107">JSON representation</span></span>

<span data-ttu-id="2c4f8-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2c4f8-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="2c4f8-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c4f8-109">Properties</span></span>

| <span data-ttu-id="2c4f8-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c4f8-110">Property</span></span> | <span data-ttu-id="2c4f8-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c4f8-111">Type</span></span>   | <span data-ttu-id="2c4f8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c4f8-112">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="2c4f8-113">state</span><span class="sxs-lookup"><span data-stu-id="2c4f8-113">state</span></span>    | <span data-ttu-id="2c4f8-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2c4f8-114">String</span></span> | <span data-ttu-id="2c4f8-115">Representa o estado do item excluído.</span><span class="sxs-lookup"><span data-stu-id="2c4f8-115">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="2c4f8-116">Comentários</span><span class="sxs-lookup"><span data-stu-id="2c4f8-116">Remarks</span></span> 

<span data-ttu-id="2c4f8-117">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="2c4f8-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->
