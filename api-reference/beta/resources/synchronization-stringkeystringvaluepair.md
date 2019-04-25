---
title: tipo de recurso stringKeyStringValuePair
description: Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é uma cadeia de caracteres.
localization_priority: Normal
ms.openlocfilehash: f91d63ee4b4d3b0328bbb6fbe58c74ec8f78c5b2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526269"
---
# <a name="stringkeystringvaluepair-resource-type"></a><span data-ttu-id="3bdc6-103">tipo de recurso stringKeyStringValuePair</span><span class="sxs-lookup"><span data-stu-id="3bdc6-103">stringKeyStringValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bdc6-104">Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é uma cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="3bdc6-104">Represents a key-value pair where the key is a string and the value is a string.</span></span>

## <a name="properties"></a><span data-ttu-id="3bdc6-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3bdc6-105">Properties</span></span>
| <span data-ttu-id="3bdc6-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3bdc6-106">Property</span></span>     | <span data-ttu-id="3bdc6-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3bdc6-107">Type</span></span>   |<span data-ttu-id="3bdc6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bdc6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3bdc6-109">key</span><span class="sxs-lookup"><span data-stu-id="3bdc6-109">key</span></span>|<span data-ttu-id="3bdc6-110">String</span><span class="sxs-lookup"><span data-stu-id="3bdc6-110">String</span></span>|<span data-ttu-id="3bdc6-111">Chave.</span><span class="sxs-lookup"><span data-stu-id="3bdc6-111">Key.</span></span>|
|<span data-ttu-id="3bdc6-112">value</span><span class="sxs-lookup"><span data-stu-id="3bdc6-112">value</span></span>|<span data-ttu-id="3bdc6-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bdc6-113">String</span></span>|<span data-ttu-id="3bdc6-114">Valor.</span><span class="sxs-lookup"><span data-stu-id="3bdc6-114">Value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3bdc6-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3bdc6-115">JSON representation</span></span>

<span data-ttu-id="3bdc6-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3bdc6-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyStringValuePair"
}-->

```json
{
  "key": "String",
  "value": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyStringValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-stringkeystringvaluepair.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
