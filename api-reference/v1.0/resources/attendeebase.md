---
title: Tipo de recurso attendeeBase
description: O tipo de participante.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a7eaf030413e576721bd672fc63111a62742c163
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532073"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="ac963-103">Tipo de recurso attendeeBase</span><span class="sxs-lookup"><span data-stu-id="ac963-103">attendeeBase resource type</span></span>

<span data-ttu-id="ac963-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac963-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ac963-105">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="ac963-105">The type of attendee.</span></span>

<span data-ttu-id="ac963-106">Derivado do [destinatário](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="ac963-106">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac963-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac963-107">JSON representation</span></span>

<span data-ttu-id="ac963-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="ac963-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="ac963-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac963-109">Properties</span></span>
| <span data-ttu-id="ac963-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac963-110">Property</span></span>     | <span data-ttu-id="ac963-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac963-111">Type</span></span>   |<span data-ttu-id="ac963-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac963-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac963-113">type</span><span class="sxs-lookup"><span data-stu-id="ac963-113">type</span></span>|<span data-ttu-id="ac963-114">articipantetype</span><span class="sxs-lookup"><span data-stu-id="ac963-114">attendeeType</span></span>| <span data-ttu-id="ac963-115">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="ac963-115">The type of attendee.</span></span> <span data-ttu-id="ac963-116">Os valores possíveis são: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="ac963-116">The possible values are: `required`, `optional`, `resource`.</span></span> <span data-ttu-id="ac963-117">Atualmente, se o participante é uma pessoa, [findMeetingTimes](../api/user-findmeetingtimes.md) sempre considera que a pessoa é do tipo `Required`.</span><span class="sxs-lookup"><span data-stu-id="ac963-117">Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="ac963-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ac963-118">emailAddress</span></span>|[<span data-ttu-id="ac963-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ac963-119">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="ac963-120">Inclui o nome e endereço SMTP do participante.</span><span class="sxs-lookup"><span data-stu-id="ac963-120">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
