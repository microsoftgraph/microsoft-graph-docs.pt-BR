---
title: Tipo de recurso reminder
description: Um lembrete para um evento em um calendário do usuário.
ms.openlocfilehash: e7b7e2266b5959c6aa4927ecad52e24342d607e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036454"
---
# <a name="reminder-resource-type"></a><span data-ttu-id="99c59-103">Tipo de recurso reminder</span><span class="sxs-lookup"><span data-stu-id="99c59-103">reminder resource type</span></span>

> <span data-ttu-id="99c59-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="99c59-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99c59-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="99c59-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="99c59-106">Um lembrete para um [evento](event.md) em um [calendário](calendar.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="99c59-106">A reminder for an [event](event.md) in a user [calendar](calendar.md).</span></span>

## <a name="properties"></a><span data-ttu-id="99c59-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="99c59-107">Properties</span></span>
| <span data-ttu-id="99c59-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99c59-108">Property</span></span>     | <span data-ttu-id="99c59-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="99c59-109">Type</span></span>   |<span data-ttu-id="99c59-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="99c59-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99c59-111">changeKey</span><span class="sxs-lookup"><span data-stu-id="99c59-111">changeKey</span></span>|<span data-ttu-id="99c59-112">String</span><span class="sxs-lookup"><span data-stu-id="99c59-112">String</span></span>|<span data-ttu-id="99c59-p102">Identifica a versão do lembrete. Toda vez que o lembrete é alterado, **changeKey** também muda. Isso permite que o Exchange aplique as alterações na versão correta do objeto.</span><span class="sxs-lookup"><span data-stu-id="99c59-p102">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="99c59-116">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="99c59-116">eventEndTime</span></span>|[<span data-ttu-id="99c59-117">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="99c59-117">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="99c59-118">A data, a hora e o fuso horário em que o evento termina.</span><span class="sxs-lookup"><span data-stu-id="99c59-118">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="99c59-119">eventId</span><span class="sxs-lookup"><span data-stu-id="99c59-119">eventId</span></span>|<span data-ttu-id="99c59-120">String</span><span class="sxs-lookup"><span data-stu-id="99c59-120">String</span></span>|<span data-ttu-id="99c59-p103">A ID exclusiva do evento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="99c59-p103">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="99c59-123">eventLocation</span><span class="sxs-lookup"><span data-stu-id="99c59-123">eventLocation</span></span>|[<span data-ttu-id="99c59-124">Location</span><span class="sxs-lookup"><span data-stu-id="99c59-124">Location</span></span>](location.md)|<span data-ttu-id="99c59-125">O local do evento.</span><span class="sxs-lookup"><span data-stu-id="99c59-125">The location of the event.</span></span>|
|<span data-ttu-id="99c59-126">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="99c59-126">eventStartTime</span></span>|[<span data-ttu-id="99c59-127">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="99c59-127">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="99c59-128">A data, a hora e o fuso horário em que o evento começa.</span><span class="sxs-lookup"><span data-stu-id="99c59-128">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="99c59-129">eventSubject</span><span class="sxs-lookup"><span data-stu-id="99c59-129">eventSubject</span></span>|<span data-ttu-id="99c59-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99c59-130">String</span></span>|<span data-ttu-id="99c59-131">O texto da linha de assunto do evento.</span><span class="sxs-lookup"><span data-stu-id="99c59-131">The text of the event's subject line.</span></span>|
|<span data-ttu-id="99c59-132">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="99c59-132">eventWebLink</span></span>|<span data-ttu-id="99c59-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99c59-133">String</span></span>|<span data-ttu-id="99c59-134">A URL para abrir o evento no Outlook na Web.</span><span class="sxs-lookup"><span data-stu-id="99c59-134">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="99c59-p104">O evento será aberto no navegador se você estiver conectado à sua caixa de correio através do Outlook na Web. Você será solicitado a fazer login se já não estiver conectado no navegador.</span><span class="sxs-lookup"><span data-stu-id="99c59-p104">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="99c59-137">Essa URL pode ser acessada de um iFrame.</span><span class="sxs-lookup"><span data-stu-id="99c59-137">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="99c59-138">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="99c59-138">reminderFireTime</span></span>|[<span data-ttu-id="99c59-139">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="99c59-139">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="99c59-140">A data, a hora e o fuso horário do lembrete.</span><span class="sxs-lookup"><span data-stu-id="99c59-140">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="99c59-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="99c59-141">JSON representation</span></span>

<span data-ttu-id="99c59-142">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="99c59-142">Here is a JSON representation of the resource</span></span>

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