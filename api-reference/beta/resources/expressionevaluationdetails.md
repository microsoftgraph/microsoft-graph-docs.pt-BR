---
title: Tipo de recurso expressionEvaluationDetails
description: Representa os detalhes da expressão, o resultado e os detalhes da propriedade.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 01cc4aa4bd6de88541d3886efe54e5da71228448
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129485"
---
# <a name="expressionevaluationdetails-resource-type"></a><span data-ttu-id="882b4-103">Tipo de recurso expressionEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="882b4-103">expressionEvaluationDetails resource type</span></span>

<span data-ttu-id="882b4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="882b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="882b4-105">Representa os detalhes da expressão, o resultado e os detalhes da propriedade.</span><span class="sxs-lookup"><span data-stu-id="882b4-105">Represents the expression details, result, and property details.</span></span>

## <a name="properties"></a><span data-ttu-id="882b4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="882b4-106">Properties</span></span>

| <span data-ttu-id="882b4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="882b4-107">Property</span></span>     | <span data-ttu-id="882b4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="882b4-108">Type</span></span>        | <span data-ttu-id="882b4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="882b4-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="882b4-110">expressão</span><span class="sxs-lookup"><span data-stu-id="882b4-110">expression</span></span> | <span data-ttu-id="882b4-111">String</span><span class="sxs-lookup"><span data-stu-id="882b4-111">String</span></span> | <span data-ttu-id="882b4-112">Representa a expressão que foi avaliada.</span><span class="sxs-lookup"><span data-stu-id="882b4-112">Represents expression which has been evaluated.</span></span> |
| <span data-ttu-id="882b4-113">expressionEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="882b4-113">expressionEvaluationDetails</span></span> | <span data-ttu-id="882b4-114">Coleção expressionEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="882b4-114">expressionEvaluationDetails collection</span></span> | <span data-ttu-id="882b4-115">Representa os detalhes da avaliação da expressão.</span><span class="sxs-lookup"><span data-stu-id="882b4-115">Represents the details of the evaluation of the expression.</span></span> |
| <span data-ttu-id="882b4-116">expressionResult</span><span class="sxs-lookup"><span data-stu-id="882b4-116">expressionResult</span></span> | <span data-ttu-id="882b4-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="882b4-117">Boolean</span></span> | <span data-ttu-id="882b4-118">Representa o valor do resultado da expressão atual.</span><span class="sxs-lookup"><span data-stu-id="882b4-118">Represents the value of the result of the current expression.</span></span> |
| <span data-ttu-id="882b4-119">propertyToEvaluate</span><span class="sxs-lookup"><span data-stu-id="882b4-119">propertyToEvaluate</span></span> | [<span data-ttu-id="882b4-120">propertyToEvaluate</span><span class="sxs-lookup"><span data-stu-id="882b4-120">propertyToEvaluate</span></span>](propertytoevaluate.md) | <span data-ttu-id="882b4-121">Define o nome da propriedade e o valor dessa propriedade.</span><span class="sxs-lookup"><span data-stu-id="882b4-121">Defines the name of the property and the value of that property.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="882b4-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="882b4-122">JSON representation</span></span>

<span data-ttu-id="882b4-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="882b4-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expressionEvaluationDetails",
  "baseType": null
}-->

```json
{
  "expression": "String",
  "expressionEvaluationDetails": [{"@odata.type": "microsoft.graph.expressionEvaluationDetails"}],
  "expressionResult": true,
  "propertyToEvaluate": {"@odata.type": "microsoft.graph.propertyToEvaluate"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "expressionEvaluationDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


