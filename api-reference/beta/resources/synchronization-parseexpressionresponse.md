---
title: tipo de recurso parseExpressionResponse
description: 'Representa a resposta da ação [synchronizationSchema: ParseName](../api/synchronization_synchronizationschema_parseexpression.md) .'
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c752d5c021418dd4a3154a539a61c6ab3bae8a61
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520132"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="17a6e-103">tipo de recurso parseExpressionResponse</span><span class="sxs-lookup"><span data-stu-id="17a6e-103">parseExpressionResponse resource type</span></span>

<span data-ttu-id="17a6e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="17a6e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17a6e-105">Representa a resposta da ação [parsery](../api/synchronization-synchronizationschema-parseexpression.md) .</span><span class="sxs-lookup"><span data-stu-id="17a6e-105">Represents the response from the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="17a6e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="17a6e-106">Properties</span></span>
| <span data-ttu-id="17a6e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17a6e-107">Property</span></span>     | <span data-ttu-id="17a6e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="17a6e-108">Type</span></span>   |<span data-ttu-id="17a6e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="17a6e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17a6e-110">erro</span><span class="sxs-lookup"><span data-stu-id="17a6e-110">error</span></span>|<span data-ttu-id="17a6e-111">publicError</span><span class="sxs-lookup"><span data-stu-id="17a6e-111">publicError</span></span>|<span data-ttu-id="17a6e-112">Detalhes do erro, se a avaliação da expressão resultar em um erro.</span><span class="sxs-lookup"><span data-stu-id="17a6e-112">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="17a6e-113">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="17a6e-113">evaluationResult</span></span>|<span data-ttu-id="17a6e-114">String collection</span><span class="sxs-lookup"><span data-stu-id="17a6e-114">String collection</span></span>|<span data-ttu-id="17a6e-115">Uma coleção de valores produzidos pela avaliação da expressão.</span><span class="sxs-lookup"><span data-stu-id="17a6e-115">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="17a6e-116">evaluationSucceeded</span><span class="sxs-lookup"><span data-stu-id="17a6e-116">evaluationSucceeded</span></span>|<span data-ttu-id="17a6e-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="17a6e-117">Boolean</span></span>|<span data-ttu-id="17a6e-118">`true`se a avaliação tiver sido bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="17a6e-118">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="17a6e-119">parsedExpression</span><span class="sxs-lookup"><span data-stu-id="17a6e-119">parsedExpression</span></span>|[<span data-ttu-id="17a6e-120">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="17a6e-120">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="17a6e-121">Um objeto [attributeMappingSource](synchronization-attributemappingsource.md) que representa a expressão analisada.</span><span class="sxs-lookup"><span data-stu-id="17a6e-121">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="17a6e-122">parsingSucceeded</span><span class="sxs-lookup"><span data-stu-id="17a6e-122">parsingSucceeded</span></span>|<span data-ttu-id="17a6e-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="17a6e-123">Boolean</span></span>|<span data-ttu-id="17a6e-124">`true`se a expressão tiver sido analisada com êxito.</span><span class="sxs-lookup"><span data-stu-id="17a6e-124">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="17a6e-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="17a6e-125">JSON representation</span></span>

<span data-ttu-id="17a6e-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="17a6e-126">The following is a JSON representation of the resource.</span></span>

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
