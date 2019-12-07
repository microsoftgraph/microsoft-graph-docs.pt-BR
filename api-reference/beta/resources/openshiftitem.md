---
title: tipo de recurso openShiftItem
description: Representa uma única contagem de um turno aberto.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 86392d330403acf667f81c1dce4bbc951bb8185d
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895568"
---
# <a name="openshiftitem-resource-type"></a><span data-ttu-id="72a08-103">tipo de recurso openShiftItem</span><span class="sxs-lookup"><span data-stu-id="72a08-103">openShiftItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72a08-104">Representa uma única contagem de um [openshift](../resources/openshift.md).</span><span class="sxs-lookup"><span data-stu-id="72a08-104">Represents a single count of an [openshift](../resources/openshift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="72a08-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="72a08-105">Properties</span></span>

| <span data-ttu-id="72a08-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="72a08-106">Property</span></span>     | <span data-ttu-id="72a08-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="72a08-107">Type</span></span>        | <span data-ttu-id="72a08-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="72a08-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="72a08-109">openSlotCount</span><span class="sxs-lookup"><span data-stu-id="72a08-109">openSlotCount</span></span>|<span data-ttu-id="72a08-110">Int32</span><span class="sxs-lookup"><span data-stu-id="72a08-110">Int32</span></span>| <span data-ttu-id="72a08-111">Contagem do número de Slots para o turno aberto especificado.</span><span class="sxs-lookup"><span data-stu-id="72a08-111">Count of the number of slots for the given open shift.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="72a08-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="72a08-112">JSON representation</span></span>

<span data-ttu-id="72a08-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="72a08-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openShiftItem",
  "baseType": "microsoft.graph.shiftItem"
}-->

```json
{
  "openSlotCount": 1024
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openShiftItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
