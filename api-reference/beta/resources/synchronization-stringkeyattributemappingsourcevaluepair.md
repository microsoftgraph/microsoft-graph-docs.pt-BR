---
title: tipo de recurso stringKeyAttributeMappingSourceValuePair
description: Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é attributeMappingSource.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dab0376441904f7ec935aa87da3b825d2a0e197d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007876"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a><span data-ttu-id="3ea6f-103">tipo de recurso stringKeyAttributeMappingSourceValuePair</span><span class="sxs-lookup"><span data-stu-id="3ea6f-103">stringKeyAttributeMappingSourceValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ea6f-104">Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é [attributeMappingSource](synchronization-attributemappingsource.md).</span><span class="sxs-lookup"><span data-stu-id="3ea6f-104">Represents a key-value pair where the key is a string and the value is [attributeMappingSource](synchronization-attributemappingsource.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3ea6f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3ea6f-105">Properties</span></span>
| <span data-ttu-id="3ea6f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ea6f-106">Property</span></span>     | <span data-ttu-id="3ea6f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ea6f-107">Type</span></span>   |<span data-ttu-id="3ea6f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ea6f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ea6f-109">key</span><span class="sxs-lookup"><span data-stu-id="3ea6f-109">key</span></span>|<span data-ttu-id="3ea6f-110">String</span><span class="sxs-lookup"><span data-stu-id="3ea6f-110">String</span></span>|<span data-ttu-id="3ea6f-111">O nome do parâmetro.</span><span class="sxs-lookup"><span data-stu-id="3ea6f-111">The name of the parameter.</span></span>|
|<span data-ttu-id="3ea6f-112">valor</span><span class="sxs-lookup"><span data-stu-id="3ea6f-112">value</span></span>|[<span data-ttu-id="3ea6f-113">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="3ea6f-113">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="3ea6f-114">O valor do parâmetro.</span><span class="sxs-lookup"><span data-stu-id="3ea6f-114">The value of the parameter.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3ea6f-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3ea6f-115">JSON representation</span></span>

<span data-ttu-id="3ea6f-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3ea6f-116">The following is a JSON representation of the resource.</span></span>

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
