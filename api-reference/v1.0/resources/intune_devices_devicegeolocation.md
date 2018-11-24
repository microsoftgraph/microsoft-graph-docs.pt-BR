# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="f35ee-101">Tipo de recurso deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="f35ee-101">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="f35ee-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f35ee-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f35ee-103">Localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f35ee-103">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="f35ee-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f35ee-104">Properties</span></span>
|<span data-ttu-id="f35ee-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f35ee-105">Property</span></span>|<span data-ttu-id="f35ee-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="f35ee-106">Type</span></span>|<span data-ttu-id="f35ee-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="f35ee-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f35ee-108">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="f35ee-108">lastCollectedDateTime</span></span>|<span data-ttu-id="f35ee-109">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f35ee-109">DateTimeOffset</span></span>|<span data-ttu-id="f35ee-110">Hora em que a localização foi registrada, em relação ao UTC</span><span class="sxs-lookup"><span data-stu-id="f35ee-110">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="f35ee-111">longitude</span><span class="sxs-lookup"><span data-stu-id="f35ee-111">longitude</span></span>|<span data-ttu-id="f35ee-112">Double</span><span class="sxs-lookup"><span data-stu-id="f35ee-112">Double</span></span>|<span data-ttu-id="f35ee-113">Coordenada de longitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f35ee-113">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="f35ee-114">latitude</span><span class="sxs-lookup"><span data-stu-id="f35ee-114">latitude</span></span>|<span data-ttu-id="f35ee-115">Double</span><span class="sxs-lookup"><span data-stu-id="f35ee-115">Double</span></span>|<span data-ttu-id="f35ee-116">Coordenada de latitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f35ee-116">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="f35ee-117">altitude</span><span class="sxs-lookup"><span data-stu-id="f35ee-117">altitude</span></span>|<span data-ttu-id="f35ee-118">Double</span><span class="sxs-lookup"><span data-stu-id="f35ee-118">Double</span></span>|<span data-ttu-id="f35ee-119">Altitude, especificada em metros acima do nível do mar</span><span class="sxs-lookup"><span data-stu-id="f35ee-119">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="f35ee-120">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="f35ee-120">horizontalAccuracy</span></span>|<span data-ttu-id="f35ee-121">Double</span><span class="sxs-lookup"><span data-stu-id="f35ee-121">Double</span></span>|<span data-ttu-id="f35ee-122">Precisão da latitude e da longitude em metros</span><span class="sxs-lookup"><span data-stu-id="f35ee-122">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="f35ee-123">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="f35ee-123">verticalAccuracy</span></span>|<span data-ttu-id="f35ee-124">Double</span><span class="sxs-lookup"><span data-stu-id="f35ee-124">Double</span></span>|<span data-ttu-id="f35ee-125">Precisão da altitude em metros</span><span class="sxs-lookup"><span data-stu-id="f35ee-125">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="f35ee-126">heading</span><span class="sxs-lookup"><span data-stu-id="f35ee-126">heading</span></span>|<span data-ttu-id="f35ee-127">Double</span><span class="sxs-lookup"><span data-stu-id="f35ee-127">Double</span></span>|<span data-ttu-id="f35ee-128">Direção em graus do norte verdadeiro</span><span class="sxs-lookup"><span data-stu-id="f35ee-128">Heading in degrees from true north</span></span>|
|<span data-ttu-id="f35ee-129">speed</span><span class="sxs-lookup"><span data-stu-id="f35ee-129">speed</span></span>|<span data-ttu-id="f35ee-130">Double</span><span class="sxs-lookup"><span data-stu-id="f35ee-130">Double</span></span>|<span data-ttu-id="f35ee-131">Velocidade na qual o dispositivo está viajando, em metros por segundo</span><span class="sxs-lookup"><span data-stu-id="f35ee-131">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="f35ee-132">Relações</span><span class="sxs-lookup"><span data-stu-id="f35ee-132">Relationships</span></span>
<span data-ttu-id="f35ee-133">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="f35ee-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f35ee-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f35ee-134">JSON Representation</span></span>
<span data-ttu-id="f35ee-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f35ee-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
  "lastCollectedDateTime": "String (timestamp)",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "altitude": "<Unknown Primitive Type Edm.Double>",
  "horizontalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "verticalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "heading": "<Unknown Primitive Type Edm.Double>",
  "speed": "<Unknown Primitive Type Edm.Double>"
}
```



