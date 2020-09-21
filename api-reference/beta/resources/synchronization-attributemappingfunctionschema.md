---
title: tipo de recurso attributeMappingFunctionSchema
description: Descreve uma função que pode ser usada em um mapeamento de atributo para transformar valores durante a sincronização.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0b655d9cfac5835f6887c54c5a6bcbf79887d586
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078070"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="07390-103">tipo de recurso attributeMappingFunctionSchema</span><span class="sxs-lookup"><span data-stu-id="07390-103">attributeMappingFunctionSchema resource type</span></span>

<span data-ttu-id="07390-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07390-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07390-105">Descreve uma função que pode ser usada em um [mapeamento de atributo](synchronization-attributemapping.md) para transformar valores durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="07390-105">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="07390-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="07390-106">Methods</span></span>

| <span data-ttu-id="07390-107">Método</span><span class="sxs-lookup"><span data-stu-id="07390-107">Method</span></span>           | <span data-ttu-id="07390-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="07390-108">Return Type</span></span>    |<span data-ttu-id="07390-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="07390-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="07390-110">List</span><span class="sxs-lookup"><span data-stu-id="07390-110">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="07390-111">coleção [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)</span><span class="sxs-lookup"><span data-stu-id="07390-111">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="07390-112">Listar funções de mapeamento de atributos com suporte.</span><span class="sxs-lookup"><span data-stu-id="07390-112">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="07390-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="07390-113">Properties</span></span>

| <span data-ttu-id="07390-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07390-114">Property</span></span>                   | <span data-ttu-id="07390-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="07390-115">Type</span></span>                      | <span data-ttu-id="07390-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="07390-116">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="07390-117">name</span><span class="sxs-lookup"><span data-stu-id="07390-117">name</span></span>                        |<span data-ttu-id="07390-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07390-118">String</span></span>                    |<span data-ttu-id="07390-119">Nome do operador.</span><span class="sxs-lookup"><span data-stu-id="07390-119">Operator name.</span></span> |
|<span data-ttu-id="07390-120">parameters</span><span class="sxs-lookup"><span data-stu-id="07390-120">parameters</span></span>                  |<span data-ttu-id="07390-121">coleção [attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md)</span><span class="sxs-lookup"><span data-stu-id="07390-121">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="07390-122">Conjunto de parâmetros de função.</span><span class="sxs-lookup"><span data-stu-id="07390-122">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="07390-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07390-123">JSON representation</span></span>

<span data-ttu-id="07390-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="07390-124">The following is a JSON representation of the resource.</span></span>

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


