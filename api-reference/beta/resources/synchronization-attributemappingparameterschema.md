---
title: tipo de recurso attributeMappingParameterSchema
description: Descreve um único parâmetro usado em um attributeMappingFunctionSchema.
localization_priority: Normal
ms.openlocfilehash: 44234e7e76b5b0d0fb514366be6106c8177b56db
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342912"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="a160b-103">tipo de recurso attributeMappingParameterSchema</span><span class="sxs-lookup"><span data-stu-id="a160b-103">attributeMappingParameterSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a160b-104">Descreve um único parâmetro usado em um [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span><span class="sxs-lookup"><span data-stu-id="a160b-104">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a160b-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a160b-105">Properties</span></span>

| <span data-ttu-id="a160b-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a160b-106">Property</span></span>                   | <span data-ttu-id="a160b-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a160b-107">Type</span></span>                      | <span data-ttu-id="a160b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a160b-108">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="a160b-109">allowMultipleOccurrences</span><span class="sxs-lookup"><span data-stu-id="a160b-109">allowMultipleOccurrences</span></span>    |<span data-ttu-id="a160b-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="a160b-110">Boolean</span></span>                   |<span data-ttu-id="a160b-111">O parâmetro fornecido pode ser fornecido várias vezes (por exemplo, várias cadeias de caracteres `Concatenate(string,string,...)` de entrada na função).</span><span class="sxs-lookup"><span data-stu-id="a160b-111">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="a160b-112">name</span><span class="sxs-lookup"><span data-stu-id="a160b-112">name</span></span>                        |<span data-ttu-id="a160b-113">String</span><span class="sxs-lookup"><span data-stu-id="a160b-113">String</span></span>                    |<span data-ttu-id="a160b-114">Nome do parâmetro.</span><span class="sxs-lookup"><span data-stu-id="a160b-114">Parameter name.</span></span> |
|<span data-ttu-id="a160b-115">obrigatório</span><span class="sxs-lookup"><span data-stu-id="a160b-115">required</span></span>                    |<span data-ttu-id="a160b-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="a160b-116">Boolean</span></span>                   |<span data-ttu-id="a160b-117">`true`Se o parâmetro for necessário; caso `false`contrário.</span><span class="sxs-lookup"><span data-stu-id="a160b-117">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="a160b-118">type</span><span class="sxs-lookup"><span data-stu-id="a160b-118">type</span></span>                        |<span data-ttu-id="a160b-119">String</span><span class="sxs-lookup"><span data-stu-id="a160b-119">String</span></span>                    |<span data-ttu-id="a160b-120">Os valores possíveis são: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="a160b-120">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="a160b-121">O padrão é `String`.</span><span class="sxs-lookup"><span data-stu-id="a160b-121">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a160b-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a160b-122">JSON representation</span></span>

<span data-ttu-id="a160b-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a160b-123">The following is a JSON representation of the resource.</span></span>

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
