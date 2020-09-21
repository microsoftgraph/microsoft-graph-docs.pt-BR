---
title: tipo de recurso attributeMappingParameterSchema
description: Descreve um único parâmetro usado em um attributeMappingFunctionSchema.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 32710c5411f054ad096bdd293a2f7d46e89a6944
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078071"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="832e5-103">tipo de recurso attributeMappingParameterSchema</span><span class="sxs-lookup"><span data-stu-id="832e5-103">attributeMappingParameterSchema resource type</span></span>

<span data-ttu-id="832e5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="832e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="832e5-105">Descreve um único parâmetro usado em um [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span><span class="sxs-lookup"><span data-stu-id="832e5-105">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="832e5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="832e5-106">Properties</span></span>

| <span data-ttu-id="832e5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="832e5-107">Property</span></span>                   | <span data-ttu-id="832e5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="832e5-108">Type</span></span>                      | <span data-ttu-id="832e5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="832e5-109">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="832e5-110">allowMultipleOccurrences</span><span class="sxs-lookup"><span data-stu-id="832e5-110">allowMultipleOccurrences</span></span>    |<span data-ttu-id="832e5-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="832e5-111">Boolean</span></span>                   |<span data-ttu-id="832e5-112">O parâmetro fornecido pode ser fornecido várias vezes (por exemplo, várias cadeias de caracteres de entrada na `Concatenate(string,string,...)` função).</span><span class="sxs-lookup"><span data-stu-id="832e5-112">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="832e5-113">name</span><span class="sxs-lookup"><span data-stu-id="832e5-113">name</span></span>                        |<span data-ttu-id="832e5-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="832e5-114">String</span></span>                    |<span data-ttu-id="832e5-115">Nome do parâmetro.</span><span class="sxs-lookup"><span data-stu-id="832e5-115">Parameter name.</span></span> |
|<span data-ttu-id="832e5-116">obrigatório</span><span class="sxs-lookup"><span data-stu-id="832e5-116">required</span></span>                    |<span data-ttu-id="832e5-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="832e5-117">Boolean</span></span>                   |<span data-ttu-id="832e5-118">`true` Se o parâmetro for necessário; caso contrário `false` .</span><span class="sxs-lookup"><span data-stu-id="832e5-118">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="832e5-119">tipo</span><span class="sxs-lookup"><span data-stu-id="832e5-119">type</span></span>                        |<span data-ttu-id="832e5-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="832e5-120">String</span></span>                    |<span data-ttu-id="832e5-121">Os valores possíveis são: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="832e5-121">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="832e5-122">O padrão é `String`.</span><span class="sxs-lookup"><span data-stu-id="832e5-122">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="832e5-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="832e5-123">JSON representation</span></span>

<span data-ttu-id="832e5-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="832e5-124">The following is a JSON representation of the resource.</span></span>

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


