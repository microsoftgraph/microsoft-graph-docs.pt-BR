# <a name="daylighttimezoneoffset-resource-type"></a><span data-ttu-id="b3b7b-101">Tipo de recurso daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="b3b7b-101">daylightTimeZoneOffset resource type</span></span>

<span data-ttu-id="b3b7b-102">Especifica quando um fuso horário muda do horário padrão para o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="b3b7b-102">Specifies when a time zone switches from standard time to daylight saving time.</span></span>

<span data-ttu-id="b3b7b-103">Por exemplo, se um fuso horário estiver especificado com as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="b3b7b-103">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="b3b7b-104">**bias** como 300</span><span class="sxs-lookup"><span data-stu-id="b3b7b-104">**bias** is 300</span></span>
- <span data-ttu-id="b3b7b-105">**daylightBias** como -100</span><span class="sxs-lookup"><span data-stu-id="b3b7b-105">**daylightBias** is -100</span></span>
- <span data-ttu-id="b3b7b-106">**dayOccurrence** como 4</span><span class="sxs-lookup"><span data-stu-id="b3b7b-106">**dayOccurrence** is 4</span></span>
- <span data-ttu-id="b3b7b-107">**dayOfWeek** como "domingo"</span><span class="sxs-lookup"><span data-stu-id="b3b7b-107">**dayOfWeek** is "sunday"</span></span>
- <span data-ttu-id="b3b7b-108">**month** como 5</span><span class="sxs-lookup"><span data-stu-id="b3b7b-108">**month** is 5</span></span>
- <span data-ttu-id="b3b7b-109">**time** como 02:00:00 _**year** como 0, significa que a hora durante o horário de verão é +300-100=200 minutos adiantada ao UTC.</span><span class="sxs-lookup"><span data-stu-id="b3b7b-109">**time** is 02:00:00 _ **year** is 0 That means the time during daylight saving time is +300-100=200 minutes ahead of UTC.</span></span> <span data-ttu-id="b3b7b-110">A transição do fuso horário de horário de verão para o horário padrão ocorre às 2 da manhã no quarto domingo de maio, todos os anos.</span><span class="sxs-lookup"><span data-stu-id="b3b7b-110">The time zone transition from daylight saving time to standard occurs at 2 AM on the fourth Sunday of May, every year.</span></span>


## <a name="properties"></a><span data-ttu-id="b3b7b-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b3b7b-111">Properties</span></span>
| <span data-ttu-id="b3b7b-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3b7b-112">Property</span></span>     | <span data-ttu-id="b3b7b-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3b7b-113">Type</span></span>   |<span data-ttu-id="b3b7b-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3b7b-114">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b3b7b-115">daylightBias</span><span class="sxs-lookup"><span data-stu-id="b3b7b-115">daylightBias</span></span> | <span data-ttu-id="b3b7b-116">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="b3b7b-116">Edm.Int32</span></span> | <span data-ttu-id="b3b7b-117">A diferença de horário em relação ao UTC (Tempo Universal Coordenado) para o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="b3b7b-117">The time offset from Coordinated Universal Time (UTC) for daylight saving time.</span></span> <span data-ttu-id="b3b7b-118">Este valor está em minutos.</span><span class="sxs-lookup"><span data-stu-id="b3b7b-118">This value is in minutes.</span></span>  |
| <span data-ttu-id="b3b7b-119">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="b3b7b-119">dayOccurrence</span></span> | <span data-ttu-id="b3b7b-120">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="b3b7b-120">Edm.Int32</span></span> | <span data-ttu-id="b3b7b-121">Representa a enésima ocorrência do dia da semana em que a transição do horário padrão para o horário de verão acontece.</span><span class="sxs-lookup"><span data-stu-id="b3b7b-121">Represents the nth occurrence of the day of week that the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="b3b7b-122">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="b3b7b-122">dayOfWeek</span></span> | <span data-ttu-id="b3b7b-123">string</span><span class="sxs-lookup"><span data-stu-id="b3b7b-123">string</span></span> | <span data-ttu-id="b3b7b-124">Representa o dia da semana em que a transição do horário padrão para o horário de verão acontece.</span><span class="sxs-lookup"><span data-stu-id="b3b7b-124">Represents the day of the week when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="b3b7b-125">month</span><span class="sxs-lookup"><span data-stu-id="b3b7b-125">month</span></span> | <span data-ttu-id="b3b7b-126">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="b3b7b-126">Edm.Int32</span></span> | <span data-ttu-id="b3b7b-127">Representa o mês do ano em que a transição do horário padrão para o horário de verão acontece.</span><span class="sxs-lookup"><span data-stu-id="b3b7b-127">Represents the month of the year when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="b3b7b-128">time</span><span class="sxs-lookup"><span data-stu-id="b3b7b-128">time</span></span> | <span data-ttu-id="b3b7b-129">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b3b7b-129">Edm.TimeOfDay</span></span> | <span data-ttu-id="b3b7b-130">Representa a hora do dia em que a transição do horário padrão para o horário de verão acontece.</span><span class="sxs-lookup"><span data-stu-id="b3b7b-130">Represents the time of day when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="b3b7b-131">year</span><span class="sxs-lookup"><span data-stu-id="b3b7b-131">year</span></span> | <span data-ttu-id="b3b7b-132">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="b3b7b-132">Edm.Int32</span></span> | <span data-ttu-id="b3b7b-133">Representa com que frequência, em anos, a transição do horário padrão para o horário de verão acontece.</span><span class="sxs-lookup"><span data-stu-id="b3b7b-133">Represents how frequently in terms of years the change from standard time to daylight saving time occurs.</span></span> <span data-ttu-id="b3b7b-134">Por exemplo, um valor 0 significa todos os anos.</span><span class="sxs-lookup"><span data-stu-id="b3b7b-134">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b3b7b-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b3b7b-135">JSON representation</span></span>

<span data-ttu-id="b3b7b-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b3b7b-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.standardTimeZoneOffset",
  "@odata.type": "microsoft.graph.daylightTimeZoneOffset"
}-->

```json
{
  "daylightBias": "Int32",
  "dayOccurrence": "Int32",
  "dayOfWeek": "string",
  "month": "Int32",
  "time": "TimeOfDay",
  "year": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "daylightTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->