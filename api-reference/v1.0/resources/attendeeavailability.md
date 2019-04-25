---
title: Tipo de recurso attendeeAvailability
description: A disponibilidade de um participante.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 63014553824b833e2e4cdfb03485fcb7962c01a0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569358"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="e5dd4-103">Tipo de recurso attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="e5dd4-103">attendeeAvailability resource type</span></span>

<span data-ttu-id="e5dd4-104">A disponibilidade de um participante.</span><span class="sxs-lookup"><span data-stu-id="e5dd4-104">The availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5dd4-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e5dd4-105">JSON representation</span></span>

<span data-ttu-id="e5dd4-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e5dd4-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="e5dd4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e5dd4-107">Properties</span></span>
| <span data-ttu-id="e5dd4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5dd4-108">Property</span></span>     | <span data-ttu-id="e5dd4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5dd4-109">Type</span></span>   |<span data-ttu-id="e5dd4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5dd4-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5dd4-111">attendee</span><span class="sxs-lookup"><span data-stu-id="e5dd4-111">attendee</span></span>|[<span data-ttu-id="e5dd4-112">attendeeBase</span><span class="sxs-lookup"><span data-stu-id="e5dd4-112">attendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="e5dd4-113">O endereço de email e o tipo de participante, se é uma pessoa ou um recurso, e se é obrigatório ou opcional se for uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="e5dd4-113">The email address and type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="e5dd4-114">availability</span><span class="sxs-lookup"><span data-stu-id="e5dd4-114">availability</span></span>|<span data-ttu-id="e5dd4-115">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="e5dd4-115">freeBusyStatus</span></span>| <span data-ttu-id="e5dd4-116">O status de disponibilidade do participante.</span><span class="sxs-lookup"><span data-stu-id="e5dd4-116">The availability status of the attendee.</span></span> <span data-ttu-id="e5dd4-117">Os valores possíveis são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="e5dd4-117">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
