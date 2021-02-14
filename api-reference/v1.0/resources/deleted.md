---
author: JeremyKelley
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
description: O recurso Deleted indica que o item foi excluído.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3743a343b9928eda4a888cff06a3ff1b7525f9c9
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239608"
---
# <a name="deleted-facet"></a><span data-ttu-id="fd032-103">Faceta Deleted</span><span class="sxs-lookup"><span data-stu-id="fd032-103">Deleted facet</span></span>

<span data-ttu-id="fd032-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd032-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fd032-p101">O recurso **Deleted** indica que o item foi excluído. Nesta versão da API, a presença (não nulo) do valor do recurso indica que o arquivo foi excluído. Um valor nulo (ou faltante) indica que o arquivo não foi excluído.</span><span class="sxs-lookup"><span data-stu-id="fd032-p101">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="fd032-108">Consulte [exibir alterações de um item](../api/driveitem-delta.md) para saber mais sobre como acompanhar as alterações e localizar itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="fd032-108">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd032-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fd032-109">JSON representation</span></span>

<span data-ttu-id="fd032-110">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fd032-110">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="fd032-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fd032-111">Properties</span></span>

| <span data-ttu-id="fd032-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd032-112">Property</span></span> | <span data-ttu-id="fd032-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd032-113">Type</span></span>   | <span data-ttu-id="fd032-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd032-114">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="fd032-115">estado</span><span class="sxs-lookup"><span data-stu-id="fd032-115">state</span></span>    | <span data-ttu-id="fd032-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd032-116">String</span></span> | <span data-ttu-id="fd032-117">Representa o estado do item excluído.</span><span class="sxs-lookup"><span data-stu-id="fd032-117">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="fd032-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="fd032-118">Remarks</span></span> 

<span data-ttu-id="fd032-119">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="fd032-119">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->

