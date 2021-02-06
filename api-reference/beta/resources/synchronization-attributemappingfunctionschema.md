---
title: Tipo de recurso attributeMappingFunctionSchema
description: Descreve uma função que pode ser usada em um mapeamento de atributos para transformar valores durante a sincronização.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: a62d2d635504208fc8266e98add66a8503e3e4d2
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128740"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="7d151-103">Tipo de recurso attributeMappingFunctionSchema</span><span class="sxs-lookup"><span data-stu-id="7d151-103">attributeMappingFunctionSchema resource type</span></span>

<span data-ttu-id="7d151-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d151-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d151-105">Descreve uma função que pode ser usada em um mapeamento [de atributos para](synchronization-attributemapping.md) transformar valores durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="7d151-105">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="7d151-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="7d151-106">Methods</span></span>

| <span data-ttu-id="7d151-107">Método</span><span class="sxs-lookup"><span data-stu-id="7d151-107">Method</span></span>           | <span data-ttu-id="7d151-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7d151-108">Return Type</span></span>    |<span data-ttu-id="7d151-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d151-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7d151-110">List</span><span class="sxs-lookup"><span data-stu-id="7d151-110">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="7d151-111">[Coleção attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)</span><span class="sxs-lookup"><span data-stu-id="7d151-111">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="7d151-112">Listar funções de mapeamento de atributos com suporte.</span><span class="sxs-lookup"><span data-stu-id="7d151-112">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="7d151-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7d151-113">Properties</span></span>

| <span data-ttu-id="7d151-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d151-114">Property</span></span>                   | <span data-ttu-id="7d151-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d151-115">Type</span></span>                      | <span data-ttu-id="7d151-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d151-116">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="7d151-117">nome</span><span class="sxs-lookup"><span data-stu-id="7d151-117">name</span></span>                        |<span data-ttu-id="7d151-118">String</span><span class="sxs-lookup"><span data-stu-id="7d151-118">String</span></span>                    |<span data-ttu-id="7d151-119">Nome do operador.</span><span class="sxs-lookup"><span data-stu-id="7d151-119">Operator name.</span></span> |
|<span data-ttu-id="7d151-120">parameters</span><span class="sxs-lookup"><span data-stu-id="7d151-120">parameters</span></span>                  |<span data-ttu-id="7d151-121">[Coleção attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md)</span><span class="sxs-lookup"><span data-stu-id="7d151-121">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="7d151-122">Coleção de parâmetros de função.</span><span class="sxs-lookup"><span data-stu-id="7d151-122">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7d151-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7d151-123">JSON representation</span></span>

<span data-ttu-id="7d151-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7d151-124">The following is a JSON representation of the resource.</span></span>

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


