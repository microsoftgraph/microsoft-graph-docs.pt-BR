---
title: tipo de recurso filterClause
description: Representa uma declaração única que um objeto candidato deve satisfazer.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 91cc7f85dc4c42f806be5e365f21adb0d5e972fc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968363"
---
# <a name="filterclause-resource-type"></a><span data-ttu-id="7e5d4-103">tipo de recurso filterClause</span><span class="sxs-lookup"><span data-stu-id="7e5d4-103">filterClause resource type</span></span>

<span data-ttu-id="7e5d4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e5d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e5d4-105">Representa uma declaração única que um objeto candidato deve satisfazer e é avaliada como `true` (objeto satisfaz a asserção) ou `false` (o objeto não satisfaz a asserção).</span><span class="sxs-lookup"><span data-stu-id="7e5d4-105">Represents a single assertion that a candidate object must satisfy, and is evaluated to either `true` (object satisfies the assertion) or `false` (object does not satisfy the assertion).</span></span>

## <a name="properties"></a><span data-ttu-id="7e5d4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7e5d4-106">Properties</span></span>
| <span data-ttu-id="7e5d4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7e5d4-107">Property</span></span>     | <span data-ttu-id="7e5d4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e5d4-108">Type</span></span>   |<span data-ttu-id="7e5d4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e5d4-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e5d4-110">OperatorName</span><span class="sxs-lookup"><span data-stu-id="7e5d4-110">operatorName</span></span>|<span data-ttu-id="7e5d4-111">String</span><span class="sxs-lookup"><span data-stu-id="7e5d4-111">String</span></span>|<span data-ttu-id="7e5d4-112">Nome do operador a ser aplicado aos operandos de origem e de destino.</span><span class="sxs-lookup"><span data-stu-id="7e5d4-112">Name of the operator to be applied to the source and target operands.</span></span> <span data-ttu-id="7e5d4-113">Deve ser um dos operadores com suporte.</span><span class="sxs-lookup"><span data-stu-id="7e5d4-113">Must be one of the supported operators.</span></span> <span data-ttu-id="7e5d4-114">Os operadores com suporte podem ser descobertos.</span><span class="sxs-lookup"><span data-stu-id="7e5d4-114">Supported operators can be discovered.</span></span>|
|<span data-ttu-id="7e5d4-115">sourceOperandName</span><span class="sxs-lookup"><span data-stu-id="7e5d4-115">sourceOperandName</span></span>|<span data-ttu-id="7e5d4-116">String</span><span class="sxs-lookup"><span data-stu-id="7e5d4-116">String</span></span>|<span data-ttu-id="7e5d4-117">Nome do operando de origem (o operando que está sendo testado).</span><span class="sxs-lookup"><span data-stu-id="7e5d4-117">Name of source operand (the operand being tested).</span></span> <span data-ttu-id="7e5d4-118">O nome do operando de origem deve corresponder a um dos nomes de atributo no objeto de origem.</span><span class="sxs-lookup"><span data-stu-id="7e5d4-118">The source operand name must match one of the attribute names on the source object.</span></span>|
|<span data-ttu-id="7e5d4-119">targetOperand</span><span class="sxs-lookup"><span data-stu-id="7e5d4-119">targetOperand</span></span>|[<span data-ttu-id="7e5d4-120">filterOperand</span><span class="sxs-lookup"><span data-stu-id="7e5d4-120">filterOperand</span></span>](synchronization-filteroperand.md)|<span data-ttu-id="7e5d4-121">Valores em relação ao qual o operando de origem será testado.</span><span class="sxs-lookup"><span data-stu-id="7e5d4-121">Values that the source operand will be tested against.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7e5d4-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7e5d4-122">JSON representation</span></span>

<span data-ttu-id="7e5d4-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7e5d4-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterClause"
}-->

```json
{
  "operatorName": "String",
  "sourceOperandName": "String",
  "targetOperand": {"@odata.type": "microsoft.graph.filterOperand"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterClause resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


