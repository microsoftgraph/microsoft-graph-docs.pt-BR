---
title: tipo de recurso timeStamp
description: Informações de data e hora para um ponto no tempo.
localization_priority: Normal
ms.openlocfilehash: 79faa8f74fbaf64eb6756183ecc309c6522873e6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463569"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="5db76-103">tipo de recurso timeStamp</span><span class="sxs-lookup"><span data-stu-id="5db76-103">timeStamp resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5db76-104">Informações de data e hora para um ponto no tempo.</span><span class="sxs-lookup"><span data-stu-id="5db76-104">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5db76-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5db76-105">JSON representation</span></span>

<span data-ttu-id="5db76-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="5db76-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="5db76-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5db76-107">Properties</span></span>
| <span data-ttu-id="5db76-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5db76-108">Property</span></span>     | <span data-ttu-id="5db76-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5db76-109">Type</span></span>   |<span data-ttu-id="5db76-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5db76-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5db76-111">data</span><span class="sxs-lookup"><span data-stu-id="5db76-111">date</span></span>|<span data-ttu-id="5db76-112">Data</span><span class="sxs-lookup"><span data-stu-id="5db76-112">Date</span></span>|<span data-ttu-id="5db76-113">A parte de data do carimbo de data/hora.</span><span class="sxs-lookup"><span data-stu-id="5db76-113">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="5db76-114">time</span><span class="sxs-lookup"><span data-stu-id="5db76-114">time</span></span>|<span data-ttu-id="5db76-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="5db76-115">TimeOfDay</span></span>|<span data-ttu-id="5db76-116">A parte de tempo do carimbo de data/hora.</span><span class="sxs-lookup"><span data-stu-id="5db76-116">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="5db76-117">timeZone</span><span class="sxs-lookup"><span data-stu-id="5db76-117">timeZone</span></span>|<span data-ttu-id="5db76-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5db76-118">String</span></span>|<span data-ttu-id="5db76-119">A parte de fuso horário do carimbo de data/hora, que é uma das 24 áreas de longitudinal do mundo.</span><span class="sxs-lookup"><span data-stu-id="5db76-119">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

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
