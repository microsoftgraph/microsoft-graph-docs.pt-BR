---
title: Tipo de recurso attendeeAvailability
description: A disponibilidade de um participante.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 396c53b8d03f573c214dcf43a3637cf06f412a33
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/28/2019
ms.locfileid: "30937758"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="602b1-103">Tipo de recurso attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="602b1-103">attendeeAvailability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="602b1-104">A disponibilidade de um participante.</span><span class="sxs-lookup"><span data-stu-id="602b1-104">The availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="602b1-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="602b1-105">JSON representation</span></span>

<span data-ttu-id="602b1-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="602b1-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailability"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeBase"},
  "availability": "String"
}

```
## <a name="properties"></a><span data-ttu-id="602b1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="602b1-107">Properties</span></span>
| <span data-ttu-id="602b1-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="602b1-108">Property</span></span>     | <span data-ttu-id="602b1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="602b1-109">Type</span></span>   |<span data-ttu-id="602b1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="602b1-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="602b1-111">attendee</span><span class="sxs-lookup"><span data-stu-id="602b1-111">attendee</span></span>|[<span data-ttu-id="602b1-112">attendeeBase</span><span class="sxs-lookup"><span data-stu-id="602b1-112">attendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="602b1-113">O endereço de email e o tipo de participante, se é uma pessoa ou um recurso, e se é obrigatório ou opcional se for uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="602b1-113">The email address and type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="602b1-114">availability</span><span class="sxs-lookup"><span data-stu-id="602b1-114">availability</span></span>|<span data-ttu-id="602b1-115">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="602b1-115">freeBusyStatus</span></span>| <span data-ttu-id="602b1-p101">O status de disponibilidade do participante. Os possíveis valores são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="602b1-p101">The availability status of the attendee. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeeavailability.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->