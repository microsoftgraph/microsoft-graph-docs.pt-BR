---
title: tipo de recurso attributeMappingParameterSchema
description: Descreve um único parâmetro usado em um attributeMappingFunctionSchema.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d4415c6ece2fc9095070eb888ad4bd7bba583d54
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520237"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="d482c-103">tipo de recurso attributeMappingParameterSchema</span><span class="sxs-lookup"><span data-stu-id="d482c-103">attributeMappingParameterSchema resource type</span></span>

<span data-ttu-id="d482c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d482c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d482c-105">Descreve um único parâmetro usado em um [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span><span class="sxs-lookup"><span data-stu-id="d482c-105">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d482c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d482c-106">Properties</span></span>

| <span data-ttu-id="d482c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d482c-107">Property</span></span>                   | <span data-ttu-id="d482c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d482c-108">Type</span></span>                      | <span data-ttu-id="d482c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d482c-109">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="d482c-110">allowMultipleOccurrences</span><span class="sxs-lookup"><span data-stu-id="d482c-110">allowMultipleOccurrences</span></span>    |<span data-ttu-id="d482c-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="d482c-111">Boolean</span></span>                   |<span data-ttu-id="d482c-112">O parâmetro fornecido pode ser fornecido várias vezes (por exemplo, várias cadeias de caracteres `Concatenate(string,string,...)` de entrada na função).</span><span class="sxs-lookup"><span data-stu-id="d482c-112">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="d482c-113">nome</span><span class="sxs-lookup"><span data-stu-id="d482c-113">name</span></span>                        |<span data-ttu-id="d482c-114">String</span><span class="sxs-lookup"><span data-stu-id="d482c-114">String</span></span>                    |<span data-ttu-id="d482c-115">Nome do parâmetro.</span><span class="sxs-lookup"><span data-stu-id="d482c-115">Parameter name.</span></span> |
|<span data-ttu-id="d482c-116">obrigatório</span><span class="sxs-lookup"><span data-stu-id="d482c-116">required</span></span>                    |<span data-ttu-id="d482c-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="d482c-117">Boolean</span></span>                   |<span data-ttu-id="d482c-118">`true`Se o parâmetro for necessário; caso `false`contrário.</span><span class="sxs-lookup"><span data-stu-id="d482c-118">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="d482c-119">type</span><span class="sxs-lookup"><span data-stu-id="d482c-119">type</span></span>                        |<span data-ttu-id="d482c-120">String</span><span class="sxs-lookup"><span data-stu-id="d482c-120">String</span></span>                    |<span data-ttu-id="d482c-121">Os valores possíveis são: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="d482c-121">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="d482c-122">O padrão é `String`.</span><span class="sxs-lookup"><span data-stu-id="d482c-122">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d482c-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d482c-123">JSON representation</span></span>

<span data-ttu-id="d482c-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d482c-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingParameterSchema"
}-->

```json
{
  "allowMultipleOccurrences": "Boolean",
  "name": "String",
  "required": "Boolean",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingParameterSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
