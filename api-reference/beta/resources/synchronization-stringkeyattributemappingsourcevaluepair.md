---
title: Tipo de recurso stringKeyAttributeMappingSourceValuePair
description: Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é attributeMappingSource.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: d0bd761b64c41c930bda84b820d98501870e0c26
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135090"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a><span data-ttu-id="90ac1-103">Tipo de recurso stringKeyAttributeMappingSourceValuePair</span><span class="sxs-lookup"><span data-stu-id="90ac1-103">stringKeyAttributeMappingSourceValuePair resource type</span></span>

<span data-ttu-id="90ac1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90ac1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90ac1-105">Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é [attributeMappingSource](synchronization-attributemappingsource.md).</span><span class="sxs-lookup"><span data-stu-id="90ac1-105">Represents a key-value pair where the key is a string and the value is [attributeMappingSource](synchronization-attributemappingsource.md).</span></span>

## <a name="properties"></a><span data-ttu-id="90ac1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="90ac1-106">Properties</span></span>
| <span data-ttu-id="90ac1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90ac1-107">Property</span></span>     | <span data-ttu-id="90ac1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="90ac1-108">Type</span></span>   |<span data-ttu-id="90ac1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="90ac1-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90ac1-110">key</span><span class="sxs-lookup"><span data-stu-id="90ac1-110">key</span></span>|<span data-ttu-id="90ac1-111">String</span><span class="sxs-lookup"><span data-stu-id="90ac1-111">String</span></span>|<span data-ttu-id="90ac1-112">O nome do parâmetro.</span><span class="sxs-lookup"><span data-stu-id="90ac1-112">The name of the parameter.</span></span>|
|<span data-ttu-id="90ac1-113">valor</span><span class="sxs-lookup"><span data-stu-id="90ac1-113">value</span></span>|[<span data-ttu-id="90ac1-114">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="90ac1-114">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="90ac1-115">O valor do parâmetro.</span><span class="sxs-lookup"><span data-stu-id="90ac1-115">The value of the parameter.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="90ac1-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="90ac1-116">JSON representation</span></span>

<span data-ttu-id="90ac1-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="90ac1-117">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyAttributeMappingSourceValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


