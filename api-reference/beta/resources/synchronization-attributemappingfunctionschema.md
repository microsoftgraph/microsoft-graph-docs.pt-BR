---
title: tipo de recurso de attributeMappingFunctionSchema
description: Descreve uma função que pode ser usada em um mapeamento de atributo para transformar valores durante a sincronização.
localization_priority: Normal
ms.openlocfilehash: e2c0139f7c797c3f519cc638561b09f611018b28
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511979"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="0085b-103">tipo de recurso de attributeMappingFunctionSchema</span><span class="sxs-lookup"><span data-stu-id="0085b-103">attributeMappingFunctionSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0085b-104">Descreve uma função que pode ser usada em um [mapeamento de atributos](synchronization-attributemapping.md) para transformar valores durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="0085b-104">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="0085b-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="0085b-105">Methods</span></span>

| <span data-ttu-id="0085b-106">Método</span><span class="sxs-lookup"><span data-stu-id="0085b-106">Method</span></span>           | <span data-ttu-id="0085b-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0085b-107">Return Type</span></span>    |<span data-ttu-id="0085b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0085b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0085b-109">List</span><span class="sxs-lookup"><span data-stu-id="0085b-109">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="0085b-110">coleção [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)</span><span class="sxs-lookup"><span data-stu-id="0085b-110">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="0085b-111">Funções de mapeamento de atributo de lista com suporte.</span><span class="sxs-lookup"><span data-stu-id="0085b-111">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="0085b-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0085b-112">Properties</span></span>

| <span data-ttu-id="0085b-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0085b-113">Property</span></span>                   | <span data-ttu-id="0085b-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="0085b-114">Type</span></span>                      | <span data-ttu-id="0085b-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="0085b-115">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="0085b-116">name</span><span class="sxs-lookup"><span data-stu-id="0085b-116">name</span></span>                        |<span data-ttu-id="0085b-117">String</span><span class="sxs-lookup"><span data-stu-id="0085b-117">String</span></span>                    |<span data-ttu-id="0085b-118">Nome do operador.</span><span class="sxs-lookup"><span data-stu-id="0085b-118">Operator name.</span></span> |
|<span data-ttu-id="0085b-119">parâmetros</span><span class="sxs-lookup"><span data-stu-id="0085b-119">parameters</span></span>                  |<span data-ttu-id="0085b-120">coleção [attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md)</span><span class="sxs-lookup"><span data-stu-id="0085b-120">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="0085b-121">Coleção de parâmetros de função.</span><span class="sxs-lookup"><span data-stu-id="0085b-121">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0085b-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0085b-122">JSON representation</span></span>

<span data-ttu-id="0085b-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0085b-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingFunctionSchema"
}-->

```json
{
  "name": "String (identifier)",
  "parameters": [{"@odata.type": "microsoft.graph.attributeMappingParameterSchema"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingFunctionSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemappingfunctionschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
