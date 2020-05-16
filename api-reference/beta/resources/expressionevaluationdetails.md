---
title: tipo de recurso expressionEvaluationDetails
description: Representa os detalhes de propriedade, resultado e detalhes da expressão.
localization_priority: Normal
author: yyuank
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 347e356bda19228ea8b3738b5bf8b72f57da95f7
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272819"
---
# <a name="expressionevaluationdetails-resource-type"></a><span data-ttu-id="ecd31-103">tipo de recurso expressionEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="ecd31-103">expressionEvaluationDetails resource type</span></span>

<span data-ttu-id="ecd31-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecd31-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ecd31-105">Representa os detalhes de propriedade, resultado e detalhes da expressão.</span><span class="sxs-lookup"><span data-stu-id="ecd31-105">Represents the expression details, result, and property details.</span></span>

## <a name="properties"></a><span data-ttu-id="ecd31-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ecd31-106">Properties</span></span>

| <span data-ttu-id="ecd31-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ecd31-107">Property</span></span>     | <span data-ttu-id="ecd31-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ecd31-108">Type</span></span>        | <span data-ttu-id="ecd31-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecd31-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ecd31-110">expressão</span><span class="sxs-lookup"><span data-stu-id="ecd31-110">expression</span></span> | <span data-ttu-id="ecd31-111">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="ecd31-111">String</span></span> | <span data-ttu-id="ecd31-112">Representa a expressão que foi avaliada.</span><span class="sxs-lookup"><span data-stu-id="ecd31-112">Represents expression which has been evaluated.</span></span> |
| <span data-ttu-id="ecd31-113">expressionEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="ecd31-113">expressionEvaluationDetails</span></span> | <span data-ttu-id="ecd31-114">coleção expressionEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="ecd31-114">expressionEvaluationDetails collection</span></span> | <span data-ttu-id="ecd31-115">Representa os detalhes da avaliação da expressão.</span><span class="sxs-lookup"><span data-stu-id="ecd31-115">Represents the details of the evaluation of the expression.</span></span> |
| <span data-ttu-id="ecd31-116">expressionResult</span><span class="sxs-lookup"><span data-stu-id="ecd31-116">expressionResult</span></span> | <span data-ttu-id="ecd31-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="ecd31-117">Boolean</span></span> | <span data-ttu-id="ecd31-118">Representa o valor do resultado da expressão atual.</span><span class="sxs-lookup"><span data-stu-id="ecd31-118">Represents the value of the result of the current expression.</span></span> |
| <span data-ttu-id="ecd31-119">propertyToEvaluate</span><span class="sxs-lookup"><span data-stu-id="ecd31-119">propertyToEvaluate</span></span> | [<span data-ttu-id="ecd31-120">propertyToEvaluate</span><span class="sxs-lookup"><span data-stu-id="ecd31-120">propertyToEvaluate</span></span>](propertytoevaluate.md) | <span data-ttu-id="ecd31-121">Define o nome da propriedade e o valor dessa propriedade.</span><span class="sxs-lookup"><span data-stu-id="ecd31-121">Defines the name of the property and the value of that property.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ecd31-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ecd31-122">JSON representation</span></span>

<span data-ttu-id="ecd31-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ecd31-123">The following is a JSON representation of the resource.</span></span>

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
