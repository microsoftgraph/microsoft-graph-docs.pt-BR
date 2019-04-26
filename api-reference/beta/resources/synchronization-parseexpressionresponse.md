---
title: tipo de recurso parseExpressionResponse
description: 'Representa a resposta da ação [synchronizationSchema: ParseName](../api/synchronization_synchronizationschema_parseexpression.md) .'
localization_priority: Normal
ms.openlocfilehash: 14fcce13d2e78b99a8712c51768e6a94928fa07f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345534"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="03b32-103">tipo de recurso parseExpressionResponse</span><span class="sxs-lookup"><span data-stu-id="03b32-103">parseExpressionResponse resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03b32-104">Representa a resposta da ação [parsery](../api/synchronization-synchronizationschema-parseexpression.md) .</span><span class="sxs-lookup"><span data-stu-id="03b32-104">Represents the response from the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="03b32-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="03b32-105">Properties</span></span>
| <span data-ttu-id="03b32-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03b32-106">Property</span></span>     | <span data-ttu-id="03b32-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="03b32-107">Type</span></span>   |<span data-ttu-id="03b32-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="03b32-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03b32-109">erro</span><span class="sxs-lookup"><span data-stu-id="03b32-109">error</span></span>|<span data-ttu-id="03b32-110">publicError</span><span class="sxs-lookup"><span data-stu-id="03b32-110">publicError</span></span>|<span data-ttu-id="03b32-111">Detalhes do erro, se a avaliação da expressão resultar em um erro.</span><span class="sxs-lookup"><span data-stu-id="03b32-111">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="03b32-112">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="03b32-112">evaluationResult</span></span>|<span data-ttu-id="03b32-113">Coleção String</span><span class="sxs-lookup"><span data-stu-id="03b32-113">String collection</span></span>|<span data-ttu-id="03b32-114">Uma coleção de valores produzidos pela avaliação da expressão.</span><span class="sxs-lookup"><span data-stu-id="03b32-114">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="03b32-115">evaluationSucceeded</span><span class="sxs-lookup"><span data-stu-id="03b32-115">evaluationSucceeded</span></span>|<span data-ttu-id="03b32-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="03b32-116">Boolean</span></span>|<span data-ttu-id="03b32-117">`true`se a avaliação tiver sido bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="03b32-117">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="03b32-118">parsedExpression</span><span class="sxs-lookup"><span data-stu-id="03b32-118">parsedExpression</span></span>|[<span data-ttu-id="03b32-119">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="03b32-119">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="03b32-120">Um objeto [attributeMappingSource](synchronization-attributemappingsource.md) que representa a expressão analisada.</span><span class="sxs-lookup"><span data-stu-id="03b32-120">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="03b32-121">parsingSucceeded</span><span class="sxs-lookup"><span data-stu-id="03b32-121">parsingSucceeded</span></span>|<span data-ttu-id="03b32-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="03b32-122">Boolean</span></span>|<span data-ttu-id="03b32-123">`true`se a expressão tiver sido analisada com êxito.</span><span class="sxs-lookup"><span data-stu-id="03b32-123">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="03b32-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="03b32-124">JSON representation</span></span>

<span data-ttu-id="03b32-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="03b32-125">The following is a JSON representation of the resource.</span></span>

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
