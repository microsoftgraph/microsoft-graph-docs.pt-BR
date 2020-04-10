---
title: tipo de recurso attributeMappingParameterSchema
description: Descreve um único parâmetro usado em um attributeMappingFunctionSchema.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 12f1a38340b4c341d65930000c22a6cd2daeb567
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219169"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="7475e-103">tipo de recurso attributeMappingParameterSchema</span><span class="sxs-lookup"><span data-stu-id="7475e-103">attributeMappingParameterSchema resource type</span></span>

<span data-ttu-id="7475e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7475e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7475e-105">Descreve um único parâmetro usado em um [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span><span class="sxs-lookup"><span data-stu-id="7475e-105">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7475e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7475e-106">Properties</span></span>

| <span data-ttu-id="7475e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7475e-107">Property</span></span>                   | <span data-ttu-id="7475e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7475e-108">Type</span></span>                      | <span data-ttu-id="7475e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7475e-109">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="7475e-110">allowMultipleOccurrences</span><span class="sxs-lookup"><span data-stu-id="7475e-110">allowMultipleOccurrences</span></span>    |<span data-ttu-id="7475e-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="7475e-111">Boolean</span></span>                   |<span data-ttu-id="7475e-112">O parâmetro fornecido pode ser fornecido várias vezes (por exemplo, várias cadeias de caracteres `Concatenate(string,string,...)` de entrada na função).</span><span class="sxs-lookup"><span data-stu-id="7475e-112">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="7475e-113">nome</span><span class="sxs-lookup"><span data-stu-id="7475e-113">name</span></span>                        |<span data-ttu-id="7475e-114">String</span><span class="sxs-lookup"><span data-stu-id="7475e-114">String</span></span>                    |<span data-ttu-id="7475e-115">Nome do parâmetro.</span><span class="sxs-lookup"><span data-stu-id="7475e-115">Parameter name.</span></span> |
|<span data-ttu-id="7475e-116">obrigatório</span><span class="sxs-lookup"><span data-stu-id="7475e-116">required</span></span>                    |<span data-ttu-id="7475e-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="7475e-117">Boolean</span></span>                   |<span data-ttu-id="7475e-118">`true`Se o parâmetro for necessário; caso `false`contrário.</span><span class="sxs-lookup"><span data-stu-id="7475e-118">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="7475e-119">tipo</span><span class="sxs-lookup"><span data-stu-id="7475e-119">type</span></span>                        |<span data-ttu-id="7475e-120">String</span><span class="sxs-lookup"><span data-stu-id="7475e-120">String</span></span>                    |<span data-ttu-id="7475e-121">Os valores possíveis são: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="7475e-121">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="7475e-122">O padrão é `String`.</span><span class="sxs-lookup"><span data-stu-id="7475e-122">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7475e-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7475e-123">JSON representation</span></span>

<span data-ttu-id="7475e-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7475e-124">The following is a JSON representation of the resource.</span></span>

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
