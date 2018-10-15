# <a name="timeconstraint-resource-type"></a><span data-ttu-id="b2998-101">Tipo de recurso timeConstraint</span><span class="sxs-lookup"><span data-stu-id="b2998-101">timeConstraint resource type</span></span>

<span data-ttu-id="b2998-102">Restringe as sugestões de horário para reuniões a certas horas e dias da semana de acordo com a natureza especificada da atividade e intervalos de tempo disponíveis.</span><span class="sxs-lookup"><span data-stu-id="b2998-102">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2998-103">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b2998-103">JSON representation</span></span>

<span data-ttu-id="b2998-104">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b2998-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeConstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a><span data-ttu-id="b2998-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b2998-105">Properties</span></span>
| <span data-ttu-id="b2998-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2998-106">Property</span></span>     | <span data-ttu-id="b2998-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2998-107">Type</span></span>   |<span data-ttu-id="b2998-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2998-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2998-109">activityDomain</span><span class="sxs-lookup"><span data-stu-id="b2998-109">activityDomain</span></span>|<span data-ttu-id="b2998-110">activityDomain</span><span class="sxs-lookup"><span data-stu-id="b2998-110">activityDomain</span></span>|<span data-ttu-id="b2998-111">A natureza da atividade, opcional.</span><span class="sxs-lookup"><span data-stu-id="b2998-111">The nature of the activity, optional. Possible values are: , , , or .</span></span> <span data-ttu-id="b2998-112">Os valores possíveis são `work`, `personal`, `unrestricted` ou `unknown`.</span><span class="sxs-lookup"><span data-stu-id="b2998-112">The possible values are `work`, `personal`, `unrestricted`, , , , , , , , , or `unknown`.</span></span>|
|<span data-ttu-id="b2998-113">timeslots</span><span class="sxs-lookup"><span data-stu-id="b2998-113">timeslots</span></span>|<span data-ttu-id="b2998-114">Coleção [timeSlot](timeslot.md)</span><span class="sxs-lookup"><span data-stu-id="b2998-114">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="b2998-115">Uma matriz de períodos de tempo.</span><span class="sxs-lookup"><span data-stu-id="b2998-115">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
