---
title: Tipo de recurso attendee
description: Um participante do evento. Pode ser uma pessoa ou recurso, como uma sala de reunião ou equipamento, que seja configurado como um recurso no Exchange Server para o locatário.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: 4e906a2f7f9d95cd3c3623d1f84c41aedded6cc4
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37621584"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="a226a-104">Tipo de recurso attendee</span><span class="sxs-lookup"><span data-stu-id="a226a-104">attendee resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a226a-105">Um participante do evento.</span><span class="sxs-lookup"><span data-stu-id="a226a-105">An event attendee.</span></span> <span data-ttu-id="a226a-106">Pode ser uma pessoa ou recurso, como uma sala de reunião ou equipamento, que seja configurado como um recurso no Exchange Server para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a226a-106">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="a226a-107">Derivado de [attendeeBase](attendeebase.md).</span><span class="sxs-lookup"><span data-stu-id="a226a-107">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a226a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a226a-108">Properties</span></span>
| <span data-ttu-id="a226a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a226a-109">Property</span></span>     | <span data-ttu-id="a226a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a226a-110">Type</span></span>   |<span data-ttu-id="a226a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a226a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a226a-112">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a226a-112">emailAddress</span></span>|[<span data-ttu-id="a226a-113">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a226a-113">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="a226a-114">Inclui o nome e endereço SMTP do participante.</span><span class="sxs-lookup"><span data-stu-id="a226a-114">Includes the name and SMTP address of the attendee.</span></span>|
|<span data-ttu-id="a226a-115">proposedNewTime</span><span class="sxs-lookup"><span data-stu-id="a226a-115">proposedNewTime</span></span>|[<span data-ttu-id="a226a-116">timeSlot</span><span class="sxs-lookup"><span data-stu-id="a226a-116">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="a226a-117">Uma data/hora alternativa proposta pelo participante para que uma solicitação de reunião inicie e termine.</span><span class="sxs-lookup"><span data-stu-id="a226a-117">An alternate date/time proposed by the attendee for a meeting request to start and end.</span></span> <span data-ttu-id="a226a-118">Se o participante não propôs outra vez, essa propriedade não é incluída em uma resposta de um evento GET.</span><span class="sxs-lookup"><span data-stu-id="a226a-118">If the attendee hasn't proposed another time, then this property is not included in a response of a GET event.</span></span>|
|<span data-ttu-id="a226a-119">status</span><span class="sxs-lookup"><span data-stu-id="a226a-119">status</span></span>|[<span data-ttu-id="a226a-120">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="a226a-120">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="a226a-121">A resposta do participante (nenhum, aceito, recusado, etc.) para o evento e a data e a hora em que a resposta foi enviada.</span><span class="sxs-lookup"><span data-stu-id="a226a-121">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="a226a-122">type</span><span class="sxs-lookup"><span data-stu-id="a226a-122">type</span></span>|<span data-ttu-id="a226a-123">String</span><span class="sxs-lookup"><span data-stu-id="a226a-123">String</span></span>|<span data-ttu-id="a226a-124">O tipo de participante: `required`, `optional` ou `resource`.</span><span class="sxs-lookup"><span data-stu-id="a226a-124">The attendee type: `required`, `optional`, `resource`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a226a-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a226a-125">JSON representation</span></span>

<span data-ttu-id="a226a-126">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a226a-126">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
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
<!--
{
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
