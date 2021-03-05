---
title: Tipo de recurso attendeeAvailability
description: A disponibilidade de um participante.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 9cfdc6b1f944457d24f1b569aa3d6263e6375aa8
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473564"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="dffb7-103">Tipo de recurso attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="dffb7-103">attendeeAvailability resource type</span></span>

<span data-ttu-id="dffb7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dffb7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dffb7-105">A disponibilidade de um participante.</span><span class="sxs-lookup"><span data-stu-id="dffb7-105">The availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dffb7-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dffb7-106">JSON representation</span></span>

<span data-ttu-id="dffb7-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="dffb7-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="dffb7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dffb7-108">Properties</span></span>
| <span data-ttu-id="dffb7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dffb7-109">Property</span></span>     | <span data-ttu-id="dffb7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="dffb7-110">Type</span></span>   |<span data-ttu-id="dffb7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="dffb7-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dffb7-112">attendee</span><span class="sxs-lookup"><span data-stu-id="dffb7-112">attendee</span></span>|[<span data-ttu-id="dffb7-113">attendeeBase</span><span class="sxs-lookup"><span data-stu-id="dffb7-113">attendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="dffb7-114">O endereço de email e o tipo de participante - se é uma pessoa ou um recurso e se é obrigatório ou opcional se for uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="dffb7-114">The email address and type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="dffb7-115">availability</span><span class="sxs-lookup"><span data-stu-id="dffb7-115">availability</span></span>|<span data-ttu-id="dffb7-116">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="dffb7-116">freeBusyStatus</span></span>| <span data-ttu-id="dffb7-p101">O status de disponibilidade do participante. Os possíveis valores são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="dffb7-p101">The availability status of the attendee. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

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


