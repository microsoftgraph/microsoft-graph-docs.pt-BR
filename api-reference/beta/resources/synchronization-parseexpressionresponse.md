---
title: Tipo de recurso parseExpressionResponse
description: 'Representa a resposta da ação synchronizationSchema: parseExpression.'
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: e564cb2ad7a80c91fec7d6298254fa19bde4537c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133144"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="11a04-103">Tipo de recurso parseExpressionResponse</span><span class="sxs-lookup"><span data-stu-id="11a04-103">parseExpressionResponse resource type</span></span>

<span data-ttu-id="11a04-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11a04-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11a04-105">Representa a resposta da [ação parseExpression.](../api/synchronization-synchronizationschema-parseexpression.md)</span><span class="sxs-lookup"><span data-stu-id="11a04-105">Represents the response from the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="11a04-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11a04-106">Properties</span></span>
| <span data-ttu-id="11a04-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11a04-107">Property</span></span>     | <span data-ttu-id="11a04-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="11a04-108">Type</span></span>   |<span data-ttu-id="11a04-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="11a04-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11a04-110">erro</span><span class="sxs-lookup"><span data-stu-id="11a04-110">error</span></span>|<span data-ttu-id="11a04-111">publicError</span><span class="sxs-lookup"><span data-stu-id="11a04-111">publicError</span></span>|<span data-ttu-id="11a04-112">Detalhes do erro, se a avaliação de expressão tiver resultado em um erro.</span><span class="sxs-lookup"><span data-stu-id="11a04-112">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="11a04-113">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="11a04-113">evaluationResult</span></span>|<span data-ttu-id="11a04-114">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="11a04-114">String collection</span></span>|<span data-ttu-id="11a04-115">Uma coleção de valores produzidos pela avaliação da expressão.</span><span class="sxs-lookup"><span data-stu-id="11a04-115">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="11a04-116">evaluationSucceeded</span><span class="sxs-lookup"><span data-stu-id="11a04-116">evaluationSucceeded</span></span>|<span data-ttu-id="11a04-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="11a04-117">Boolean</span></span>|<span data-ttu-id="11a04-118">`true` se a avaliação foi bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="11a04-118">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="11a04-119">parsedExpression</span><span class="sxs-lookup"><span data-stu-id="11a04-119">parsedExpression</span></span>|[<span data-ttu-id="11a04-120">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="11a04-120">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="11a04-121">Um [objeto attributeMappingSource](synchronization-attributemappingsource.md) que representa a expressão analisado.</span><span class="sxs-lookup"><span data-stu-id="11a04-121">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="11a04-122">parsingSucceeded</span><span class="sxs-lookup"><span data-stu-id="11a04-122">parsingSucceeded</span></span>|<span data-ttu-id="11a04-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="11a04-123">Boolean</span></span>|<span data-ttu-id="11a04-124">`true` se a expressão foi analisado com êxito.</span><span class="sxs-lookup"><span data-stu-id="11a04-124">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11a04-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11a04-125">JSON representation</span></span>

<span data-ttu-id="11a04-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="11a04-126">The following is a JSON representation of the resource.</span></span>

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


