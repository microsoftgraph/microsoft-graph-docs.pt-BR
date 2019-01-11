---
title: tipo de recurso de attributeMappingFunctionSchema
description: Descreve uma função que pode ser usada em um mapeamento de atributo para transformar valores durante a sincronização.
localization_priority: Normal
ms.openlocfilehash: 7273534d281d8ea5eaf3709b530776295cd9c767
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822159"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="a4210-103">tipo de recurso de attributeMappingFunctionSchema</span><span class="sxs-lookup"><span data-stu-id="a4210-103">attributeMappingFunctionSchema resource type</span></span>

> <span data-ttu-id="a4210-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a4210-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4210-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a4210-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a4210-106">Descreve uma função que pode ser usada em um [mapeamento de atributos](synchronization-attributemapping.md) para transformar valores durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="a4210-106">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="a4210-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="a4210-107">Methods</span></span>

| <span data-ttu-id="a4210-108">Método</span><span class="sxs-lookup"><span data-stu-id="a4210-108">Method</span></span>           | <span data-ttu-id="a4210-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a4210-109">Return Type</span></span>    |<span data-ttu-id="a4210-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4210-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a4210-111">List</span><span class="sxs-lookup"><span data-stu-id="a4210-111">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="a4210-112">coleção [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)</span><span class="sxs-lookup"><span data-stu-id="a4210-112">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="a4210-113">Funções de mapeamento de atributo de lista com suporte.</span><span class="sxs-lookup"><span data-stu-id="a4210-113">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="a4210-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a4210-114">Properties</span></span>

| <span data-ttu-id="a4210-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a4210-115">Property</span></span>                   | <span data-ttu-id="a4210-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4210-116">Type</span></span>                      | <span data-ttu-id="a4210-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4210-117">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="a4210-118">name</span><span class="sxs-lookup"><span data-stu-id="a4210-118">name</span></span>                        |<span data-ttu-id="a4210-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4210-119">String</span></span>                    |<span data-ttu-id="a4210-120">Nome do operador.</span><span class="sxs-lookup"><span data-stu-id="a4210-120">Operator name.</span></span> |
|<span data-ttu-id="a4210-121">parâmetros</span><span class="sxs-lookup"><span data-stu-id="a4210-121">parameters</span></span>                  |<span data-ttu-id="a4210-122">coleção [attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md)</span><span class="sxs-lookup"><span data-stu-id="a4210-122">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="a4210-123">Coleção de parâmetros de função.</span><span class="sxs-lookup"><span data-stu-id="a4210-123">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a4210-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a4210-124">JSON representation</span></span>

<span data-ttu-id="a4210-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a4210-125">The following is a JSON representation of the resource.</span></span>

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
