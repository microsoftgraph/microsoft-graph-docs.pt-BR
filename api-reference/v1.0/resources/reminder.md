# <a name="reminder-resource-type"></a><span data-ttu-id="5813e-101">tipo de recurso de lembrete</span><span class="sxs-lookup"><span data-stu-id="5813e-101">reminder resource type</span></span>

<span data-ttu-id="5813e-102">Um lembrete para um [evento](event.md) no [calendário](calendar.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="5813e-102">A reminder for an [event](event.md) in a user [calendar](calendar.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5813e-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5813e-103">Properties</span></span>
| <span data-ttu-id="5813e-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5813e-104">Property</span></span>     | <span data-ttu-id="5813e-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="5813e-105">Type</span></span>   |<span data-ttu-id="5813e-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="5813e-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5813e-107">changeKey</span><span class="sxs-lookup"><span data-stu-id="5813e-107">changeKey</span></span>|<span data-ttu-id="5813e-108">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="5813e-108">String</span></span>|<span data-ttu-id="5813e-p101">Identifica a versão do lembrete. Toda vez que o lembrete é alterado, **changeKey** também muda. Isso permite que o Exchange aplique as alterações na versão correta do objeto.</span><span class="sxs-lookup"><span data-stu-id="5813e-p101">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="5813e-112">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="5813e-112">eventEndTime</span></span>|[<span data-ttu-id="5813e-113">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5813e-113">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="5813e-114">A data, a hora e o fuso horário em que o evento termina.</span><span class="sxs-lookup"><span data-stu-id="5813e-114">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="5813e-115">eventId</span><span class="sxs-lookup"><span data-stu-id="5813e-115">eventId</span></span>|<span data-ttu-id="5813e-116">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="5813e-116">String</span></span>|<span data-ttu-id="5813e-p102">A ID exclusiva do evento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5813e-p102">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="5813e-119">eventLocation</span><span class="sxs-lookup"><span data-stu-id="5813e-119">eventLocation</span></span>|[<span data-ttu-id="5813e-120">Localização</span><span class="sxs-lookup"><span data-stu-id="5813e-120">Location</span></span>](location.md)|<span data-ttu-id="5813e-121">O local do evento.</span><span class="sxs-lookup"><span data-stu-id="5813e-121">The location of the event.</span></span>|
|<span data-ttu-id="5813e-122">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="5813e-122">eventStartTime</span></span>|[<span data-ttu-id="5813e-123">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5813e-123">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="5813e-124">A data, a hora e o fuso horário em que o evento começa.</span><span class="sxs-lookup"><span data-stu-id="5813e-124">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="5813e-125">eventSubject</span><span class="sxs-lookup"><span data-stu-id="5813e-125">eventSubject</span></span>|<span data-ttu-id="5813e-126">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="5813e-126">String</span></span>|<span data-ttu-id="5813e-127">O texto da linha de assunto do evento.</span><span class="sxs-lookup"><span data-stu-id="5813e-127">The text of the event's subject line.</span></span>|
|<span data-ttu-id="5813e-128">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="5813e-128">eventWebLink</span></span>|<span data-ttu-id="5813e-129">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="5813e-129">String</span></span>|<span data-ttu-id="5813e-130">A URL para abrir o evento no Outlook na Web.</span><span class="sxs-lookup"><span data-stu-id="5813e-130">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="5813e-p103">O evento será aberto no navegador se você estiver conectado à sua caixa de correio através do Outlook na Web. Você será solicitado a fazer login se já não estiver conectado no navegador.</span><span class="sxs-lookup"><span data-stu-id="5813e-p103">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="5813e-133">Essa URL pode ser acessada de um iFrame.</span><span class="sxs-lookup"><span data-stu-id="5813e-133">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="5813e-134">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="5813e-134">reminderFireTime</span></span>|[<span data-ttu-id="5813e-135">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5813e-135">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="5813e-136">A data, a hora e o fuso horário do lembrete.</span><span class="sxs-lookup"><span data-stu-id="5813e-136">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5813e-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5813e-137">JSON representation</span></span>

<span data-ttu-id="5813e-138">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="5813e-138">Here is a JSON representation of the resource</span></span>

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