---
title: Tipo de recurso attendeeAvailability
description: A disponibilidade de um participante.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8e9a9eb91ccfc70e771357abf3b91d6a23dbd367
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013252"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="e3239-103">Tipo de recurso attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="e3239-103">attendeeAvailability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3239-104">A disponibilidade de um participante.</span><span class="sxs-lookup"><span data-stu-id="e3239-104">The availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3239-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e3239-105">JSON representation</span></span>

<span data-ttu-id="e3239-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e3239-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="e3239-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e3239-107">Properties</span></span>
| <span data-ttu-id="e3239-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3239-108">Property</span></span>     | <span data-ttu-id="e3239-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3239-109">Type</span></span>   |<span data-ttu-id="e3239-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3239-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3239-111">attendee</span><span class="sxs-lookup"><span data-stu-id="e3239-111">attendee</span></span>|[<span data-ttu-id="e3239-112">attendeeBase</span><span class="sxs-lookup"><span data-stu-id="e3239-112">attendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="e3239-113">O endereço de email e o tipo de participante, se é uma pessoa ou um recurso, e se é obrigatório ou opcional se for uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="e3239-113">The email address and type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="e3239-114">availability</span><span class="sxs-lookup"><span data-stu-id="e3239-114">availability</span></span>|<span data-ttu-id="e3239-115">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="e3239-115">freeBusyStatus</span></span>| <span data-ttu-id="e3239-p101">O status de disponibilidade do participante. Os possíveis valores são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="e3239-p101">The availability status of the attendee. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
