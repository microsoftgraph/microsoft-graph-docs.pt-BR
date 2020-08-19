---
title: Tipo de recurso reminder
description: Um lembrete para um evento em um calendário do usuário.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: harini84
ms.openlocfilehash: 906e860cd6bab507a0acf89d561ccd8aeb1d1468
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812453"
---
# <a name="reminder-resource-type"></a><span data-ttu-id="edb12-103">Tipo de recurso reminder</span><span class="sxs-lookup"><span data-stu-id="edb12-103">reminder resource type</span></span>

<span data-ttu-id="edb12-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edb12-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edb12-105">Um lembrete para um [evento](event.md) em um [calendário](calendar.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="edb12-105">A reminder for an [event](event.md) in a user [calendar](calendar.md).</span></span>

## <a name="properties"></a><span data-ttu-id="edb12-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="edb12-106">Properties</span></span>
| <span data-ttu-id="edb12-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="edb12-107">Property</span></span>     | <span data-ttu-id="edb12-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="edb12-108">Type</span></span>   |<span data-ttu-id="edb12-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="edb12-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="edb12-110">changeKey</span><span class="sxs-lookup"><span data-stu-id="edb12-110">changeKey</span></span>|<span data-ttu-id="edb12-111">String</span><span class="sxs-lookup"><span data-stu-id="edb12-111">String</span></span>|<span data-ttu-id="edb12-p101">Identifica a versão do lembrete. Toda vez que o lembrete é alterado, **changeKey** também muda. Isso permite que o Exchange aplique as alterações na versão correta do objeto.</span><span class="sxs-lookup"><span data-stu-id="edb12-p101">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="edb12-115">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="edb12-115">eventEndTime</span></span>|[<span data-ttu-id="edb12-116">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="edb12-116">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="edb12-117">A data, a hora e o fuso horário em que o evento termina.</span><span class="sxs-lookup"><span data-stu-id="edb12-117">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="edb12-118">eventId</span><span class="sxs-lookup"><span data-stu-id="edb12-118">eventId</span></span>|<span data-ttu-id="edb12-119">String</span><span class="sxs-lookup"><span data-stu-id="edb12-119">String</span></span>|<span data-ttu-id="edb12-p102">A ID exclusiva do evento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="edb12-p102">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="edb12-122">eventLocation</span><span class="sxs-lookup"><span data-stu-id="edb12-122">eventLocation</span></span>|[<span data-ttu-id="edb12-123">Location</span><span class="sxs-lookup"><span data-stu-id="edb12-123">Location</span></span>](location.md)|<span data-ttu-id="edb12-124">O local do evento.</span><span class="sxs-lookup"><span data-stu-id="edb12-124">The location of the event.</span></span>|
|<span data-ttu-id="edb12-125">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="edb12-125">eventStartTime</span></span>|[<span data-ttu-id="edb12-126">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="edb12-126">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="edb12-127">A data, a hora e o fuso horário em que o evento começa.</span><span class="sxs-lookup"><span data-stu-id="edb12-127">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="edb12-128">eventSubject</span><span class="sxs-lookup"><span data-stu-id="edb12-128">eventSubject</span></span>|<span data-ttu-id="edb12-129">String</span><span class="sxs-lookup"><span data-stu-id="edb12-129">String</span></span>|<span data-ttu-id="edb12-130">O texto da linha de assunto do evento.</span><span class="sxs-lookup"><span data-stu-id="edb12-130">The text of the event's subject line.</span></span>|
|<span data-ttu-id="edb12-131">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="edb12-131">eventWebLink</span></span>|<span data-ttu-id="edb12-132">String</span><span class="sxs-lookup"><span data-stu-id="edb12-132">String</span></span>|<span data-ttu-id="edb12-133">A URL para abrir o evento no Outlook na Web.</span><span class="sxs-lookup"><span data-stu-id="edb12-133">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="edb12-p103">O evento será aberto no navegador se você estiver conectado à sua caixa de correio através do Outlook na Web. Você será solicitado a fazer login se já não estiver conectado no navegador.</span><span class="sxs-lookup"><span data-stu-id="edb12-p103">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="edb12-136">Essa URL pode ser acessada de um iFrame.</span><span class="sxs-lookup"><span data-stu-id="edb12-136">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="edb12-137">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="edb12-137">reminderFireTime</span></span>|[<span data-ttu-id="edb12-138">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="edb12-138">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="edb12-139">A data, a hora e o fuso horário do lembrete.</span><span class="sxs-lookup"><span data-stu-id="edb12-139">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="edb12-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="edb12-140">JSON representation</span></span>

<span data-ttu-id="edb12-141">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="edb12-141">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "reminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
