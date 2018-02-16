# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="4a8da-101">Tipo de recurso locateDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="4a8da-101">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="4a8da-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4a8da-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a8da-103">Resultado da ação de localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="4a8da-103">Locate device action result</span></span>

<span data-ttu-id="4a8da-104">Herda de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4a8da-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4a8da-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a8da-105">Properties</span></span>
|<span data-ttu-id="4a8da-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a8da-106">Property</span></span>|<span data-ttu-id="4a8da-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a8da-107">Type</span></span>|<span data-ttu-id="4a8da-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a8da-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a8da-109">actionName</span><span class="sxs-lookup"><span data-stu-id="4a8da-109">actionName</span></span>|<span data-ttu-id="4a8da-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a8da-110">String</span></span>|<span data-ttu-id="4a8da-111">Nome da ação Herdado de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4a8da-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="4a8da-112">actionState</span><span class="sxs-lookup"><span data-stu-id="4a8da-112">actionState</span></span>|<span data-ttu-id="4a8da-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a8da-113">String</span></span>|<span data-ttu-id="4a8da-114">Estado da ação Herdado de [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="4a8da-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="4a8da-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4a8da-115">startDateTime</span></span>|<span data-ttu-id="4a8da-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a8da-116">DateTimeOffset</span></span>|<span data-ttu-id="4a8da-117">Hora de início da ação Herdada de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4a8da-117">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="4a8da-118">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a8da-118">lastUpdatedDateTime</span></span>|<span data-ttu-id="4a8da-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a8da-119">DateTimeOffset</span></span>|<span data-ttu-id="4a8da-120">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4a8da-120">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="4a8da-121">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="4a8da-121">deviceLocation</span></span>|[<span data-ttu-id="4a8da-122">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="4a8da-122">deviceGeoLocation</span></span>](../resources/intune_devices_devicegeolocation.md)|<span data-ttu-id="4a8da-123">local do dispositivo</span><span class="sxs-lookup"><span data-stu-id="4a8da-123">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a8da-124">Relações</span><span class="sxs-lookup"><span data-stu-id="4a8da-124">Relationships</span></span>
<span data-ttu-id="4a8da-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4a8da-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4a8da-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a8da-126">JSON Representation</span></span>
<span data-ttu-id="4a8da-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4a8da-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.locateDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.locateDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "deviceLocation": {
    "@odata.type": "microsoft.graph.deviceGeoLocation",
    "lastCollectedDateTime": "String (timestamp)",
    "longitude": "<Unknown Primitive Type Edm.Double>",
    "latitude": "<Unknown Primitive Type Edm.Double>",
    "altitude": "<Unknown Primitive Type Edm.Double>",
    "horizontalAccuracy": "<Unknown Primitive Type Edm.Double>",
    "verticalAccuracy": "<Unknown Primitive Type Edm.Double>",
    "heading": "<Unknown Primitive Type Edm.Double>",
    "speed": "<Unknown Primitive Type Edm.Double>"
  }
}
```



