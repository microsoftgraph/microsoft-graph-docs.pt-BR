---
title: Tipo de recurso attributeMappingParameterSchema
description: Descreve um único parâmetro usado em um atributoMappingFunctionSchema.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: c8779211382ffcf7284c5ebf4035be6134efd8bf
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128733"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="40468-103">Tipo de recurso attributeMappingParameterSchema</span><span class="sxs-lookup"><span data-stu-id="40468-103">attributeMappingParameterSchema resource type</span></span>

<span data-ttu-id="40468-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40468-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40468-105">Descreve um único parâmetro usado em um [atributoMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span><span class="sxs-lookup"><span data-stu-id="40468-105">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="40468-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="40468-106">Properties</span></span>

| <span data-ttu-id="40468-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40468-107">Property</span></span>                   | <span data-ttu-id="40468-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="40468-108">Type</span></span>                      | <span data-ttu-id="40468-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="40468-109">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="40468-110">allowMultipleOccurrences</span><span class="sxs-lookup"><span data-stu-id="40468-110">allowMultipleOccurrences</span></span>    |<span data-ttu-id="40468-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="40468-111">Boolean</span></span>                   |<span data-ttu-id="40468-112">O parâmetro fornecido pode ser fornecido várias vezes (por exemplo, várias cadeias de caracteres de entrada na `Concatenate(string,string,...)` função).</span><span class="sxs-lookup"><span data-stu-id="40468-112">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="40468-113">nome</span><span class="sxs-lookup"><span data-stu-id="40468-113">name</span></span>                        |<span data-ttu-id="40468-114">String</span><span class="sxs-lookup"><span data-stu-id="40468-114">String</span></span>                    |<span data-ttu-id="40468-115">Nome do parâmetro.</span><span class="sxs-lookup"><span data-stu-id="40468-115">Parameter name.</span></span> |
|<span data-ttu-id="40468-116">obrigatório</span><span class="sxs-lookup"><span data-stu-id="40468-116">required</span></span>                    |<span data-ttu-id="40468-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="40468-117">Boolean</span></span>                   |<span data-ttu-id="40468-118">`true` se o parâmetro for necessário; Caso `false` contrário.</span><span class="sxs-lookup"><span data-stu-id="40468-118">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="40468-119">type</span><span class="sxs-lookup"><span data-stu-id="40468-119">type</span></span>                        |<span data-ttu-id="40468-120">String</span><span class="sxs-lookup"><span data-stu-id="40468-120">String</span></span>                    |<span data-ttu-id="40468-121">Os valores possíveis são: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="40468-121">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="40468-122">O padrão é `String`.</span><span class="sxs-lookup"><span data-stu-id="40468-122">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="40468-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="40468-123">JSON representation</span></span>

<span data-ttu-id="40468-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="40468-124">The following is a JSON representation of the resource.</span></span>

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


