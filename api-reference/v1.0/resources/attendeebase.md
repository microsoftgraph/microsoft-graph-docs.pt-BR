---
title: Tipo de recurso attendeeBase
description: O tipo de participante.
localization_priority: Normal
ms.openlocfilehash: d009ef6a58c63017addf8b8a1bdecc1974abbff3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569350"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="8464a-103">Tipo de recurso attendeeBase</span><span class="sxs-lookup"><span data-stu-id="8464a-103">attendeeBase resource type</span></span>

<span data-ttu-id="8464a-104">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="8464a-104">The type of attendee.</span></span>

<span data-ttu-id="8464a-105">Derivado do [destinatário](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="8464a-105">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="8464a-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8464a-106">JSON representation</span></span>

<span data-ttu-id="8464a-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="8464a-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="8464a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8464a-108">Properties</span></span>
| <span data-ttu-id="8464a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8464a-109">Property</span></span>     | <span data-ttu-id="8464a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8464a-110">Type</span></span>   |<span data-ttu-id="8464a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8464a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8464a-112">type</span><span class="sxs-lookup"><span data-stu-id="8464a-112">type</span></span>|<span data-ttu-id="8464a-113">articipantetype</span><span class="sxs-lookup"><span data-stu-id="8464a-113">attendeeType</span></span>| <span data-ttu-id="8464a-114">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="8464a-114">The type of attendee.</span></span> <span data-ttu-id="8464a-115">Os valores possíveis são: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="8464a-115">The possible values are: `required`, `optional`, `resource`.</span></span> <span data-ttu-id="8464a-116">Atualmente, se o participante é uma pessoa, [findMeetingTimes](../api/user-findmeetingtimes.md) sempre considera que a pessoa é do tipo `Required`.</span><span class="sxs-lookup"><span data-stu-id="8464a-116">Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="8464a-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8464a-117">emailAddress</span></span>|[<span data-ttu-id="8464a-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8464a-118">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="8464a-119">Inclui o nome e endereço SMTP do participante.</span><span class="sxs-lookup"><span data-stu-id="8464a-119">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
