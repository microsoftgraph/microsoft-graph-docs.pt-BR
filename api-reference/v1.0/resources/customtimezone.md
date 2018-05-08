# <a name="customtimezone-resource-type"></a><span data-ttu-id="bc2c8-101">Tipo de recurso customTimeZone</span><span class="sxs-lookup"><span data-stu-id="bc2c8-101">customTimeZone resource type</span></span>

<span data-ttu-id="bc2c8-102">Representa um fuso horário em que a transição do horário padrão para o horário de verão, ou vice-versa, não é padrão.</span><span class="sxs-lookup"><span data-stu-id="bc2c8-102">Represents a time zone where the transition from standard to daylight saving time, or vice versa is not standard.</span></span>


## <a name="properties"></a><span data-ttu-id="bc2c8-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bc2c8-103">Properties</span></span>
| <span data-ttu-id="bc2c8-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc2c8-104">Property</span></span>     | <span data-ttu-id="bc2c8-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc2c8-105">Type</span></span>   |<span data-ttu-id="bc2c8-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc2c8-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bc2c8-107">bias</span><span class="sxs-lookup"><span data-stu-id="bc2c8-107">Bias</span></span> | <span data-ttu-id="bc2c8-108">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="bc2c8-108">Edm.Int32</span></span> | <span data-ttu-id="bc2c8-109">A diferença de tempo em relação ao fuso horário UTC (Tempo Universal Coordenado).</span><span class="sxs-lookup"><span data-stu-id="bc2c8-109">The time offset of the time zone from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="bc2c8-110">Este valor está em minutos.</span><span class="sxs-lookup"><span data-stu-id="bc2c8-110">This value is in points.</span></span> <span data-ttu-id="bc2c8-111">Os fusos horários que estão adiantados em relação ao UTC têm uma diferença de tempo positiva, enquanto os atrasados têm uma diferença de tempo negativa.</span><span class="sxs-lookup"><span data-stu-id="bc2c8-111">Time zones that are ahead of UTC have a positive offset; time zones that are behind UTC have a negative offset.</span></span>|
| <span data-ttu-id="bc2c8-112">daylightOffset</span><span class="sxs-lookup"><span data-stu-id="bc2c8-112">daylightOffset</span></span> | [<span data-ttu-id="bc2c8-113">daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="bc2c8-113">daylightTimeZoneOffset</span></span>](daylighttimezoneoffset.md) | <span data-ttu-id="bc2c8-114">Especifica quando o fuso horário muda do horário padrão para o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="bc2c8-114">Specifies when the time zone switches from standard time to daylight saving time.</span></span> |
| <span data-ttu-id="bc2c8-115">name</span><span class="sxs-lookup"><span data-stu-id="bc2c8-115">name</span></span> | <span data-ttu-id="bc2c8-116">string</span><span class="sxs-lookup"><span data-stu-id="bc2c8-116">string</span></span> | <span data-ttu-id="bc2c8-117">O nome do fuso horário personalizado.</span><span class="sxs-lookup"><span data-stu-id="bc2c8-117">The name of the custom time zone.</span></span> |
| <span data-ttu-id="bc2c8-118">standardOffset</span><span class="sxs-lookup"><span data-stu-id="bc2c8-118">standardOffset</span></span> | [<span data-ttu-id="bc2c8-119">standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="bc2c8-119">standardTimeZoneOffset</span></span>](standardtimezoneoffset.md) | <span data-ttu-id="bc2c8-120">Especifica quando o fuso horário muda do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="bc2c8-120">Specifies when the time zone switches from daylight saving time to standard time.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="bc2c8-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bc2c8-121">JSON representation</span></span>

<span data-ttu-id="bc2c8-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bc2c8-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.customTimeZone"
}-->

```json
{
  "bias": "Int32",
  "daylightOffset": {"@odata.type": "microsoft.graph.daylightTimeZoneOffset"},
  "name": "string",
  "standardOffset": {"@odata.type": "microsoft.graph.standardTimeZoneOffset"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "customTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->