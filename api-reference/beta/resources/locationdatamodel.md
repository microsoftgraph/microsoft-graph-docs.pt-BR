---
title: tipo de recurso locationDataModel
description: Representa as informações de locationDataModel de um evento.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 2b1fd0c25cdd41e6a8d9c87f8a1c0c80d70b78e5
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057325"
---
# <a name="locationdatamodel-resource-type"></a><span data-ttu-id="c9626-103">tipo de recurso locationDataModel</span><span class="sxs-lookup"><span data-stu-id="c9626-103">locationDataModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9626-104">Representa informações de localização de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="c9626-104">Represents location information for a meeting.</span></span>


## <a name="properties"></a><span data-ttu-id="c9626-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c9626-105">Properties</span></span>
| <span data-ttu-id="c9626-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9626-106">Property</span></span>  | <span data-ttu-id="c9626-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9626-107">Type</span></span>   | <span data-ttu-id="c9626-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9626-108">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="c9626-109">address</span><span class="sxs-lookup"><span data-stu-id="c9626-109">address</span></span> | [<span data-ttu-id="c9626-110">postalAddress</span><span class="sxs-lookup"><span data-stu-id="c9626-110">postalAddress</span></span>](postaladdress.md) |<span data-ttu-id="c9626-111">O endereço físico do local.</span><span class="sxs-lookup"><span data-stu-id="c9626-111">The street address of the location.</span></span> |
| <span data-ttu-id="c9626-112">coordenadas</span><span class="sxs-lookup"><span data-stu-id="c9626-112">coordinates</span></span> | [<span data-ttu-id="c9626-113">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="c9626-113">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="c9626-114">As coordenadas geográficas e a elevação do local.</span><span class="sxs-lookup"><span data-stu-id="c9626-114">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="c9626-115">displayName</span><span class="sxs-lookup"><span data-stu-id="c9626-115">displayName</span></span>  | <span data-ttu-id="c9626-116">String</span><span class="sxs-lookup"><span data-stu-id="c9626-116">String</span></span> | <span data-ttu-id="c9626-117">O nome associado ao local.</span><span class="sxs-lookup"><span data-stu-id="c9626-117">The name associated with the location.</span></span>                       |
| <span data-ttu-id="c9626-118">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="c9626-118">locationEmailAddress</span></span> | <span data-ttu-id="c9626-119">String</span><span class="sxs-lookup"><span data-stu-id="c9626-119">String</span></span> | <span data-ttu-id="c9626-120">O endereço de email opcional do local.</span><span class="sxs-lookup"><span data-stu-id="c9626-120">Optional email address of the location.</span></span> |
| <span data-ttu-id="c9626-121">locationUri</span><span class="sxs-lookup"><span data-stu-id="c9626-121">locationUri</span></span> | <span data-ttu-id="c9626-122">String</span><span class="sxs-lookup"><span data-stu-id="c9626-122">String</span></span> | <span data-ttu-id="c9626-123">URI opcional que representa o local.</span><span class="sxs-lookup"><span data-stu-id="c9626-123">Optional URI representing the location.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="c9626-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c9626-124">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locationDataModel"
}-->
```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "coordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "displayName": "string",
  "locationEmailAddress": "string",
  "locationUri": "string"
}

```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "locationDataModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/locationdatamodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
