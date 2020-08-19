---
title: Tipo de recurso attendee
description: Um participante do evento. Pode ser uma pessoa ou recurso, como uma sala de reunião ou equipamento, que seja configurado como um recurso no Exchange Server para o locatário.
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 858018ac269fdf16929e2f0efea6ec40bada7639
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808358"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="1463e-104">Tipo de recurso attendee</span><span class="sxs-lookup"><span data-stu-id="1463e-104">attendee resource type</span></span>

<span data-ttu-id="1463e-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1463e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1463e-106">Um participante do evento.</span><span class="sxs-lookup"><span data-stu-id="1463e-106">An event attendee.</span></span> <span data-ttu-id="1463e-107">Pode ser uma pessoa ou recurso, como uma sala de reunião ou equipamento, que seja configurado como um recurso no Exchange Server para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1463e-107">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="1463e-108">Derivado de [attendeeBase](attendeebase.md).</span><span class="sxs-lookup"><span data-stu-id="1463e-108">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1463e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1463e-109">Properties</span></span>
| <span data-ttu-id="1463e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1463e-110">Property</span></span>     | <span data-ttu-id="1463e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="1463e-111">Type</span></span>   |<span data-ttu-id="1463e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1463e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1463e-113">emailAddress</span><span class="sxs-lookup"><span data-stu-id="1463e-113">emailAddress</span></span>|[<span data-ttu-id="1463e-114">emailAddress</span><span class="sxs-lookup"><span data-stu-id="1463e-114">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="1463e-115">Inclui o nome e endereço SMTP do participante.</span><span class="sxs-lookup"><span data-stu-id="1463e-115">Includes the name and SMTP address of the attendee.</span></span>|
|<span data-ttu-id="1463e-116">proposedNewTime</span><span class="sxs-lookup"><span data-stu-id="1463e-116">proposedNewTime</span></span>|[<span data-ttu-id="1463e-117">timeSlot</span><span class="sxs-lookup"><span data-stu-id="1463e-117">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="1463e-118">Uma data/hora alternativa proposta pelo participante para que uma solicitação de reunião inicie e termine.</span><span class="sxs-lookup"><span data-stu-id="1463e-118">An alternate date/time proposed by the attendee for a meeting request to start and end.</span></span> <span data-ttu-id="1463e-119">Se o participante não propôs outra vez, essa propriedade não é incluída em uma resposta de um evento GET.</span><span class="sxs-lookup"><span data-stu-id="1463e-119">If the attendee hasn't proposed another time, then this property is not included in a response of a GET event.</span></span>|
|<span data-ttu-id="1463e-120">status</span><span class="sxs-lookup"><span data-stu-id="1463e-120">status</span></span>|[<span data-ttu-id="1463e-121">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="1463e-121">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="1463e-122">A resposta do participante (nenhum, aceito, recusado, etc.) para o evento e a data e a hora em que a resposta foi enviada.</span><span class="sxs-lookup"><span data-stu-id="1463e-122">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="1463e-123">type</span><span class="sxs-lookup"><span data-stu-id="1463e-123">type</span></span>|<span data-ttu-id="1463e-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1463e-124">String</span></span>|<span data-ttu-id="1463e-125">O tipo de participante: `required`, `optional` ou `resource`.</span><span class="sxs-lookup"><span data-stu-id="1463e-125">The attendee type: `required`, `optional`, `resource`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1463e-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1463e-126">JSON representation</span></span>

<span data-ttu-id="1463e-127">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="1463e-127">Here is a JSON representation of the resource</span></span>

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
