---
title: tipo de recurso attributeMappingFunctionSchema
description: Descreve uma função que pode ser usada em um mapeamento de atributo para transformar valores durante a sincronização.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 16dae5dca65b3d238c2d12fddc2b474e7e03ac0d
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219176"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="36db6-103">tipo de recurso attributeMappingFunctionSchema</span><span class="sxs-lookup"><span data-stu-id="36db6-103">attributeMappingFunctionSchema resource type</span></span>

<span data-ttu-id="36db6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36db6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36db6-105">Descreve uma função que pode ser usada em um [mapeamento de atributo](synchronization-attributemapping.md) para transformar valores durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="36db6-105">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="36db6-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="36db6-106">Methods</span></span>

| <span data-ttu-id="36db6-107">Método</span><span class="sxs-lookup"><span data-stu-id="36db6-107">Method</span></span>           | <span data-ttu-id="36db6-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="36db6-108">Return Type</span></span>    |<span data-ttu-id="36db6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="36db6-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="36db6-110">List</span><span class="sxs-lookup"><span data-stu-id="36db6-110">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="36db6-111">coleção [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)</span><span class="sxs-lookup"><span data-stu-id="36db6-111">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="36db6-112">Listar funções de mapeamento de atributos com suporte.</span><span class="sxs-lookup"><span data-stu-id="36db6-112">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="36db6-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="36db6-113">Properties</span></span>

| <span data-ttu-id="36db6-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36db6-114">Property</span></span>                   | <span data-ttu-id="36db6-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="36db6-115">Type</span></span>                      | <span data-ttu-id="36db6-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="36db6-116">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="36db6-117">nome</span><span class="sxs-lookup"><span data-stu-id="36db6-117">name</span></span>                        |<span data-ttu-id="36db6-118">String</span><span class="sxs-lookup"><span data-stu-id="36db6-118">String</span></span>                    |<span data-ttu-id="36db6-119">Nome do operador.</span><span class="sxs-lookup"><span data-stu-id="36db6-119">Operator name.</span></span> |
|<span data-ttu-id="36db6-120">parameters</span><span class="sxs-lookup"><span data-stu-id="36db6-120">parameters</span></span>                  |<span data-ttu-id="36db6-121">coleção [attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md)</span><span class="sxs-lookup"><span data-stu-id="36db6-121">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="36db6-122">Conjunto de parâmetros de função.</span><span class="sxs-lookup"><span data-stu-id="36db6-122">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="36db6-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="36db6-123">JSON representation</span></span>

<span data-ttu-id="36db6-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="36db6-124">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
