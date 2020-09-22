---
title: Tipo de recurso attendeeBase
description: O tipo de participante.
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 59e1aa072d511c575bb6911e19387de753d47bee
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988545"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="9f2f2-103">Tipo de recurso attendeeBase</span><span class="sxs-lookup"><span data-stu-id="9f2f2-103">attendeeBase resource type</span></span>

<span data-ttu-id="9f2f2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f2f2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9f2f2-105">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="9f2f2-105">The type of attendee.</span></span>

<span data-ttu-id="9f2f2-106">Derivado do [destinatário](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="9f2f2-106">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f2f2-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9f2f2-107">JSON representation</span></span>

<span data-ttu-id="9f2f2-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="9f2f2-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="9f2f2-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9f2f2-109">Properties</span></span>
| <span data-ttu-id="9f2f2-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f2f2-110">Property</span></span>     | <span data-ttu-id="9f2f2-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f2f2-111">Type</span></span>   |<span data-ttu-id="9f2f2-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f2f2-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f2f2-113">type</span><span class="sxs-lookup"><span data-stu-id="9f2f2-113">type</span></span>|<span data-ttu-id="9f2f2-114">articipantetype</span><span class="sxs-lookup"><span data-stu-id="9f2f2-114">attendeeType</span></span>| <span data-ttu-id="9f2f2-115">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="9f2f2-115">The type of attendee.</span></span> <span data-ttu-id="9f2f2-116">Os valores possíveis são: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="9f2f2-116">The possible values are: `required`, `optional`, `resource`.</span></span> <span data-ttu-id="9f2f2-117">Atualmente, se o participante é uma pessoa, [findMeetingTimes](../api/user-findmeetingtimes.md) sempre considera que a pessoa é do tipo `Required`.</span><span class="sxs-lookup"><span data-stu-id="9f2f2-117">Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="9f2f2-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9f2f2-118">emailAddress</span></span>|[<span data-ttu-id="9f2f2-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9f2f2-119">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="9f2f2-120">Inclui o nome e endereço SMTP do participante.</span><span class="sxs-lookup"><span data-stu-id="9f2f2-120">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

