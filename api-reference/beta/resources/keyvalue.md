---
title: tipo de recurso keyValue
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 4223df85f9f120ba6477480f943d65a2511b6f2e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528526"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="8fddd-103">tipo de recurso keyValue</span><span class="sxs-lookup"><span data-stu-id="8fddd-103">keyValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="8fddd-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8fddd-104">JSON representation</span></span>

<span data-ttu-id="8fddd-105">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8fddd-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyvalue"
}-->

```json
{
  "key": "string",
  "value": "string"
}

```
## <a name="properties"></a><span data-ttu-id="8fddd-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8fddd-106">Properties</span></span>
| <span data-ttu-id="8fddd-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8fddd-107">Property</span></span>     | <span data-ttu-id="8fddd-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8fddd-108">Type</span></span>   |<span data-ttu-id="8fddd-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8fddd-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8fddd-110">key</span><span class="sxs-lookup"><span data-stu-id="8fddd-110">key</span></span>|<span data-ttu-id="8fddd-111">string</span><span class="sxs-lookup"><span data-stu-id="8fddd-111">string</span></span>||
|<span data-ttu-id="8fddd-112">valor</span><span class="sxs-lookup"><span data-stu-id="8fddd-112">value</span></span>|<span data-ttu-id="8fddd-113">string</span><span class="sxs-lookup"><span data-stu-id="8fddd-113">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "keyValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/keyvalue.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
