---
title: tipo de recurso parseExpressionResponse
description: 'Representa a resposta da ação synchronizationSchema: ParseName.'
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9bd675b079f42856e85f54b7da84a091a0f57f4f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988811"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="e2d97-103">tipo de recurso parseExpressionResponse</span><span class="sxs-lookup"><span data-stu-id="e2d97-103">parseExpressionResponse resource type</span></span>

<span data-ttu-id="e2d97-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2d97-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2d97-105">Representa a resposta da ação [parsery](../api/synchronization-synchronizationschema-parseexpression.md) .</span><span class="sxs-lookup"><span data-stu-id="e2d97-105">Represents the response from the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="e2d97-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2d97-106">Properties</span></span>
| <span data-ttu-id="e2d97-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2d97-107">Property</span></span>     | <span data-ttu-id="e2d97-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2d97-108">Type</span></span>   |<span data-ttu-id="e2d97-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2d97-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2d97-110">erro</span><span class="sxs-lookup"><span data-stu-id="e2d97-110">error</span></span>|<span data-ttu-id="e2d97-111">publicError</span><span class="sxs-lookup"><span data-stu-id="e2d97-111">publicError</span></span>|<span data-ttu-id="e2d97-112">Detalhes do erro, se a avaliação da expressão resultar em um erro.</span><span class="sxs-lookup"><span data-stu-id="e2d97-112">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="e2d97-113">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="e2d97-113">evaluationResult</span></span>|<span data-ttu-id="e2d97-114">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2d97-114">String collection</span></span>|<span data-ttu-id="e2d97-115">Uma coleção de valores produzidos pela avaliação da expressão.</span><span class="sxs-lookup"><span data-stu-id="e2d97-115">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="e2d97-116">evaluationSucceeded</span><span class="sxs-lookup"><span data-stu-id="e2d97-116">evaluationSucceeded</span></span>|<span data-ttu-id="e2d97-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2d97-117">Boolean</span></span>|<span data-ttu-id="e2d97-118">`true` se a avaliação tiver sido bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="e2d97-118">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="e2d97-119">parsedExpression</span><span class="sxs-lookup"><span data-stu-id="e2d97-119">parsedExpression</span></span>|[<span data-ttu-id="e2d97-120">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="e2d97-120">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="e2d97-121">Um objeto [attributeMappingSource](synchronization-attributemappingsource.md) que representa a expressão analisada.</span><span class="sxs-lookup"><span data-stu-id="e2d97-121">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="e2d97-122">parsingSucceeded</span><span class="sxs-lookup"><span data-stu-id="e2d97-122">parsingSucceeded</span></span>|<span data-ttu-id="e2d97-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2d97-123">Boolean</span></span>|<span data-ttu-id="e2d97-124">`true` se a expressão tiver sido analisada com êxito.</span><span class="sxs-lookup"><span data-stu-id="e2d97-124">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2d97-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2d97-125">JSON representation</span></span>

<span data-ttu-id="e2d97-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e2d97-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.parseExpressionResponse"
}-->

```json
{
  "error": {"@odata.type": "microsoft.graph.publicError"},
  "evaluationResult": ["String"],
  "evaluationSucceeded": true,
  "parsedExpression": {"@odata.type": "microsoft.graph.attributeMappingSource"},
  "parsingSucceeded": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "parseExpressionResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


