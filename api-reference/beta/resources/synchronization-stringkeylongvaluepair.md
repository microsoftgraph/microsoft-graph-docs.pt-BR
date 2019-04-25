---
title: tipo de recurso stringKeyLongValuePair
description: Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é Int64.
localization_priority: Normal
ms.openlocfilehash: 97ca9f4f7b4079311a1ce6996fde0472c527e7f9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524537"
---
# <a name="stringkeylongvaluepair-resource-type"></a><span data-ttu-id="64be9-103">tipo de recurso stringKeyLongValuePair</span><span class="sxs-lookup"><span data-stu-id="64be9-103">stringKeyLongValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64be9-104">Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é Int64.</span><span class="sxs-lookup"><span data-stu-id="64be9-104">Represents a key-value pair where the key is a string and the value is an Int64.</span></span>

## <a name="properties"></a><span data-ttu-id="64be9-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="64be9-105">Properties</span></span>
| <span data-ttu-id="64be9-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64be9-106">Property</span></span>     | <span data-ttu-id="64be9-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="64be9-107">Type</span></span>   |<span data-ttu-id="64be9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="64be9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64be9-109">key</span><span class="sxs-lookup"><span data-stu-id="64be9-109">key</span></span>|<span data-ttu-id="64be9-110">String</span><span class="sxs-lookup"><span data-stu-id="64be9-110">String</span></span>|<span data-ttu-id="64be9-111">Chave.</span><span class="sxs-lookup"><span data-stu-id="64be9-111">Key.</span></span>|
|<span data-ttu-id="64be9-112">valor</span><span class="sxs-lookup"><span data-stu-id="64be9-112">value</span></span>|<span data-ttu-id="64be9-113">Int64</span><span class="sxs-lookup"><span data-stu-id="64be9-113">Int64</span></span>|<span data-ttu-id="64be9-114">Valor.</span><span class="sxs-lookup"><span data-stu-id="64be9-114">Value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="64be9-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="64be9-115">JSON representation</span></span>

<span data-ttu-id="64be9-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="64be9-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyLongValuePair"
}-->

```json
{
  "key": "String",
  "value": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyLongValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-stringkeylongvaluepair.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
