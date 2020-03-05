---
title: tipo de recurso filterClause
description: Representa uma declaração única que um objeto candidato deve satisfazer e é avaliada como `true` (objeto satisfaz a asserção) ou `false` (o objeto não satisfaz a asserção).
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 66ccbc4e445b6fa90dad1bac55c00f894bbd934b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520188"
---
# <a name="filterclause-resource-type"></a><span data-ttu-id="ee976-103">tipo de recurso filterClause</span><span class="sxs-lookup"><span data-stu-id="ee976-103">filterClause resource type</span></span>

<span data-ttu-id="ee976-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ee976-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee976-105">Representa uma declaração única que um objeto candidato deve satisfazer e é avaliada como `true` (objeto satisfaz a asserção) ou `false` (o objeto não satisfaz a asserção).</span><span class="sxs-lookup"><span data-stu-id="ee976-105">Represents a single assertion that a candidate object must satisfy, and is evaluated to either `true` (object satisfies the assertion) or `false` (object does not satisfy the assertion).</span></span>

## <a name="properties"></a><span data-ttu-id="ee976-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee976-106">Properties</span></span>
| <span data-ttu-id="ee976-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee976-107">Property</span></span>     | <span data-ttu-id="ee976-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee976-108">Type</span></span>   |<span data-ttu-id="ee976-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee976-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee976-110">OperatorName</span><span class="sxs-lookup"><span data-stu-id="ee976-110">operatorName</span></span>|<span data-ttu-id="ee976-111">String</span><span class="sxs-lookup"><span data-stu-id="ee976-111">String</span></span>|<span data-ttu-id="ee976-112">Nome do operador a ser aplicado aos operandos de origem e de destino.</span><span class="sxs-lookup"><span data-stu-id="ee976-112">Name of the operator to be applied to the source and target operands.</span></span> <span data-ttu-id="ee976-113">Deve ser um dos operadores com suporte.</span><span class="sxs-lookup"><span data-stu-id="ee976-113">Must be one of the supported operators.</span></span> <span data-ttu-id="ee976-114">Os operadores com suporte podem ser descobertos.</span><span class="sxs-lookup"><span data-stu-id="ee976-114">Supported operators can be discovered.</span></span>|
|<span data-ttu-id="ee976-115">sourceOperandName</span><span class="sxs-lookup"><span data-stu-id="ee976-115">sourceOperandName</span></span>|<span data-ttu-id="ee976-116">String</span><span class="sxs-lookup"><span data-stu-id="ee976-116">String</span></span>|<span data-ttu-id="ee976-117">Nome do operando de origem (o operando que está sendo testado).</span><span class="sxs-lookup"><span data-stu-id="ee976-117">Name of source operand (the operand being tested).</span></span> <span data-ttu-id="ee976-118">O nome do operando de origem deve corresponder a um dos nomes de atributo no objeto de origem.</span><span class="sxs-lookup"><span data-stu-id="ee976-118">The source operand name must match one of the attribute names on the source object.</span></span>|
|<span data-ttu-id="ee976-119">targetOperand</span><span class="sxs-lookup"><span data-stu-id="ee976-119">targetOperand</span></span>|[<span data-ttu-id="ee976-120">filterOperand</span><span class="sxs-lookup"><span data-stu-id="ee976-120">filterOperand</span></span>](synchronization-filteroperand.md)|<span data-ttu-id="ee976-121">Valores em relação ao qual o operando de origem será testado.</span><span class="sxs-lookup"><span data-stu-id="ee976-121">Values that the source operand will be tested against.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ee976-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee976-122">JSON representation</span></span>

<span data-ttu-id="ee976-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee976-123">The following is a JSON representation of the resource.</span></span>

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
