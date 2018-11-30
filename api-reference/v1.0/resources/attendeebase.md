---
title: Tipo de recurso attendeeBase
description: O tipo de participante.
ms.openlocfilehash: 6995ac94a600a60313ef26208b441c6ef6fdf001
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006052"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="a2e8a-103">Tipo de recurso attendeeBase</span><span class="sxs-lookup"><span data-stu-id="a2e8a-103">attendeeBase resource type</span></span>

<span data-ttu-id="a2e8a-104">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="a2e8a-104">The type of attendee.</span></span>

<span data-ttu-id="a2e8a-105">Derivado do [destinatário](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="a2e8a-105">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2e8a-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2e8a-106">JSON representation</span></span>

<span data-ttu-id="a2e8a-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a2e8a-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.recipient",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeBase"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a><span data-ttu-id="a2e8a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2e8a-108">Properties</span></span>
| <span data-ttu-id="a2e8a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2e8a-109">Property</span></span>     | <span data-ttu-id="a2e8a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2e8a-110">Type</span></span>   |<span data-ttu-id="a2e8a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2e8a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2e8a-112">type</span><span class="sxs-lookup"><span data-stu-id="a2e8a-112">type</span></span>|<span data-ttu-id="a2e8a-113">attendeeType</span><span class="sxs-lookup"><span data-stu-id="a2e8a-113">attendeeType</span></span>| <span data-ttu-id="a2e8a-114">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="a2e8a-114">The type of attendee.</span></span> <span data-ttu-id="a2e8a-115">Os valores possíveis são: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="a2e8a-115">The possible values are: `required`, `optional`, `resource`.</span></span> <span data-ttu-id="a2e8a-116">Se o nome do participante é uma pessoa, [findMeetingTimes](../api/user-findmeetingtimes.md) sempre considera atualmente a pessoa é do `Required` tipo.</span><span class="sxs-lookup"><span data-stu-id="a2e8a-116">Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="a2e8a-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a2e8a-117">emailAddress</span></span>|[<span data-ttu-id="a2e8a-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a2e8a-118">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="a2e8a-119">Inclui o nome e endereço SMTP do participante.</span><span class="sxs-lookup"><span data-stu-id="a2e8a-119">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
