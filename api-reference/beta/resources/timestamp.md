---
title: tipo de recurso da carimbo de hora
description: Data e hora informações para um ponto no tempo.
localization_priority: Normal
ms.openlocfilehash: 79faa8f74fbaf64eb6756183ecc309c6522873e6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529359"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="fcfd9-103">tipo de recurso da carimbo de hora</span><span class="sxs-lookup"><span data-stu-id="fcfd9-103">timeStamp resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fcfd9-104">Data e hora informações para um ponto no tempo.</span><span class="sxs-lookup"><span data-stu-id="fcfd9-104">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fcfd9-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fcfd9-105">JSON representation</span></span>

<span data-ttu-id="fcfd9-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="fcfd9-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeStamp"
}-->

```json
{
  "date": "String (timestamp)",
  "time": "String (timestamp)",
  "timeZone": "string"
}

```
## <a name="properties"></a><span data-ttu-id="fcfd9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fcfd9-107">Properties</span></span>
| <span data-ttu-id="fcfd9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fcfd9-108">Property</span></span>     | <span data-ttu-id="fcfd9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fcfd9-109">Type</span></span>   |<span data-ttu-id="fcfd9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcfd9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fcfd9-111">data</span><span class="sxs-lookup"><span data-stu-id="fcfd9-111">date</span></span>|<span data-ttu-id="fcfd9-112">Data</span><span class="sxs-lookup"><span data-stu-id="fcfd9-112">Date</span></span>|<span data-ttu-id="fcfd9-113">A parte da data do carimbo de hora.</span><span class="sxs-lookup"><span data-stu-id="fcfd9-113">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="fcfd9-114">time</span><span class="sxs-lookup"><span data-stu-id="fcfd9-114">time</span></span>|<span data-ttu-id="fcfd9-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="fcfd9-115">TimeOfDay</span></span>|<span data-ttu-id="fcfd9-116">A parte do tempo do carimbo de hora.</span><span class="sxs-lookup"><span data-stu-id="fcfd9-116">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="fcfd9-117">timeZone</span><span class="sxs-lookup"><span data-stu-id="fcfd9-117">timeZone</span></span>|<span data-ttu-id="fcfd9-118">String</span><span class="sxs-lookup"><span data-stu-id="fcfd9-118">String</span></span>|<span data-ttu-id="fcfd9-119">A porção de fuso horário da carimbo de hora, o que é uma das áreas longitudinal 24 no mundo.</span><span class="sxs-lookup"><span data-stu-id="fcfd9-119">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timestamp.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
