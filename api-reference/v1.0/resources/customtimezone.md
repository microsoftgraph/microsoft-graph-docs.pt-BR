# <a name="customtimezone-resource-type"></a><span data-ttu-id="3a8fe-101">Tipo de recurso customTimeZone</span><span class="sxs-lookup"><span data-stu-id="3a8fe-101">customTimeZone resource type</span></span>

<span data-ttu-id="3a8fe-102">Representa um fuso horário em que a transição do horário padrão para o horário de verão, ou vice-versa, não é padrão.</span><span class="sxs-lookup"><span data-stu-id="3a8fe-102">Represents a time zone where the transition from standard to daylight saving time, or vice versa is not standard.</span></span>


## <a name="properties"></a><span data-ttu-id="3a8fe-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a8fe-103">Properties</span></span>
| <span data-ttu-id="3a8fe-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a8fe-104">Property</span></span>     | <span data-ttu-id="3a8fe-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a8fe-105">Type</span></span>   |<span data-ttu-id="3a8fe-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a8fe-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3a8fe-107">bias</span><span class="sxs-lookup"><span data-stu-id="3a8fe-107">bias</span></span> | <span data-ttu-id="3a8fe-108">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="3a8fe-108">Edm.Int32</span></span> | <span data-ttu-id="3a8fe-109">A diferença de tempo em relação ao fuso horário UTC (Tempo Universal Coordenado).</span><span class="sxs-lookup"><span data-stu-id="3a8fe-109">The time offset of the time zone from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="3a8fe-110">Este valor está em minutos.</span><span class="sxs-lookup"><span data-stu-id="3a8fe-110">This value is in minutes.</span></span> <span data-ttu-id="3a8fe-111">Os fusos horários que estão adiantados em relação ao UTC têm uma diferença de tempo positiva, enquanto os atrasados têm uma diferença de tempo negativa.</span><span class="sxs-lookup"><span data-stu-id="3a8fe-111">Time zones that are ahead of UTC have a positive offset; time zones that are behind UTC have a negative offset.</span></span>|
| <span data-ttu-id="3a8fe-112">daylightOffset</span><span class="sxs-lookup"><span data-stu-id="3a8fe-112">daylightOffset</span></span> | [<span data-ttu-id="3a8fe-113">daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="3a8fe-113">daylightTimeZoneOffset</span></span>](daylighttimezoneoffset.md) | <span data-ttu-id="3a8fe-114">Especifica quando o fuso horário muda do horário padrão para o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="3a8fe-114">Specifies when the time zone switches from standard time to daylight saving time.</span></span> |
| <span data-ttu-id="3a8fe-115">name</span><span class="sxs-lookup"><span data-stu-id="3a8fe-115">name</span></span> | <span data-ttu-id="3a8fe-116">string</span><span class="sxs-lookup"><span data-stu-id="3a8fe-116">string</span></span> | <span data-ttu-id="3a8fe-117">O nome do fuso horário personalizado.</span><span class="sxs-lookup"><span data-stu-id="3a8fe-117">The name of the custom time zone.</span></span> |
| <span data-ttu-id="3a8fe-118">standardOffset</span><span class="sxs-lookup"><span data-stu-id="3a8fe-118">standardOffset</span></span> | [<span data-ttu-id="3a8fe-119">standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="3a8fe-119">standardTimeZoneOffset</span></span>](standardtimezoneoffset.md) | <span data-ttu-id="3a8fe-120">Especifica quando o fuso horário muda do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="3a8fe-120">Specifies when the time zone switches from daylight saving time to standard time.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="3a8fe-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a8fe-121">JSON representation</span></span>

<span data-ttu-id="3a8fe-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3a8fe-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.timeZoneBase",
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