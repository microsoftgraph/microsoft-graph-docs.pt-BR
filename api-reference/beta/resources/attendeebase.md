---
title: Tipo de recurso attendeeBase
description: O tipo de participante.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: harini84
ms.openlocfilehash: 5ad86fd3cd1ec6818c6f8466f5ff47a90b17dc94
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807196"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="c6736-103">Tipo de recurso attendeeBase</span><span class="sxs-lookup"><span data-stu-id="c6736-103">attendeeBase resource type</span></span>

<span data-ttu-id="c6736-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6736-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6736-105">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="c6736-105">The type of attendee.</span></span>

<span data-ttu-id="c6736-106">Derivado do [destinatário](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="c6736-106">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6736-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c6736-107">JSON representation</span></span>

<span data-ttu-id="c6736-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c6736-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="c6736-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c6736-109">Properties</span></span>
| <span data-ttu-id="c6736-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6736-110">Property</span></span>     | <span data-ttu-id="c6736-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6736-111">Type</span></span>   |<span data-ttu-id="c6736-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6736-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6736-113">type</span><span class="sxs-lookup"><span data-stu-id="c6736-113">type</span></span>|<span data-ttu-id="c6736-114">String</span><span class="sxs-lookup"><span data-stu-id="c6736-114">String</span></span>| <span data-ttu-id="c6736-p101">O tipo de participante. Os valores possíveis são: `required`, `optional`, `resource`. Atualmente, se o participante é uma pessoa, [findMeetingTimes](../api/user-findmeetingtimes.md) sempre considera que a pessoa é do tipo `Required`.</span><span class="sxs-lookup"><span data-stu-id="c6736-p101">The type of attendee. Possible values are: `required`, `optional`, `resource`. Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="c6736-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="c6736-118">emailAddress</span></span>|[<span data-ttu-id="c6736-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="c6736-119">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="c6736-120">Inclui o nome e endereço SMTP do participante.</span><span class="sxs-lookup"><span data-stu-id="c6736-120">Includes the name and SMTP address of the attendee.</span></span>|

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
