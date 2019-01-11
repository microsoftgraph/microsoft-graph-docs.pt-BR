---
title: tipo de recurso de stringKeyAttributeMappingSourceValuePair
description: Representa um par de chave-valor em que a chave é uma cadeia de caracteres e o valor é attributeMappingSource.
localization_priority: Normal
ms.openlocfilehash: 24695cc64fd3c240d5416a7b37e9a5d373e5a88a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805086"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a><span data-ttu-id="408b3-103">tipo de recurso de stringKeyAttributeMappingSourceValuePair</span><span class="sxs-lookup"><span data-stu-id="408b3-103">stringKeyAttributeMappingSourceValuePair resource type</span></span>

> <span data-ttu-id="408b3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="408b3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="408b3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="408b3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="408b3-106">Representa um par de chave-valor em que a chave é uma cadeia de caracteres e o valor é [attributeMappingSource](synchronization-attributemappingsource.md).</span><span class="sxs-lookup"><span data-stu-id="408b3-106">Represents a key-value pair where the key is a string and the value is [attributeMappingSource](synchronization-attributemappingsource.md).</span></span>

## <a name="properties"></a><span data-ttu-id="408b3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="408b3-107">Properties</span></span>
| <span data-ttu-id="408b3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="408b3-108">Property</span></span>     | <span data-ttu-id="408b3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="408b3-109">Type</span></span>   |<span data-ttu-id="408b3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="408b3-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="408b3-111">key</span><span class="sxs-lookup"><span data-stu-id="408b3-111">key</span></span>|<span data-ttu-id="408b3-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="408b3-112">String</span></span>|<span data-ttu-id="408b3-113">O nome do parâmetro.</span><span class="sxs-lookup"><span data-stu-id="408b3-113">The name of the parameter.</span></span>|
|<span data-ttu-id="408b3-114">valor</span><span class="sxs-lookup"><span data-stu-id="408b3-114">value</span></span>|[<span data-ttu-id="408b3-115">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="408b3-115">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="408b3-116">O valor do parâmetro.</span><span class="sxs-lookup"><span data-stu-id="408b3-116">The value of the parameter.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="408b3-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="408b3-117">JSON representation</span></span>

<span data-ttu-id="408b3-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="408b3-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"
}-->

```json
{
  "key": "String",
  "value": {"@odata.type": "microsoft.graph.attributeMappingSource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "stringKeyAttributeMappingSourceValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
