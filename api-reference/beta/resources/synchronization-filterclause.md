---
title: tipo de recurso de filterClause
description: Representa um único assertion que um objeto de candidato deve satisfazer e é avaliado para uma `true` (objeto atenda a afirmação) ou `false` (o objeto não atender a afirmação).
localization_priority: Normal
ms.openlocfilehash: 62623cee5b2991acbe162561940adb1afd3574a1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523866"
---
# <a name="filterclause-resource-type"></a><span data-ttu-id="cb5fc-103">tipo de recurso de filterClause</span><span class="sxs-lookup"><span data-stu-id="cb5fc-103">filterClause resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb5fc-104">Representa um único assertion que um objeto de candidato deve satisfazer e é avaliado para uma `true` (objeto atenda a afirmação) ou `false` (o objeto não atender a afirmação).</span><span class="sxs-lookup"><span data-stu-id="cb5fc-104">Represents a single assertion that a candidate object must satisfy, and is evaluated to either `true` (object satisfies the assertion) or `false` (object does not satisfy the assertion).</span></span>

## <a name="properties"></a><span data-ttu-id="cb5fc-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cb5fc-105">Properties</span></span>
| <span data-ttu-id="cb5fc-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb5fc-106">Property</span></span>     | <span data-ttu-id="cb5fc-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb5fc-107">Type</span></span>   |<span data-ttu-id="cb5fc-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb5fc-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb5fc-109">operatorName</span><span class="sxs-lookup"><span data-stu-id="cb5fc-109">operatorName</span></span>|<span data-ttu-id="cb5fc-110">String</span><span class="sxs-lookup"><span data-stu-id="cb5fc-110">String</span></span>|<span data-ttu-id="cb5fc-111">Nome do operador a ser aplicada à operandos de origem e destino.</span><span class="sxs-lookup"><span data-stu-id="cb5fc-111">Name of the operator to be applied to the source and target operands.</span></span> <span data-ttu-id="cb5fc-112">Deve ser um dos operadores com suporte.</span><span class="sxs-lookup"><span data-stu-id="cb5fc-112">Must be one of the supported operators.</span></span> <span data-ttu-id="cb5fc-113">Os operadores com suporte que podem ser descobertos.</span><span class="sxs-lookup"><span data-stu-id="cb5fc-113">Supported operators can be discovered.</span></span>|
|<span data-ttu-id="cb5fc-114">sourceOperandName</span><span class="sxs-lookup"><span data-stu-id="cb5fc-114">sourceOperandName</span></span>|<span data-ttu-id="cb5fc-115">String</span><span class="sxs-lookup"><span data-stu-id="cb5fc-115">String</span></span>|<span data-ttu-id="cb5fc-116">Nome do operando de origem (o operando que está sendo testado).</span><span class="sxs-lookup"><span data-stu-id="cb5fc-116">Name of source operand (the operand being tested).</span></span> <span data-ttu-id="cb5fc-117">O nome da fonte operando deve corresponder a um dos nomes de atributo no objeto de origem.</span><span class="sxs-lookup"><span data-stu-id="cb5fc-117">The source operand name must match one of the attribute names on the source object.</span></span>|
|<span data-ttu-id="cb5fc-118">targetOperand</span><span class="sxs-lookup"><span data-stu-id="cb5fc-118">targetOperand</span></span>|[<span data-ttu-id="cb5fc-119">filterOperand</span><span class="sxs-lookup"><span data-stu-id="cb5fc-119">filterOperand</span></span>](synchronization-filteroperand.md)|<span data-ttu-id="cb5fc-120">Valores que o operando de origem será testado em relação.</span><span class="sxs-lookup"><span data-stu-id="cb5fc-120">Values that the source operand will be tested against.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb5fc-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cb5fc-121">JSON representation</span></span>

<span data-ttu-id="cb5fc-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cb5fc-122">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filterclause.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
