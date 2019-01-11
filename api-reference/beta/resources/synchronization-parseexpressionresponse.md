---
title: tipo de recurso de parseExpressionResponse
description: 'Representa a resposta do [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) ação.'
localization_priority: Normal
ms.openlocfilehash: 550a46b0c27c2ca8d2d4c01baa975d8a204546f2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832945"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="0303e-103">tipo de recurso de parseExpressionResponse</span><span class="sxs-lookup"><span data-stu-id="0303e-103">parseExpressionResponse resource type</span></span>

> <span data-ttu-id="0303e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0303e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0303e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0303e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0303e-106">Representa a resposta do [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) ação.</span><span class="sxs-lookup"><span data-stu-id="0303e-106">Represents the response from the [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="0303e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0303e-107">Properties</span></span>
| <span data-ttu-id="0303e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0303e-108">Property</span></span>     | <span data-ttu-id="0303e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0303e-109">Type</span></span>   |<span data-ttu-id="0303e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0303e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0303e-111">erro</span><span class="sxs-lookup"><span data-stu-id="0303e-111">error</span></span>|<span data-ttu-id="0303e-112">OData.Error</span><span class="sxs-lookup"><span data-stu-id="0303e-112">odata.error</span></span>|<span data-ttu-id="0303e-113">Detalhes do erro, se a avaliação da expressão resultou em um erro.</span><span class="sxs-lookup"><span data-stu-id="0303e-113">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="0303e-114">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="0303e-114">evaluationResult</span></span>|<span data-ttu-id="0303e-115">String collection</span><span class="sxs-lookup"><span data-stu-id="0303e-115">String collection</span></span>|<span data-ttu-id="0303e-116">Uma coleção de valores gerados pela avaliação da expressão.</span><span class="sxs-lookup"><span data-stu-id="0303e-116">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="0303e-117">evaluationSucceeded</span><span class="sxs-lookup"><span data-stu-id="0303e-117">evaluationSucceeded</span></span>|<span data-ttu-id="0303e-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="0303e-118">Boolean</span></span>|<span data-ttu-id="0303e-119">`true`Se a avaliação foi bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="0303e-119">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="0303e-120">parsedExpression</span><span class="sxs-lookup"><span data-stu-id="0303e-120">parsedExpression</span></span>|[<span data-ttu-id="0303e-121">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="0303e-121">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="0303e-122">Um objeto de [attributeMappingSource](synchronization-attributemappingsource.md) representando a expressão analisada.</span><span class="sxs-lookup"><span data-stu-id="0303e-122">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="0303e-123">parsingSucceeded</span><span class="sxs-lookup"><span data-stu-id="0303e-123">parsingSucceeded</span></span>|<span data-ttu-id="0303e-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="0303e-124">Boolean</span></span>|<span data-ttu-id="0303e-125">`true`Se a expressão foi analisada com êxito.</span><span class="sxs-lookup"><span data-stu-id="0303e-125">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0303e-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0303e-126">JSON representation</span></span>

<span data-ttu-id="0303e-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0303e-127">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "parseExpressionResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
