---
title: tipo de recurso de attributeMappingFunctionSchema
description: Descreve uma função que pode ser usada em um mapeamento de atributo para transformar valores durante a sincronização.
ms.openlocfilehash: 9760669bb29700bfa79c1cd375857b4fd673879b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037040"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="890a8-103">tipo de recurso de attributeMappingFunctionSchema</span><span class="sxs-lookup"><span data-stu-id="890a8-103">attributeMappingFunctionSchema resource type</span></span>

> <span data-ttu-id="890a8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="890a8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="890a8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="890a8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="890a8-106">Descreve uma função que pode ser usada em um [mapeamento de atributos](synchronization-attributemapping.md) para transformar valores durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="890a8-106">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="890a8-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="890a8-107">Methods</span></span>

| <span data-ttu-id="890a8-108">Método</span><span class="sxs-lookup"><span data-stu-id="890a8-108">Method</span></span>           | <span data-ttu-id="890a8-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="890a8-109">Return Type</span></span>    |<span data-ttu-id="890a8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="890a8-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="890a8-111">List</span><span class="sxs-lookup"><span data-stu-id="890a8-111">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="890a8-112">coleção [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)</span><span class="sxs-lookup"><span data-stu-id="890a8-112">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="890a8-113">Funções de mapeamento de atributo de lista com suporte.</span><span class="sxs-lookup"><span data-stu-id="890a8-113">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="890a8-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="890a8-114">Properties</span></span>

| <span data-ttu-id="890a8-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="890a8-115">Property</span></span>                   | <span data-ttu-id="890a8-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="890a8-116">Type</span></span>                      | <span data-ttu-id="890a8-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="890a8-117">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="890a8-118">name</span><span class="sxs-lookup"><span data-stu-id="890a8-118">name</span></span>                        |<span data-ttu-id="890a8-119">String</span><span class="sxs-lookup"><span data-stu-id="890a8-119">String</span></span>                    |<span data-ttu-id="890a8-120">Nome do operador.</span><span class="sxs-lookup"><span data-stu-id="890a8-120">Operator name.</span></span> |
|<span data-ttu-id="890a8-121">parameters</span><span class="sxs-lookup"><span data-stu-id="890a8-121">parameters</span></span>                  |<span data-ttu-id="890a8-122">coleção [attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md)</span><span class="sxs-lookup"><span data-stu-id="890a8-122">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="890a8-123">Coleção de parâmetros de função.</span><span class="sxs-lookup"><span data-stu-id="890a8-123">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="890a8-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="890a8-124">JSON representation</span></span>

<span data-ttu-id="890a8-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="890a8-125">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "attributeMappingFunctionSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->