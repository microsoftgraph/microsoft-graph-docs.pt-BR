# <a name="standardtimezoneoffset-resource-type"></a><span data-ttu-id="c7d6b-101">Tipo de recurso standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="c7d6b-101">standardTimeZoneOffset resource type</span></span>

<span data-ttu-id="c7d6b-102">Especifica quando um fuso horário muda do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="c7d6b-102">Specifies when a time zone switches from daylight saving time to standard time.</span></span>

<span data-ttu-id="c7d6b-103">Por exemplo, se um fuso horário estiver especificado com as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="c7d6b-103">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="c7d6b-104">**dayOccurrence** como 3</span><span class="sxs-lookup"><span data-stu-id="c7d6b-104">**dayOccurrence** is 3</span></span>
- <span data-ttu-id="c7d6b-105">**dayOfWeek** como "Domingo"</span><span class="sxs-lookup"><span data-stu-id="c7d6b-105">**dayOfWeek** is "Sunday"</span></span>
- <span data-ttu-id="c7d6b-106">**month** como 10</span><span class="sxs-lookup"><span data-stu-id="c7d6b-106">**month** is 10</span></span>
- <span data-ttu-id="c7d6b-107">**time** como 02:00:00 _ **year** como 0. Isso significa que a transição do fuso horário do horário de verão para o horário padrão ocorre às 02:00:00 da manhã no quarto domingo de maio, todos os anos.</span><span class="sxs-lookup"><span data-stu-id="c7d6b-107">**time** is 02:00:00 _ **year** is 0 That means the transition from daylight saving time to standard occurs at 2 AM on the third Sunday of October, every year.</span></span>

## <a name="properties"></a><span data-ttu-id="c7d6b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c7d6b-108">Properties</span></span>
| <span data-ttu-id="c7d6b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7d6b-109">Property</span></span>     | <span data-ttu-id="c7d6b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7d6b-110">Type</span></span>   |<span data-ttu-id="c7d6b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7d6b-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c7d6b-112">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="c7d6b-112">dayOccurrence</span></span> | <span data-ttu-id="c7d6b-113">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="c7d6b-113">Edm.Int32</span></span> | <span data-ttu-id="c7d6b-114">Representa a enésima ocorrência do dia da semana em que ocorre a transição do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="c7d6b-114">Represents the nth occurrence of the day of week that the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="c7d6b-115">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="c7d6b-115">DAYOFWEEK</span></span> | <span data-ttu-id="c7d6b-116">string</span><span class="sxs-lookup"><span data-stu-id="c7d6b-116">string</span></span> | <span data-ttu-id="c7d6b-117">Representa o dia da semana em que ocorre a transição do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="c7d6b-117">Represents the day of the week when the transition from daylight saving time to standard time.</span></span> |
| <span data-ttu-id="c7d6b-118">month</span><span class="sxs-lookup"><span data-stu-id="c7d6b-118">month</span></span> | <span data-ttu-id="c7d6b-119">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="c7d6b-119">Edm.Int32</span></span> | <span data-ttu-id="c7d6b-120">Representa o mês do ano em que ocorre a transição do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="c7d6b-120">Represents the month of the year when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="c7d6b-121">time</span><span class="sxs-lookup"><span data-stu-id="c7d6b-121">time</span></span> | <span data-ttu-id="c7d6b-122">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c7d6b-122">Edm.TimeOfDay</span></span> | <span data-ttu-id="c7d6b-123">Representa a hora do dia em que ocorre a transição do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="c7d6b-123">Represents the time of day when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="c7d6b-124">year</span><span class="sxs-lookup"><span data-stu-id="c7d6b-124">year</span></span> | <span data-ttu-id="c7d6b-125">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="c7d6b-125">Edm.Int32</span></span> | <span data-ttu-id="c7d6b-126">Representa com que frequência, em anos, ocorre a mudança do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="c7d6b-126">Represents how frequently in terms of years the change from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="c7d6b-127">Por exemplo, um valor 0 significa todos os anos.</span><span class="sxs-lookup"><span data-stu-id="c7d6b-127">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c7d6b-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c7d6b-128">JSON representation</span></span>

<span data-ttu-id="c7d6b-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c7d6b-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.standardTimeZoneOffset"
}-->

```json
{
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
  "description": "standardTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->