---
title: Tipo de recurso attendeeBase
description: O tipo de participante.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 154584a91fc8844e2745d5198773157c4dfe26d1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033107"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="98b35-103">Tipo de recurso attendeeBase</span><span class="sxs-lookup"><span data-stu-id="98b35-103">attendeeBase resource type</span></span>

<span data-ttu-id="98b35-104">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="98b35-104">The type of attendee.</span></span>

<span data-ttu-id="98b35-105">Derivado do [destinatário](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="98b35-105">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="98b35-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="98b35-106">JSON representation</span></span>

<span data-ttu-id="98b35-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="98b35-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="98b35-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="98b35-108">Properties</span></span>
| <span data-ttu-id="98b35-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98b35-109">Property</span></span>     | <span data-ttu-id="98b35-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="98b35-110">Type</span></span>   |<span data-ttu-id="98b35-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="98b35-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98b35-112">type</span><span class="sxs-lookup"><span data-stu-id="98b35-112">type</span></span>|<span data-ttu-id="98b35-113">articipantetype</span><span class="sxs-lookup"><span data-stu-id="98b35-113">attendeeType</span></span>| <span data-ttu-id="98b35-114">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="98b35-114">The type of attendee.</span></span> <span data-ttu-id="98b35-115">Os valores possíveis são: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="98b35-115">The possible values are: `required`, `optional`, `resource`.</span></span> <span data-ttu-id="98b35-116">Atualmente, se o participante é uma pessoa, [findMeetingTimes](../api/user-findmeetingtimes.md) sempre considera que a pessoa é do tipo `Required`.</span><span class="sxs-lookup"><span data-stu-id="98b35-116">Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="98b35-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="98b35-117">emailAddress</span></span>|[<span data-ttu-id="98b35-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="98b35-118">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="98b35-119">Inclui o nome e endereço SMTP do participante.</span><span class="sxs-lookup"><span data-stu-id="98b35-119">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
