---
title: Tipo de recurso timeClockSettings
description: Representa as configurações do horário para um agendamento.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 96ffddc0730ffaff73d21a8ab051acf9ea140ccc
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786359"
---
# <a name="timeclocksettings-resource-type"></a><span data-ttu-id="66077-103">Tipo de recurso timeClockSettings</span><span class="sxs-lookup"><span data-stu-id="66077-103">timeClockSettings resource type</span></span>

<span data-ttu-id="66077-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66077-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66077-105">Representa as configurações do horário para um [agendamento.](schedule.md)</span><span class="sxs-lookup"><span data-stu-id="66077-105">Represents timeclock settings for a [schedule](schedule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="66077-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66077-106">Properties</span></span>
|<span data-ttu-id="66077-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66077-107">Property</span></span>               |<span data-ttu-id="66077-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="66077-108">Type</span></span>           |<span data-ttu-id="66077-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="66077-109">Description</span></span>                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| <span data-ttu-id="66077-110">approvedLocation</span><span class="sxs-lookup"><span data-stu-id="66077-110">approvedLocation</span></span> | [<span data-ttu-id="66077-111">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="66077-111">geoCoordinates</span></span>](geocoordinates.md)  |<span data-ttu-id="66077-112">O local aprroved do **timeClock**.</span><span class="sxs-lookup"><span data-stu-id="66077-112">The aprroved location of the **timeClock**.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="66077-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66077-113">JSON representation</span></span>

<span data-ttu-id="66077-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="66077-114">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeClockSettings"
}-->
```json
{ 
   "approvedLocation": {

           "altitude": {"@odata.type": "microsoft.graph.GeoCoordinates"},

           "latitude": {"@odata.type": "microsoft.graph.GeoCoordinates"},

           "longitude": {"@odata.type": "microsoft.graph.GeoCoordinates"}

        }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeClockSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
