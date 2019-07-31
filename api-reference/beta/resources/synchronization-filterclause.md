---
title: tipo de recurso filterClause
description: Representa uma declaração única que um objeto candidato deve satisfazer e é avaliada como `true` (objeto satisfaz a asserção) ou `false` (o objeto não satisfaz a asserção).
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 83b9c68bd86f716b47a3ba3774022ff3ba520770
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007932"
---
# <a name="filterclause-resource-type"></a><span data-ttu-id="82682-103">tipo de recurso filterClause</span><span class="sxs-lookup"><span data-stu-id="82682-103">filterClause resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82682-104">Representa uma declaração única que um objeto candidato deve satisfazer e é avaliada como `true` (objeto satisfaz a asserção) ou `false` (o objeto não satisfaz a asserção).</span><span class="sxs-lookup"><span data-stu-id="82682-104">Represents a single assertion that a candidate object must satisfy, and is evaluated to either `true` (object satisfies the assertion) or `false` (object does not satisfy the assertion).</span></span>

## <a name="properties"></a><span data-ttu-id="82682-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="82682-105">Properties</span></span>
| <span data-ttu-id="82682-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82682-106">Property</span></span>     | <span data-ttu-id="82682-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="82682-107">Type</span></span>   |<span data-ttu-id="82682-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="82682-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82682-109">OperatorName</span><span class="sxs-lookup"><span data-stu-id="82682-109">operatorName</span></span>|<span data-ttu-id="82682-110">String</span><span class="sxs-lookup"><span data-stu-id="82682-110">String</span></span>|<span data-ttu-id="82682-111">Nome do operador a ser aplicado aos operandos de origem e de destino.</span><span class="sxs-lookup"><span data-stu-id="82682-111">Name of the operator to be applied to the source and target operands.</span></span> <span data-ttu-id="82682-112">Deve ser um dos operadores com suporte.</span><span class="sxs-lookup"><span data-stu-id="82682-112">Must be one of the supported operators.</span></span> <span data-ttu-id="82682-113">Os operadores com suporte podem ser descobertos.</span><span class="sxs-lookup"><span data-stu-id="82682-113">Supported operators can be discovered.</span></span>|
|<span data-ttu-id="82682-114">sourceOperandName</span><span class="sxs-lookup"><span data-stu-id="82682-114">sourceOperandName</span></span>|<span data-ttu-id="82682-115">String</span><span class="sxs-lookup"><span data-stu-id="82682-115">String</span></span>|<span data-ttu-id="82682-116">Nome do operando de origem (o operando que está sendo testado).</span><span class="sxs-lookup"><span data-stu-id="82682-116">Name of source operand (the operand being tested).</span></span> <span data-ttu-id="82682-117">O nome do operando de origem deve corresponder a um dos nomes de atributo no objeto de origem.</span><span class="sxs-lookup"><span data-stu-id="82682-117">The source operand name must match one of the attribute names on the source object.</span></span>|
|<span data-ttu-id="82682-118">targetOperand</span><span class="sxs-lookup"><span data-stu-id="82682-118">targetOperand</span></span>|[<span data-ttu-id="82682-119">filterOperand</span><span class="sxs-lookup"><span data-stu-id="82682-119">filterOperand</span></span>](synchronization-filteroperand.md)|<span data-ttu-id="82682-120">Valores em relação ao qual o operando de origem será testado.</span><span class="sxs-lookup"><span data-stu-id="82682-120">Values that the source operand will be tested against.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="82682-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="82682-121">JSON representation</span></span>

<span data-ttu-id="82682-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="82682-122">The following is a JSON representation of the resource.</span></span>

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
