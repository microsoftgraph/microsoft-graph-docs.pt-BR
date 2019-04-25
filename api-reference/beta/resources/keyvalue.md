---
title: tipo de recurso KeyValue
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 4223df85f9f120ba6477480f943d65a2511b6f2e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581083"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="128f7-103">tipo de recurso KeyValue</span><span class="sxs-lookup"><span data-stu-id="128f7-103">keyValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="128f7-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="128f7-104">JSON representation</span></span>

<span data-ttu-id="128f7-105">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="128f7-105">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="128f7-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="128f7-106">Properties</span></span>
| <span data-ttu-id="128f7-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="128f7-107">Property</span></span>     | <span data-ttu-id="128f7-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="128f7-108">Type</span></span>   |<span data-ttu-id="128f7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="128f7-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="128f7-110">key</span><span class="sxs-lookup"><span data-stu-id="128f7-110">key</span></span>|<span data-ttu-id="128f7-111">string</span><span class="sxs-lookup"><span data-stu-id="128f7-111">string</span></span>||
|<span data-ttu-id="128f7-112">value</span><span class="sxs-lookup"><span data-stu-id="128f7-112">value</span></span>|<span data-ttu-id="128f7-113">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="128f7-113">string</span></span>||

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
