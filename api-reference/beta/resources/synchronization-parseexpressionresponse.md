---
title: tipo de recurso de parseExpressionResponse
description: 'Representa a resposta do [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) ação.'
localization_priority: Normal
ms.openlocfilehash: f8ea708468e1e580693b2bd0e6f0e7f3494996f0
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641054"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="50c03-103">tipo de recurso de parseExpressionResponse</span><span class="sxs-lookup"><span data-stu-id="50c03-103">parseExpressionResponse resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50c03-104">Representa a resposta do [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) ação.</span><span class="sxs-lookup"><span data-stu-id="50c03-104">Represents the response from the [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="50c03-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50c03-105">Properties</span></span>
| <span data-ttu-id="50c03-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50c03-106">Property</span></span>     | <span data-ttu-id="50c03-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="50c03-107">Type</span></span>   |<span data-ttu-id="50c03-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="50c03-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50c03-109">erro</span><span class="sxs-lookup"><span data-stu-id="50c03-109">error</span></span>|<span data-ttu-id="50c03-110">OData.Error</span><span class="sxs-lookup"><span data-stu-id="50c03-110">odata.error</span></span>|<span data-ttu-id="50c03-111">Detalhes do erro, se a avaliação da expressão resultou em um erro.</span><span class="sxs-lookup"><span data-stu-id="50c03-111">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="50c03-112">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="50c03-112">evaluationResult</span></span>|<span data-ttu-id="50c03-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="50c03-113">String collection</span></span>|<span data-ttu-id="50c03-114">Uma coleção de valores gerados pela avaliação da expressão.</span><span class="sxs-lookup"><span data-stu-id="50c03-114">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="50c03-115">evaluationSucceeded</span><span class="sxs-lookup"><span data-stu-id="50c03-115">evaluationSucceeded</span></span>|<span data-ttu-id="50c03-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="50c03-116">Boolean</span></span>|<span data-ttu-id="50c03-117">`true`Se a avaliação foi bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="50c03-117">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="50c03-118">parsedExpression</span><span class="sxs-lookup"><span data-stu-id="50c03-118">parsedExpression</span></span>|[<span data-ttu-id="50c03-119">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="50c03-119">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="50c03-120">Um objeto de [attributeMappingSource](synchronization-attributemappingsource.md) representando a expressão analisada.</span><span class="sxs-lookup"><span data-stu-id="50c03-120">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="50c03-121">parsingSucceeded</span><span class="sxs-lookup"><span data-stu-id="50c03-121">parsingSucceeded</span></span>|<span data-ttu-id="50c03-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="50c03-122">Boolean</span></span>|<span data-ttu-id="50c03-123">`true`Se a expressão foi analisada com êxito.</span><span class="sxs-lookup"><span data-stu-id="50c03-123">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50c03-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50c03-124">JSON representation</span></span>

<span data-ttu-id="50c03-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="50c03-125">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-parseexpressionresponse.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
