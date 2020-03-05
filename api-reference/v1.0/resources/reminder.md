---
title: Tipo de recurso reminder
description: Um lembrete para um evento em um calendário do usuário.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: cc07c6e8b787925e9ee72dbb949997c18ca70f87
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446986"
---
# <a name="reminder-resource-type"></a><span data-ttu-id="e32be-103">Tipo de recurso reminder</span><span class="sxs-lookup"><span data-stu-id="e32be-103">reminder resource type</span></span>

<span data-ttu-id="e32be-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e32be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e32be-105">Um lembrete para um [evento](event.md) em um [calendário](calendar.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="e32be-105">A reminder for an [event](event.md) in a user [calendar](calendar.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e32be-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e32be-106">Properties</span></span>
| <span data-ttu-id="e32be-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e32be-107">Property</span></span>     | <span data-ttu-id="e32be-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e32be-108">Type</span></span>   |<span data-ttu-id="e32be-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e32be-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e32be-110">changeKey</span><span class="sxs-lookup"><span data-stu-id="e32be-110">changeKey</span></span>|<span data-ttu-id="e32be-111">String</span><span class="sxs-lookup"><span data-stu-id="e32be-111">String</span></span>|<span data-ttu-id="e32be-p101">Identifica a versão do lembrete. Toda vez que o lembrete é alterado, **changeKey** também muda. Isso permite que o Exchange aplique as alterações na versão correta do objeto.</span><span class="sxs-lookup"><span data-stu-id="e32be-p101">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="e32be-115">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="e32be-115">eventEndTime</span></span>|[<span data-ttu-id="e32be-116">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e32be-116">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="e32be-117">A data, a hora e o fuso horário em que o evento termina.</span><span class="sxs-lookup"><span data-stu-id="e32be-117">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="e32be-118">eventId</span><span class="sxs-lookup"><span data-stu-id="e32be-118">eventId</span></span>|<span data-ttu-id="e32be-119">String</span><span class="sxs-lookup"><span data-stu-id="e32be-119">String</span></span>|<span data-ttu-id="e32be-p102">A ID exclusiva do evento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e32be-p102">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="e32be-122">eventLocation</span><span class="sxs-lookup"><span data-stu-id="e32be-122">eventLocation</span></span>|[<span data-ttu-id="e32be-123">Location</span><span class="sxs-lookup"><span data-stu-id="e32be-123">Location</span></span>](location.md)|<span data-ttu-id="e32be-124">O local do evento.</span><span class="sxs-lookup"><span data-stu-id="e32be-124">The location of the event.</span></span>|
|<span data-ttu-id="e32be-125">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="e32be-125">eventStartTime</span></span>|[<span data-ttu-id="e32be-126">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e32be-126">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="e32be-127">A data, a hora e o fuso horário em que o evento começa.</span><span class="sxs-lookup"><span data-stu-id="e32be-127">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="e32be-128">eventSubject</span><span class="sxs-lookup"><span data-stu-id="e32be-128">eventSubject</span></span>|<span data-ttu-id="e32be-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e32be-129">String</span></span>|<span data-ttu-id="e32be-130">O texto da linha de assunto do evento.</span><span class="sxs-lookup"><span data-stu-id="e32be-130">The text of the event's subject line.</span></span>|
|<span data-ttu-id="e32be-131">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="e32be-131">eventWebLink</span></span>|<span data-ttu-id="e32be-132">String</span><span class="sxs-lookup"><span data-stu-id="e32be-132">String</span></span>|<span data-ttu-id="e32be-133">A URL para abrir o evento no Outlook na Web.</span><span class="sxs-lookup"><span data-stu-id="e32be-133">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="e32be-p103">O evento será aberto no navegador se você estiver conectado à sua caixa de correio através do Outlook na Web. Você será solicitado a fazer login se já não estiver conectado no navegador.</span><span class="sxs-lookup"><span data-stu-id="e32be-p103">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="e32be-136">Essa URL pode ser acessada de um iFrame.</span><span class="sxs-lookup"><span data-stu-id="e32be-136">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="e32be-137">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="e32be-137">reminderFireTime</span></span>|[<span data-ttu-id="e32be-138">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e32be-138">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="e32be-139">A data, a hora e o fuso horário do lembrete.</span><span class="sxs-lookup"><span data-stu-id="e32be-139">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e32be-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e32be-140">JSON representation</span></span>

<span data-ttu-id="e32be-141">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e32be-141">Here is a JSON representation of the resource</span></span>

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
