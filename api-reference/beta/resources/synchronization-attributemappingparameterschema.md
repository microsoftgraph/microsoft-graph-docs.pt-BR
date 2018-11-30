---
title: tipo de recurso de attributeMappingParameterSchema
description: Descreve um único parâmetro usado em um attributeMappingFunctionSchema.
ms.openlocfilehash: 164387a345f245f390d24b89a349e02ee2242041
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039836"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="2089a-103">tipo de recurso de attributeMappingParameterSchema</span><span class="sxs-lookup"><span data-stu-id="2089a-103">attributeMappingParameterSchema resource type</span></span>

> <span data-ttu-id="2089a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2089a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2089a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2089a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2089a-106">Descreve um único parâmetro usado em um [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span><span class="sxs-lookup"><span data-stu-id="2089a-106">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2089a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2089a-107">Properties</span></span>

| <span data-ttu-id="2089a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2089a-108">Property</span></span>                   | <span data-ttu-id="2089a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2089a-109">Type</span></span>                      | <span data-ttu-id="2089a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2089a-110">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="2089a-111">allowMultipleOccurrences</span><span class="sxs-lookup"><span data-stu-id="2089a-111">allowMultipleOccurrences</span></span>    |<span data-ttu-id="2089a-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="2089a-112">Boolean</span></span>                   |<span data-ttu-id="2089a-113">O parâmetro determinado pode ser fornecido várias vezes (por exemplo, a entrada de vários strings no `Concatenate(string,string,...)` função).</span><span class="sxs-lookup"><span data-stu-id="2089a-113">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="2089a-114">name</span><span class="sxs-lookup"><span data-stu-id="2089a-114">name</span></span>                        |<span data-ttu-id="2089a-115">String</span><span class="sxs-lookup"><span data-stu-id="2089a-115">String</span></span>                    |<span data-ttu-id="2089a-116">Nome do parâmetro.</span><span class="sxs-lookup"><span data-stu-id="2089a-116">Parameter name.</span></span> |
|<span data-ttu-id="2089a-117">obrigatório</span><span class="sxs-lookup"><span data-stu-id="2089a-117">required</span></span>                    |<span data-ttu-id="2089a-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="2089a-118">Boolean</span></span>                   |<span data-ttu-id="2089a-119">`true`Se o parâmetro é obrigatório; Caso contrário, `false`.</span><span class="sxs-lookup"><span data-stu-id="2089a-119">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="2089a-120">type</span><span class="sxs-lookup"><span data-stu-id="2089a-120">type</span></span>                        |<span data-ttu-id="2089a-121">String</span><span class="sxs-lookup"><span data-stu-id="2089a-121">String</span></span>                    |<span data-ttu-id="2089a-122">Os valores possíveis são: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="2089a-122">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="2089a-123">O padrão é `String`.</span><span class="sxs-lookup"><span data-stu-id="2089a-123">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2089a-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2089a-124">JSON representation</span></span>

<span data-ttu-id="2089a-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2089a-125">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "attributeMappingParameterSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->