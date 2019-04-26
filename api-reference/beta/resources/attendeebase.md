---
title: Tipo de recurso attendeeBase
description: O tipo de participante.
localization_priority: Normal
ms.openlocfilehash: a0095a2076cd09bee2d4b934bac29cd030924ec1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328515"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="f9c42-103">Tipo de recurso attendeeBase</span><span class="sxs-lookup"><span data-stu-id="f9c42-103">attendeeBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9c42-104">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="f9c42-104">The type of attendee.</span></span>

<span data-ttu-id="f9c42-105">Derivado do [destinatário](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="f9c42-105">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9c42-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f9c42-106">JSON representation</span></span>

<span data-ttu-id="f9c42-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="f9c42-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="f9c42-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f9c42-108">Properties</span></span>
| <span data-ttu-id="f9c42-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9c42-109">Property</span></span>     | <span data-ttu-id="f9c42-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9c42-110">Type</span></span>   |<span data-ttu-id="f9c42-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9c42-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9c42-112">tipo</span><span class="sxs-lookup"><span data-stu-id="f9c42-112">type</span></span>|<span data-ttu-id="f9c42-113">String</span><span class="sxs-lookup"><span data-stu-id="f9c42-113">String</span></span>| <span data-ttu-id="f9c42-p101">O tipo de participante. Os valores possíveis são: `required`, `optional`, `resource`. Atualmente, se o participante é uma pessoa, [findMeetingTimes](../api/user-findmeetingtimes.md) sempre considera que a pessoa é do tipo `Required`.</span><span class="sxs-lookup"><span data-stu-id="f9c42-p101">The type of attendee. Possible values are: `required`, `optional`, `resource`. Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="f9c42-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="f9c42-117">emailAddress</span></span>|[<span data-ttu-id="f9c42-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="f9c42-118">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="f9c42-119">Inclui o nome e endereço SMTP do participante.</span><span class="sxs-lookup"><span data-stu-id="f9c42-119">Includes the name and SMTP address of the attendee.</span></span>|

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
