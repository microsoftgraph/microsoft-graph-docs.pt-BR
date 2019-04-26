---
title: tipo de recurso attributeMappingFunctionSchema
description: Descreve uma função que pode ser usada em um mapeamento de atributo para transformar valores durante a sincronização.
localization_priority: Normal
ms.openlocfilehash: ca66baf7fbc160cd4c57cba0f865ae07de9d5932
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345617"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="14eb0-103">tipo de recurso attributeMappingFunctionSchema</span><span class="sxs-lookup"><span data-stu-id="14eb0-103">attributeMappingFunctionSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14eb0-104">Descreve uma função que pode ser usada em um [mapeamento de atributo](synchronization-attributemapping.md) para transformar valores durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="14eb0-104">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="14eb0-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="14eb0-105">Methods</span></span>

| <span data-ttu-id="14eb0-106">Método</span><span class="sxs-lookup"><span data-stu-id="14eb0-106">Method</span></span>           | <span data-ttu-id="14eb0-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="14eb0-107">Return Type</span></span>    |<span data-ttu-id="14eb0-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="14eb0-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="14eb0-109">List</span><span class="sxs-lookup"><span data-stu-id="14eb0-109">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="14eb0-110">coleção [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)</span><span class="sxs-lookup"><span data-stu-id="14eb0-110">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="14eb0-111">Listar funções de mapeamento de atributos com suporte.</span><span class="sxs-lookup"><span data-stu-id="14eb0-111">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="14eb0-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="14eb0-112">Properties</span></span>

| <span data-ttu-id="14eb0-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14eb0-113">Property</span></span>                   | <span data-ttu-id="14eb0-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="14eb0-114">Type</span></span>                      | <span data-ttu-id="14eb0-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="14eb0-115">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="14eb0-116">name</span><span class="sxs-lookup"><span data-stu-id="14eb0-116">name</span></span>                        |<span data-ttu-id="14eb0-117">String</span><span class="sxs-lookup"><span data-stu-id="14eb0-117">String</span></span>                    |<span data-ttu-id="14eb0-118">Nome do operador.</span><span class="sxs-lookup"><span data-stu-id="14eb0-118">Operator name.</span></span> |
|<span data-ttu-id="14eb0-119">parameters</span><span class="sxs-lookup"><span data-stu-id="14eb0-119">parameters</span></span>                  |<span data-ttu-id="14eb0-120">coleção [attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md)</span><span class="sxs-lookup"><span data-stu-id="14eb0-120">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="14eb0-121">Conjunto de parâmetros de função.</span><span class="sxs-lookup"><span data-stu-id="14eb0-121">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="14eb0-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="14eb0-122">JSON representation</span></span>

<span data-ttu-id="14eb0-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="14eb0-123">The following is a JSON representation of the resource.</span></span>

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
