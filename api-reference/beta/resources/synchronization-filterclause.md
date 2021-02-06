---
title: Tipo de recurso filterClause
description: Representa uma única declaração que um objeto candidato deve satisfazer.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: fc633f6e25373713679da30a5b319ab8ae99fb04
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131919"
---
# <a name="filterclause-resource-type"></a><span data-ttu-id="38d5e-103">Tipo de recurso filterClause</span><span class="sxs-lookup"><span data-stu-id="38d5e-103">filterClause resource type</span></span>

<span data-ttu-id="38d5e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38d5e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38d5e-105">Representa uma única declaração que um objeto candidato deve satisfazer e é avaliada para (o objeto satisfaz a assarção) ou (o objeto não satisfaz `true` `false` a assarção).</span><span class="sxs-lookup"><span data-stu-id="38d5e-105">Represents a single assertion that a candidate object must satisfy, and is evaluated to either `true` (object satisfies the assertion) or `false` (object does not satisfy the assertion).</span></span>

## <a name="properties"></a><span data-ttu-id="38d5e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="38d5e-106">Properties</span></span>
| <span data-ttu-id="38d5e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38d5e-107">Property</span></span>     | <span data-ttu-id="38d5e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="38d5e-108">Type</span></span>   |<span data-ttu-id="38d5e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="38d5e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38d5e-110">operatorName</span><span class="sxs-lookup"><span data-stu-id="38d5e-110">operatorName</span></span>|<span data-ttu-id="38d5e-111">String</span><span class="sxs-lookup"><span data-stu-id="38d5e-111">String</span></span>|<span data-ttu-id="38d5e-112">Nome do operador a ser aplicado aos operadores de origem e de destino.</span><span class="sxs-lookup"><span data-stu-id="38d5e-112">Name of the operator to be applied to the source and target operands.</span></span> <span data-ttu-id="38d5e-113">Deve ser um dos operadores com suporte.</span><span class="sxs-lookup"><span data-stu-id="38d5e-113">Must be one of the supported operators.</span></span> <span data-ttu-id="38d5e-114">Os operadores com suporte podem ser descobertos.</span><span class="sxs-lookup"><span data-stu-id="38d5e-114">Supported operators can be discovered.</span></span>|
|<span data-ttu-id="38d5e-115">sourceOperandName</span><span class="sxs-lookup"><span data-stu-id="38d5e-115">sourceOperandName</span></span>|<span data-ttu-id="38d5e-116">String</span><span class="sxs-lookup"><span data-stu-id="38d5e-116">String</span></span>|<span data-ttu-id="38d5e-117">Nome do operand de origem (o operand que está sendo testado).</span><span class="sxs-lookup"><span data-stu-id="38d5e-117">Name of source operand (the operand being tested).</span></span> <span data-ttu-id="38d5e-118">O nome do operand de origem deve corresponder a um dos nomes de atributo no objeto de origem.</span><span class="sxs-lookup"><span data-stu-id="38d5e-118">The source operand name must match one of the attribute names on the source object.</span></span>|
|<span data-ttu-id="38d5e-119">targetOperand</span><span class="sxs-lookup"><span data-stu-id="38d5e-119">targetOperand</span></span>|[<span data-ttu-id="38d5e-120">filterOperand</span><span class="sxs-lookup"><span data-stu-id="38d5e-120">filterOperand</span></span>](synchronization-filteroperand.md)|<span data-ttu-id="38d5e-121">Valores que o operand de origem será testado.</span><span class="sxs-lookup"><span data-stu-id="38d5e-121">Values that the source operand will be tested against.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="38d5e-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="38d5e-122">JSON representation</span></span>

<span data-ttu-id="38d5e-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="38d5e-123">The following is a JSON representation of the resource.</span></span>

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


