# <a name="reminder-resource-type"></a><span data-ttu-id="3cc89-101">Tipo de recurso reminder</span><span class="sxs-lookup"><span data-stu-id="3cc89-101">reminder resource type</span></span>



## <a name="properties"></a><span data-ttu-id="3cc89-102">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3cc89-102">Properties</span></span>
| <span data-ttu-id="3cc89-103">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3cc89-103">Property</span></span>     | <span data-ttu-id="3cc89-104">Tipo</span><span class="sxs-lookup"><span data-stu-id="3cc89-104">Type</span></span>   |<span data-ttu-id="3cc89-105">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cc89-105">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3cc89-106">changeKey</span><span class="sxs-lookup"><span data-stu-id="3cc89-106">changeKey</span></span>|<span data-ttu-id="3cc89-107">String</span><span class="sxs-lookup"><span data-stu-id="3cc89-107">String</span></span>|<span data-ttu-id="3cc89-p101">Identifica a versão do lembrete. Toda vez que o lembrete é alterado, **changeKey** também muda. Isso permite que o Exchange aplique as alterações na versão correta do objeto.</span><span class="sxs-lookup"><span data-stu-id="3cc89-p101">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="3cc89-111">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="3cc89-111">eventEndTime</span></span>|[<span data-ttu-id="3cc89-112">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3cc89-112">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="3cc89-113">A data, a hora e o fuso horário em que o evento termina.</span><span class="sxs-lookup"><span data-stu-id="3cc89-113">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="3cc89-114">eventId</span><span class="sxs-lookup"><span data-stu-id="3cc89-114">eventId</span></span>|<span data-ttu-id="3cc89-115">String</span><span class="sxs-lookup"><span data-stu-id="3cc89-115">String</span></span>|<span data-ttu-id="3cc89-p102">A ID exclusiva do evento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3cc89-p102">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="3cc89-118">eventLocation</span><span class="sxs-lookup"><span data-stu-id="3cc89-118">eventLocation</span></span>|[<span data-ttu-id="3cc89-119">Location</span><span class="sxs-lookup"><span data-stu-id="3cc89-119">Location</span></span>](location.md)|<span data-ttu-id="3cc89-120">O local do evento.</span><span class="sxs-lookup"><span data-stu-id="3cc89-120">The location of the event.</span></span>|
|<span data-ttu-id="3cc89-121">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="3cc89-121">eventStartTime</span></span>|[<span data-ttu-id="3cc89-122">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3cc89-122">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="3cc89-123">A data, a hora e o fuso horário em que o evento começa.</span><span class="sxs-lookup"><span data-stu-id="3cc89-123">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="3cc89-124">eventSubject</span><span class="sxs-lookup"><span data-stu-id="3cc89-124">eventSubject</span></span>|<span data-ttu-id="3cc89-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3cc89-125">String</span></span>|<span data-ttu-id="3cc89-126">O texto da linha de assunto do evento.</span><span class="sxs-lookup"><span data-stu-id="3cc89-126">The text of the event's subject line.</span></span>|
|<span data-ttu-id="3cc89-127">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="3cc89-127">eventWebLink</span></span>|<span data-ttu-id="3cc89-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3cc89-128">String</span></span>|<span data-ttu-id="3cc89-129">A URL para abrir o evento no Outlook na Web.</span><span class="sxs-lookup"><span data-stu-id="3cc89-129">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="3cc89-p103">O evento será aberto no navegador se você estiver conectado à sua caixa de correio através do Outlook na Web. Você será solicitado a fazer login se já não estiver conectado no navegador.</span><span class="sxs-lookup"><span data-stu-id="3cc89-p103">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="3cc89-132">Essa URL pode ser acessada de um iFrame.</span><span class="sxs-lookup"><span data-stu-id="3cc89-132">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="3cc89-133">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="3cc89-133">reminderFireTime</span></span>|[<span data-ttu-id="3cc89-134">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3cc89-134">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="3cc89-135">A data, a hora e o fuso horário do lembrete.</span><span class="sxs-lookup"><span data-stu-id="3cc89-135">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3cc89-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3cc89-136">JSON representation</span></span>

<span data-ttu-id="3cc89-137">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="3cc89-137">Here is a JSON representation of the resource</span></span>

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