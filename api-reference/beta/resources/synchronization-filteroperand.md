---
title: tipo de recurso filterOperand
description: Contém uma coleção de valores para o operando.
localization_priority: Normal
ms.openlocfilehash: ab62477889cc92954ed308c508e18a638cd59375
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581797"
---
# <a name="filteroperand-resource-type"></a><span data-ttu-id="fdd81-103">tipo de recurso filterOperand</span><span class="sxs-lookup"><span data-stu-id="fdd81-103">filterOperand resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdd81-104">Contém uma coleção de valores para o operando.</span><span class="sxs-lookup"><span data-stu-id="fdd81-104">Contains a collection of values for the operand.</span></span>

## <a name="properties"></a><span data-ttu-id="fdd81-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fdd81-105">Properties</span></span>
| <span data-ttu-id="fdd81-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fdd81-106">Property</span></span>     | <span data-ttu-id="fdd81-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="fdd81-107">Type</span></span>   |<span data-ttu-id="fdd81-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdd81-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fdd81-109">values</span><span class="sxs-lookup"><span data-stu-id="fdd81-109">values</span></span>|<span data-ttu-id="fdd81-110">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="fdd81-110">String collection</span></span>|<span data-ttu-id="fdd81-111">Coleção de valores.</span><span class="sxs-lookup"><span data-stu-id="fdd81-111">Collection of values.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fdd81-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fdd81-112">JSON representation</span></span>

<span data-ttu-id="fdd81-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fdd81-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterOperand"
}-->

```json
{
  "values": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterOperand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filteroperand.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
