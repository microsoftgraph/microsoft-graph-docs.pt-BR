---
title: tipo de recurso expressionEvaluationDetails
description: Representa os detalhes de propriedade, resultado e detalhes da expressão.
localization_priority: Normal
author: yyuank
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f2d14d19bee60581c65d43e81b5ec69acc53df0a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026968"
---
# <a name="expressionevaluationdetails-resource-type"></a><span data-ttu-id="a9bb5-103">tipo de recurso expressionEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="a9bb5-103">expressionEvaluationDetails resource type</span></span>

<span data-ttu-id="a9bb5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9bb5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9bb5-105">Representa os detalhes de propriedade, resultado e detalhes da expressão.</span><span class="sxs-lookup"><span data-stu-id="a9bb5-105">Represents the expression details, result, and property details.</span></span>

## <a name="properties"></a><span data-ttu-id="a9bb5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a9bb5-106">Properties</span></span>

| <span data-ttu-id="a9bb5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9bb5-107">Property</span></span>     | <span data-ttu-id="a9bb5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9bb5-108">Type</span></span>        | <span data-ttu-id="a9bb5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9bb5-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a9bb5-110">expressão</span><span class="sxs-lookup"><span data-stu-id="a9bb5-110">expression</span></span> | <span data-ttu-id="a9bb5-111">String</span><span class="sxs-lookup"><span data-stu-id="a9bb5-111">String</span></span> | <span data-ttu-id="a9bb5-112">Representa a expressão que foi avaliada.</span><span class="sxs-lookup"><span data-stu-id="a9bb5-112">Represents expression which has been evaluated.</span></span> |
| <span data-ttu-id="a9bb5-113">expressionEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="a9bb5-113">expressionEvaluationDetails</span></span> | <span data-ttu-id="a9bb5-114">coleção expressionEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="a9bb5-114">expressionEvaluationDetails collection</span></span> | <span data-ttu-id="a9bb5-115">Representa os detalhes da avaliação da expressão.</span><span class="sxs-lookup"><span data-stu-id="a9bb5-115">Represents the details of the evaluation of the expression.</span></span> |
| <span data-ttu-id="a9bb5-116">expressionResult</span><span class="sxs-lookup"><span data-stu-id="a9bb5-116">expressionResult</span></span> | <span data-ttu-id="a9bb5-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="a9bb5-117">Boolean</span></span> | <span data-ttu-id="a9bb5-118">Representa o valor do resultado da expressão atual.</span><span class="sxs-lookup"><span data-stu-id="a9bb5-118">Represents the value of the result of the current expression.</span></span> |
| <span data-ttu-id="a9bb5-119">propertyToEvaluate</span><span class="sxs-lookup"><span data-stu-id="a9bb5-119">propertyToEvaluate</span></span> | [<span data-ttu-id="a9bb5-120">propertyToEvaluate</span><span class="sxs-lookup"><span data-stu-id="a9bb5-120">propertyToEvaluate</span></span>](propertytoevaluate.md) | <span data-ttu-id="a9bb5-121">Define o nome da propriedade e o valor dessa propriedade.</span><span class="sxs-lookup"><span data-stu-id="a9bb5-121">Defines the name of the property and the value of that property.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a9bb5-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a9bb5-122">JSON representation</span></span>

<span data-ttu-id="a9bb5-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a9bb5-123">The following is a JSON representation of the resource.</span></span>

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


