---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Excluído
localization_priority: Normal
ms.openlocfilehash: 6316f31d41e9d8e7264a671ac0317ebf9b32173f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804764"
---
# <a name="deleted-facet"></a><span data-ttu-id="e30eb-102">Faceta Deleted</span><span class="sxs-lookup"><span data-stu-id="e30eb-102">Deleted facet</span></span>

> <span data-ttu-id="e30eb-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e30eb-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e30eb-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e30eb-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e30eb-p102">O recurso **Deleted** indica que o item foi excluído. Nesta versão da API, a presença (não nulo) do valor do recurso indica que o arquivo foi excluído. Um valor nulo (ou faltante) indica que o arquivo não foi excluído.</span><span class="sxs-lookup"><span data-stu-id="e30eb-p102">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="e30eb-108">Consulte [exibir alterações de um item](../api/driveitem-delta.md) para saber mais sobre como acompanhar as alterações e localizar itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="e30eb-108">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e30eb-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e30eb-109">JSON representation</span></span>

<span data-ttu-id="e30eb-110">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e30eb-110">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="e30eb-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e30eb-111">Properties</span></span>

| <span data-ttu-id="e30eb-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e30eb-112">Property</span></span> | <span data-ttu-id="e30eb-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="e30eb-113">Type</span></span>   | <span data-ttu-id="e30eb-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="e30eb-114">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="e30eb-115">state</span><span class="sxs-lookup"><span data-stu-id="e30eb-115">state</span></span>    | <span data-ttu-id="e30eb-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e30eb-116">String</span></span> | <span data-ttu-id="e30eb-117">Representa o estado do item excluído.</span><span class="sxs-lookup"><span data-stu-id="e30eb-117">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="e30eb-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="e30eb-118">Remarks</span></span> 

<span data-ttu-id="e30eb-119">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="e30eb-119">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->
