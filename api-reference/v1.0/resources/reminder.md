---
title: Tipo de recurso reminder
description: Um lembrete para um evento em um calendário do usuário.
localization_priority: Normal
ms.openlocfilehash: e8aa591f078b90249b36d3dc2f666ddac4502461
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579342"
---
# <a name="reminder-resource-type"></a><span data-ttu-id="6d93d-103">Tipo de recurso reminder</span><span class="sxs-lookup"><span data-stu-id="6d93d-103">reminder resource type</span></span>

<span data-ttu-id="6d93d-104">Um lembrete para um [evento](event.md) em um [calendário](calendar.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="6d93d-104">A reminder for an [event](event.md) in a user [calendar](calendar.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6d93d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d93d-105">Properties</span></span>
| <span data-ttu-id="6d93d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d93d-106">Property</span></span>     | <span data-ttu-id="6d93d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d93d-107">Type</span></span>   |<span data-ttu-id="6d93d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d93d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d93d-109">changeKey</span><span class="sxs-lookup"><span data-stu-id="6d93d-109">changeKey</span></span>|<span data-ttu-id="6d93d-110">String</span><span class="sxs-lookup"><span data-stu-id="6d93d-110">String</span></span>|<span data-ttu-id="6d93d-p101">Identifica a versão do lembrete. Toda vez que o lembrete é alterado, **changeKey** também muda. Isso permite que o Exchange aplique as alterações na versão correta do objeto.</span><span class="sxs-lookup"><span data-stu-id="6d93d-p101">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="6d93d-114">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="6d93d-114">eventEndTime</span></span>|[<span data-ttu-id="6d93d-115">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6d93d-115">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="6d93d-116">A data, a hora e o fuso horário em que o evento termina.</span><span class="sxs-lookup"><span data-stu-id="6d93d-116">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="6d93d-117">eventId</span><span class="sxs-lookup"><span data-stu-id="6d93d-117">eventId</span></span>|<span data-ttu-id="6d93d-118">String</span><span class="sxs-lookup"><span data-stu-id="6d93d-118">String</span></span>|<span data-ttu-id="6d93d-p102">A ID exclusiva do evento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d93d-p102">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="6d93d-121">eventLocation</span><span class="sxs-lookup"><span data-stu-id="6d93d-121">eventLocation</span></span>|[<span data-ttu-id="6d93d-122">Location</span><span class="sxs-lookup"><span data-stu-id="6d93d-122">Location</span></span>](location.md)|<span data-ttu-id="6d93d-123">O local do evento.</span><span class="sxs-lookup"><span data-stu-id="6d93d-123">The location of the event.</span></span>|
|<span data-ttu-id="6d93d-124">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="6d93d-124">eventStartTime</span></span>|[<span data-ttu-id="6d93d-125">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6d93d-125">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="6d93d-126">A data, a hora e o fuso horário em que o evento começa.</span><span class="sxs-lookup"><span data-stu-id="6d93d-126">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="6d93d-127">eventSubject</span><span class="sxs-lookup"><span data-stu-id="6d93d-127">eventSubject</span></span>|<span data-ttu-id="6d93d-128">String</span><span class="sxs-lookup"><span data-stu-id="6d93d-128">String</span></span>|<span data-ttu-id="6d93d-129">O texto da linha de assunto do evento.</span><span class="sxs-lookup"><span data-stu-id="6d93d-129">The text of the event's subject line.</span></span>|
|<span data-ttu-id="6d93d-130">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="6d93d-130">eventWebLink</span></span>|<span data-ttu-id="6d93d-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d93d-131">String</span></span>|<span data-ttu-id="6d93d-132">A URL para abrir o evento no Outlook na Web.</span><span class="sxs-lookup"><span data-stu-id="6d93d-132">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="6d93d-p103">O evento será aberto no navegador se você estiver conectado à sua caixa de correio através do Outlook na Web. Você será solicitado a fazer login se já não estiver conectado no navegador.</span><span class="sxs-lookup"><span data-stu-id="6d93d-p103">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="6d93d-135">Essa URL pode ser acessada de um iFrame.</span><span class="sxs-lookup"><span data-stu-id="6d93d-135">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="6d93d-136">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="6d93d-136">reminderFireTime</span></span>|[<span data-ttu-id="6d93d-137">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6d93d-137">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="6d93d-138">A data, a hora e o fuso horário do lembrete.</span><span class="sxs-lookup"><span data-stu-id="6d93d-138">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6d93d-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d93d-139">JSON representation</span></span>

<span data-ttu-id="6d93d-140">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="6d93d-140">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reminder"
}-->

```json
{
  "changeKey": "string",
  "eventEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventId": "string",
  "eventLocation": {"@odata.type": "microsoft.graph.location"},
  "eventStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventSubject": "string",
  "eventWebLink": "string",
  "reminderFireTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
