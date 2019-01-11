---
title: tipo de recurso de filterClause
description: Representa um único assertion que um objeto de candidato deve satisfazer e é avaliado para uma `true` (objeto atenda a afirmação) ou `false` (o objeto não atender a afirmação).
localization_priority: Normal
ms.openlocfilehash: 89807a6086f661388c8d5b1d5f82bfe973c3af39
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833856"
---
# <a name="filterclause-resource-type"></a><span data-ttu-id="c1026-103">tipo de recurso de filterClause</span><span class="sxs-lookup"><span data-stu-id="c1026-103">filterClause resource type</span></span>

> <span data-ttu-id="c1026-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c1026-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1026-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c1026-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c1026-106">Representa um único assertion que um objeto de candidato deve satisfazer e é avaliado para uma `true` (objeto atenda a afirmação) ou `false` (o objeto não atender a afirmação).</span><span class="sxs-lookup"><span data-stu-id="c1026-106">Represents a single assertion that a candidate object must satisfy, and is evaluated to either `true` (object satisfies the assertion) or `false` (object does not satisfy the assertion).</span></span>

## <a name="properties"></a><span data-ttu-id="c1026-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c1026-107">Properties</span></span>
| <span data-ttu-id="c1026-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1026-108">Property</span></span>     | <span data-ttu-id="c1026-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1026-109">Type</span></span>   |<span data-ttu-id="c1026-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1026-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1026-111">operatorName</span><span class="sxs-lookup"><span data-stu-id="c1026-111">operatorName</span></span>|<span data-ttu-id="c1026-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1026-112">String</span></span>|<span data-ttu-id="c1026-113">Nome do operador a ser aplicada à operandos de origem e destino.</span><span class="sxs-lookup"><span data-stu-id="c1026-113">Name of the operator to be applied to the source and target operands.</span></span> <span data-ttu-id="c1026-114">Deve ser um dos operadores com suporte.</span><span class="sxs-lookup"><span data-stu-id="c1026-114">Must be one of the supported operators.</span></span> <span data-ttu-id="c1026-115">Os operadores com suporte que podem ser descobertos.</span><span class="sxs-lookup"><span data-stu-id="c1026-115">Supported operators can be discovered.</span></span>|
|<span data-ttu-id="c1026-116">sourceOperandName</span><span class="sxs-lookup"><span data-stu-id="c1026-116">sourceOperandName</span></span>|<span data-ttu-id="c1026-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1026-117">String</span></span>|<span data-ttu-id="c1026-118">Nome do operando de origem (o operando que está sendo testado).</span><span class="sxs-lookup"><span data-stu-id="c1026-118">Name of source operand (the operand being tested).</span></span> <span data-ttu-id="c1026-119">O nome da fonte operando deve corresponder a um dos nomes de atributo no objeto de origem.</span><span class="sxs-lookup"><span data-stu-id="c1026-119">The source operand name must match one of the attribute names on the source object.</span></span>|
|<span data-ttu-id="c1026-120">targetOperand</span><span class="sxs-lookup"><span data-stu-id="c1026-120">targetOperand</span></span>|[<span data-ttu-id="c1026-121">filterOperand</span><span class="sxs-lookup"><span data-stu-id="c1026-121">filterOperand</span></span>](synchronization-filteroperand.md)|<span data-ttu-id="c1026-122">Valores que o operando de origem será testado em relação.</span><span class="sxs-lookup"><span data-stu-id="c1026-122">Values that the source operand will be tested against.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c1026-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c1026-123">JSON representation</span></span>

<span data-ttu-id="c1026-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c1026-124">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "filterClause resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
