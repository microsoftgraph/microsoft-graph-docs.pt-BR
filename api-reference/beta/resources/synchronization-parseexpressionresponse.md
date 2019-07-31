---
title: tipo de recurso parseExpressionResponse
description: 'Representa a resposta da ação [synchronizationSchema: ParseName](../api/synchronization_synchronizationschema_parseexpression.md) .'
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a2c2bc0291eca7c04f246c6f62424b0bab10dced
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964778"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="9be56-103">tipo de recurso parseExpressionResponse</span><span class="sxs-lookup"><span data-stu-id="9be56-103">parseExpressionResponse resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9be56-104">Representa a resposta da ação [parsery](../api/synchronization-synchronizationschema-parseexpression.md) .</span><span class="sxs-lookup"><span data-stu-id="9be56-104">Represents the response from the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="9be56-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9be56-105">Properties</span></span>
| <span data-ttu-id="9be56-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9be56-106">Property</span></span>     | <span data-ttu-id="9be56-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="9be56-107">Type</span></span>   |<span data-ttu-id="9be56-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9be56-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9be56-109">erro</span><span class="sxs-lookup"><span data-stu-id="9be56-109">error</span></span>|<span data-ttu-id="9be56-110">publicError</span><span class="sxs-lookup"><span data-stu-id="9be56-110">publicError</span></span>|<span data-ttu-id="9be56-111">Detalhes do erro, se a avaliação da expressão resultar em um erro.</span><span class="sxs-lookup"><span data-stu-id="9be56-111">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="9be56-112">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="9be56-112">evaluationResult</span></span>|<span data-ttu-id="9be56-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9be56-113">String collection</span></span>|<span data-ttu-id="9be56-114">Uma coleção de valores produzidos pela avaliação da expressão.</span><span class="sxs-lookup"><span data-stu-id="9be56-114">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="9be56-115">evaluationSucceeded</span><span class="sxs-lookup"><span data-stu-id="9be56-115">evaluationSucceeded</span></span>|<span data-ttu-id="9be56-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="9be56-116">Boolean</span></span>|<span data-ttu-id="9be56-117">`true`se a avaliação tiver sido bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="9be56-117">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="9be56-118">parsedExpression</span><span class="sxs-lookup"><span data-stu-id="9be56-118">parsedExpression</span></span>|[<span data-ttu-id="9be56-119">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="9be56-119">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="9be56-120">Um objeto [attributeMappingSource](synchronization-attributemappingsource.md) que representa a expressão analisada.</span><span class="sxs-lookup"><span data-stu-id="9be56-120">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="9be56-121">parsingSucceeded</span><span class="sxs-lookup"><span data-stu-id="9be56-121">parsingSucceeded</span></span>|<span data-ttu-id="9be56-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="9be56-122">Boolean</span></span>|<span data-ttu-id="9be56-123">`true`se a expressão tiver sido analisada com êxito.</span><span class="sxs-lookup"><span data-stu-id="9be56-123">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9be56-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9be56-124">JSON representation</span></span>

<span data-ttu-id="9be56-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9be56-125">The following is a JSON representation of the resource.</span></span>

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
