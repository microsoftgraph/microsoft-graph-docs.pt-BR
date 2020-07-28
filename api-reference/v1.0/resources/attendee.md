---
title: Tipo de recurso attendee
description: Um participante do evento. Pode ser uma pessoa ou recurso, como uma sala de reunião ou equipamento, que seja configurado como um recurso no Exchange Server para o locatário.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6c90d086afb7716dc3696443f18931f17cb291d9
ms.sourcegitcommit: 20b951f8bd245bb3a2bc7d3f5533e8619e9db084
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/27/2020
ms.locfileid: "45427239"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="e2f87-104">Tipo de recurso attendee</span><span class="sxs-lookup"><span data-stu-id="e2f87-104">attendee resource type</span></span>

<span data-ttu-id="e2f87-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2f87-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e2f87-106">Um participante do evento.</span><span class="sxs-lookup"><span data-stu-id="e2f87-106">An event attendee.</span></span> <span data-ttu-id="e2f87-107">Pode ser uma pessoa ou recurso, como uma sala de reunião ou equipamento, que seja configurado como um recurso no Exchange Server para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e2f87-107">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="e2f87-108">Derivado de [attendeeBase](attendeebase.md).</span><span class="sxs-lookup"><span data-stu-id="e2f87-108">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e2f87-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2f87-109">Properties</span></span>
| <span data-ttu-id="e2f87-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2f87-110">Property</span></span>     | <span data-ttu-id="e2f87-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2f87-111">Type</span></span>   |<span data-ttu-id="e2f87-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2f87-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2f87-113">emailAddress</span><span class="sxs-lookup"><span data-stu-id="e2f87-113">emailAddress</span></span>|[<span data-ttu-id="e2f87-114">emailAddress</span><span class="sxs-lookup"><span data-stu-id="e2f87-114">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="e2f87-115">Inclui o nome e endereço SMTP do participante.</span><span class="sxs-lookup"><span data-stu-id="e2f87-115">Includes the name and SMTP address of the attendee.</span></span>|
|<span data-ttu-id="e2f87-116">proposedNewTime</span><span class="sxs-lookup"><span data-stu-id="e2f87-116">proposedNewTime</span></span>|[<span data-ttu-id="e2f87-117">timeSlot</span><span class="sxs-lookup"><span data-stu-id="e2f87-117">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="e2f87-118">Uma data/hora alternativa proposta pelo participante para que uma solicitação de reunião inicie e termine.</span><span class="sxs-lookup"><span data-stu-id="e2f87-118">An alternate date/time proposed by the attendee for a meeting request to start and end.</span></span> <span data-ttu-id="e2f87-119">Se o participante não propôs outra vez, essa propriedade não é incluída em uma resposta de um evento GET.</span><span class="sxs-lookup"><span data-stu-id="e2f87-119">If the attendee hasn't proposed another time, then this property is not included in a response of a GET event.</span></span>|
|<span data-ttu-id="e2f87-120">status</span><span class="sxs-lookup"><span data-stu-id="e2f87-120">status</span></span>|[<span data-ttu-id="e2f87-121">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="e2f87-121">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="e2f87-122">A resposta do participante (nenhum, aceito, recusado, etc.) para o evento e a data e a hora em que a resposta foi enviada.</span><span class="sxs-lookup"><span data-stu-id="e2f87-122">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="e2f87-123">tipo</span><span class="sxs-lookup"><span data-stu-id="e2f87-123">type</span></span>|<span data-ttu-id="e2f87-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2f87-124">String</span></span>|<span data-ttu-id="e2f87-125">O tipo de participante: `required`, `optional` ou `resource`.</span><span class="sxs-lookup"><span data-stu-id="e2f87-125">The attendee type: `required`, `optional`, `resource`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2f87-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2f87-126">JSON representation</span></span>

<span data-ttu-id="e2f87-127">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e2f87-127">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attendeeBase",
  "optionalProperties": [
   "proposedNewTime"
  ],
  "@odata.type": "microsoft.graph.attendee"
}-->

```json
{
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "proposedNewTime": {"@odata.type": "microsoft.graph.timeSlot"},
  "status": {"@odata.type": "microsoft.graph.responseStatus"},
  "type": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
