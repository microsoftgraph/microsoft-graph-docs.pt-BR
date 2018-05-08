# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="c3023-101">Tipo de recurso outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="c3023-101">outlookGeoCoordinates resource type</span></span>

<span data-ttu-id="c3023-102">As coordenadas geográficas, a elevação e o grau de precisão delas para um local físico.</span><span class="sxs-lookup"><span data-stu-id="c3023-102">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3023-103">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c3023-103">JSON representation</span></span>

<span data-ttu-id="c3023-104">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c3023-104">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookGeoCoordinates"
}-->

```json
{
  "accuracy": 1024.13,
  "altitude": 1024.13,
  "altitudeAccuracy": 1024.13,
  "latitude": 1024.13,
  "longitude": 1024.13
}

```
## <a name="properties"></a><span data-ttu-id="c3023-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c3023-105">Properties</span></span>
| <span data-ttu-id="c3023-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3023-106">Property</span></span>     | <span data-ttu-id="c3023-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3023-107">Type</span></span>   |<span data-ttu-id="c3023-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3023-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3023-109">accuracy</span><span class="sxs-lookup"><span data-stu-id="c3023-109">accuracy</span></span>|<span data-ttu-id="c3023-110">double</span><span class="sxs-lookup"><span data-stu-id="c3023-110">double</span></span>|<span data-ttu-id="c3023-111">A precisão da latitude e da longitude.</span><span class="sxs-lookup"><span data-stu-id="c3023-111">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="c3023-112">Por exemplo, a precisão pode ser medida em metros, como a precisão da latitude e da longitude em um raio de 50 metros.</span><span class="sxs-lookup"><span data-stu-id="c3023-112">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="c3023-113">altitude</span><span class="sxs-lookup"><span data-stu-id="c3023-113">altitude</span></span>|<span data-ttu-id="c3023-114">double</span><span class="sxs-lookup"><span data-stu-id="c3023-114">double</span></span>|<span data-ttu-id="c3023-115">A altitude do local.</span><span class="sxs-lookup"><span data-stu-id="c3023-115">The altitude of the location.</span></span>|
|<span data-ttu-id="c3023-116">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="c3023-116">altitudeAccuracy</span></span>|<span data-ttu-id="c3023-117">double</span><span class="sxs-lookup"><span data-stu-id="c3023-117">double</span></span>|<span data-ttu-id="c3023-118">A precisão da altitude.</span><span class="sxs-lookup"><span data-stu-id="c3023-118">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="c3023-119">latitude</span><span class="sxs-lookup"><span data-stu-id="c3023-119">latitude</span></span>|<span data-ttu-id="c3023-120">double</span><span class="sxs-lookup"><span data-stu-id="c3023-120">double</span></span>|<span data-ttu-id="c3023-121">A latitude do local.</span><span class="sxs-lookup"><span data-stu-id="c3023-121">The latitude of the location.</span></span>|
|<span data-ttu-id="c3023-122">longitude</span><span class="sxs-lookup"><span data-stu-id="c3023-122">longitude</span></span>|<span data-ttu-id="c3023-123">double</span><span class="sxs-lookup"><span data-stu-id="c3023-123">double</span></span>|<span data-ttu-id="c3023-124">A longitude do local.</span><span class="sxs-lookup"><span data-stu-id="c3023-124">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->