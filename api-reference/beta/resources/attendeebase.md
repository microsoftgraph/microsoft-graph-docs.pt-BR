---
title: Tipo de recurso attendeeBase
description: O tipo de participante.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: dfa873daf5b3c5a47e10ab480292ffb11b656b01
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974291"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="d2197-103">Tipo de recurso attendeeBase</span><span class="sxs-lookup"><span data-stu-id="d2197-103">attendeeBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2197-104">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="d2197-104">The type of attendee.</span></span>

<span data-ttu-id="d2197-105">Derivado do [destinatário](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="d2197-105">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2197-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2197-106">JSON representation</span></span>

<span data-ttu-id="d2197-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d2197-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
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
## <a name="properties"></a><span data-ttu-id="d2197-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2197-108">Properties</span></span>
| <span data-ttu-id="d2197-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2197-109">Property</span></span>     | <span data-ttu-id="d2197-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2197-110">Type</span></span>   |<span data-ttu-id="d2197-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2197-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2197-112">type</span><span class="sxs-lookup"><span data-stu-id="d2197-112">type</span></span>|<span data-ttu-id="d2197-113">String</span><span class="sxs-lookup"><span data-stu-id="d2197-113">String</span></span>| <span data-ttu-id="d2197-p101">O tipo de participante. Os valores possíveis são: `required`, `optional`, `resource`. Atualmente, se o participante é uma pessoa, [findMeetingTimes](../api/user-findmeetingtimes.md) sempre considera que a pessoa é do tipo `Required`.</span><span class="sxs-lookup"><span data-stu-id="d2197-p101">The type of attendee. Possible values are: `required`, `optional`, `resource`. Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="d2197-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d2197-117">emailAddress</span></span>|[<span data-ttu-id="d2197-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d2197-118">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="d2197-119">Inclui o nome e endereço SMTP do participante.</span><span class="sxs-lookup"><span data-stu-id="d2197-119">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
