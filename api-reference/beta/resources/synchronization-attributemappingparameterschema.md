---
title: tipo de recurso attributeMappingParameterSchema
description: Descreve um único parâmetro usado em um attributeMappingFunctionSchema.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d8624851d37f475df66ec51f1951ebbbe1ea97a8
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620264"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="6e110-103">tipo de recurso attributeMappingParameterSchema</span><span class="sxs-lookup"><span data-stu-id="6e110-103">attributeMappingParameterSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e110-104">Descreve um único parâmetro usado em um [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span><span class="sxs-lookup"><span data-stu-id="6e110-104">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6e110-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e110-105">Properties</span></span>

| <span data-ttu-id="6e110-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e110-106">Property</span></span>                   | <span data-ttu-id="6e110-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e110-107">Type</span></span>                      | <span data-ttu-id="6e110-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e110-108">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="6e110-109">allowMultipleOccurrences</span><span class="sxs-lookup"><span data-stu-id="6e110-109">allowMultipleOccurrences</span></span>    |<span data-ttu-id="6e110-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="6e110-110">Boolean</span></span>                   |<span data-ttu-id="6e110-111">O parâmetro fornecido pode ser fornecido várias vezes (por exemplo, várias cadeias de caracteres `Concatenate(string,string,...)` de entrada na função).</span><span class="sxs-lookup"><span data-stu-id="6e110-111">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="6e110-112">name</span><span class="sxs-lookup"><span data-stu-id="6e110-112">name</span></span>                        |<span data-ttu-id="6e110-113">String</span><span class="sxs-lookup"><span data-stu-id="6e110-113">String</span></span>                    |<span data-ttu-id="6e110-114">Nome do parâmetro.</span><span class="sxs-lookup"><span data-stu-id="6e110-114">Parameter name.</span></span> |
|<span data-ttu-id="6e110-115">obrigatório</span><span class="sxs-lookup"><span data-stu-id="6e110-115">required</span></span>                    |<span data-ttu-id="6e110-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="6e110-116">Boolean</span></span>                   |<span data-ttu-id="6e110-117">`true`Se o parâmetro for necessário; caso `false`contrário.</span><span class="sxs-lookup"><span data-stu-id="6e110-117">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="6e110-118">type</span><span class="sxs-lookup"><span data-stu-id="6e110-118">type</span></span>                        |<span data-ttu-id="6e110-119">String</span><span class="sxs-lookup"><span data-stu-id="6e110-119">String</span></span>                    |<span data-ttu-id="6e110-120">Os valores possíveis são: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="6e110-120">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="6e110-121">O padrão é `String`.</span><span class="sxs-lookup"><span data-stu-id="6e110-121">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6e110-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e110-122">JSON representation</span></span>

<span data-ttu-id="6e110-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6e110-123">The following is a JSON representation of the resource.</span></span>

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
