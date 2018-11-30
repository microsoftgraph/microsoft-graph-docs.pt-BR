---
title: Tipo de recurso attendeeAvailability
description: O tipo e a disponibilidade dos participantes.
ms.openlocfilehash: 446dfb77d8f85021f41795038c3c1d597c6f1a6d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004257"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="f760d-103">Tipo de recurso attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="f760d-103">attendeeAvailability resource type</span></span>

<span data-ttu-id="f760d-104">O tipo e a disponibilidade dos participantes.</span><span class="sxs-lookup"><span data-stu-id="f760d-104">The type and availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f760d-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f760d-105">JSON representation</span></span>

<span data-ttu-id="f760d-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="f760d-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="f760d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f760d-107">Properties</span></span>
| <span data-ttu-id="f760d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f760d-108">Property</span></span>     | <span data-ttu-id="f760d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f760d-109">Type</span></span>   |<span data-ttu-id="f760d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f760d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f760d-111">attendee</span><span class="sxs-lookup"><span data-stu-id="f760d-111">attendee</span></span>|[<span data-ttu-id="f760d-112">AttendeeBase</span><span class="sxs-lookup"><span data-stu-id="f760d-112">AttendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="f760d-113">O tipo de participante, ou seja, se é um recurso ou uma pessoa e, no caso de uma pessoa, se é obrigatório ou opcional.</span><span class="sxs-lookup"><span data-stu-id="f760d-113">The type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="f760d-114">availability</span><span class="sxs-lookup"><span data-stu-id="f760d-114">availability</span></span>|<span data-ttu-id="f760d-115">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="f760d-115">freeBusyStatus</span></span>| <span data-ttu-id="f760d-116">O status de disponibilidade do participante.</span><span class="sxs-lookup"><span data-stu-id="f760d-116">The availability status of the attendee.</span></span> <span data-ttu-id="f760d-117">Os valores possíveis são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f760d-117">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
