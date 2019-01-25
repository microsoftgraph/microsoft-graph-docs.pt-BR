---
title: tipo de recurso de attributeMappingParameterSchema
description: Descreve um único parâmetro usado em um attributeMappingFunctionSchema.
localization_priority: Normal
ms.openlocfilehash: bad88fc58dcc529f086a3e3870e0bb10a9d23329
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529947"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="b8c5e-103">tipo de recurso de attributeMappingParameterSchema</span><span class="sxs-lookup"><span data-stu-id="b8c5e-103">attributeMappingParameterSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8c5e-104">Descreve um único parâmetro usado em um [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span><span class="sxs-lookup"><span data-stu-id="b8c5e-104">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b8c5e-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b8c5e-105">Properties</span></span>

| <span data-ttu-id="b8c5e-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8c5e-106">Property</span></span>                   | <span data-ttu-id="b8c5e-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8c5e-107">Type</span></span>                      | <span data-ttu-id="b8c5e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8c5e-108">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="b8c5e-109">allowMultipleOccurrences</span><span class="sxs-lookup"><span data-stu-id="b8c5e-109">allowMultipleOccurrences</span></span>    |<span data-ttu-id="b8c5e-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="b8c5e-110">Boolean</span></span>                   |<span data-ttu-id="b8c5e-111">O parâmetro determinado pode ser fornecido várias vezes (por exemplo, a entrada de vários strings no `Concatenate(string,string,...)` função).</span><span class="sxs-lookup"><span data-stu-id="b8c5e-111">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="b8c5e-112">name</span><span class="sxs-lookup"><span data-stu-id="b8c5e-112">name</span></span>                        |<span data-ttu-id="b8c5e-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8c5e-113">String</span></span>                    |<span data-ttu-id="b8c5e-114">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="b8c5e-114">Parameter name.</span></span> |
|<span data-ttu-id="b8c5e-115">obrigatório</span><span class="sxs-lookup"><span data-stu-id="b8c5e-115">required</span></span>                    |<span data-ttu-id="b8c5e-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="b8c5e-116">Boolean</span></span>                   |<span data-ttu-id="b8c5e-117">`true`Se o parâmetro é obrigatório; Caso contrário, `false`.</span><span class="sxs-lookup"><span data-stu-id="b8c5e-117">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="b8c5e-118">type</span><span class="sxs-lookup"><span data-stu-id="b8c5e-118">type</span></span>                        |<span data-ttu-id="b8c5e-119">String</span><span class="sxs-lookup"><span data-stu-id="b8c5e-119">String</span></span>                    |<span data-ttu-id="b8c5e-120">Os valores possíveis são: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="b8c5e-120">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="b8c5e-121">O padrão é `String`.</span><span class="sxs-lookup"><span data-stu-id="b8c5e-121">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8c5e-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b8c5e-122">JSON representation</span></span>

<span data-ttu-id="b8c5e-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b8c5e-123">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemappingparameterschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
