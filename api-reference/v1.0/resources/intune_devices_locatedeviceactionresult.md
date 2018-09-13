# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="74dd1-101">Tipo de recurso locateDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="74dd1-101">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="74dd1-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="74dd1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74dd1-103">Resultado da ação de localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="74dd1-103">Locate device action result</span></span>

<span data-ttu-id="74dd1-104">Herda de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="74dd1-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="74dd1-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74dd1-105">Properties</span></span>
|<span data-ttu-id="74dd1-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74dd1-106">Property</span></span>|<span data-ttu-id="74dd1-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="74dd1-107">Type</span></span>|<span data-ttu-id="74dd1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="74dd1-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74dd1-109">actionName</span><span class="sxs-lookup"><span data-stu-id="74dd1-109">actionName</span></span>|<span data-ttu-id="74dd1-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74dd1-110">String</span></span>|<span data-ttu-id="74dd1-111">Nome da ação herdada de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="74dd1-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="74dd1-112">actionState</span><span class="sxs-lookup"><span data-stu-id="74dd1-112">actionState</span></span>|[<span data-ttu-id="74dd1-113">actionState</span><span class="sxs-lookup"><span data-stu-id="74dd1-113">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="74dd1-p101">Estado da ação herdado de [deviceActionResult](../resources/intune_devices_deviceactionresult.md). Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="74dd1-p101">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="74dd1-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="74dd1-116">startDateTime</span></span>|<span data-ttu-id="74dd1-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74dd1-117">DateTimeOffset</span></span>|<span data-ttu-id="74dd1-118">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="74dd1-118">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="74dd1-119">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="74dd1-119">lastUpdatedDateTime</span></span>|<span data-ttu-id="74dd1-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74dd1-120">DateTimeOffset</span></span>|<span data-ttu-id="74dd1-121">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="74dd1-121">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="74dd1-122">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="74dd1-122">deviceLocation</span></span>|[<span data-ttu-id="74dd1-123">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="74dd1-123">deviceGeoLocation</span></span>](../resources/intune_devices_devicegeolocation.md)|<span data-ttu-id="74dd1-124">local do dispositivo</span><span class="sxs-lookup"><span data-stu-id="74dd1-124">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="74dd1-125">Relações</span><span class="sxs-lookup"><span data-stu-id="74dd1-125">Relationships</span></span>
<span data-ttu-id="74dd1-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="74dd1-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="74dd1-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74dd1-127">JSON Representation</span></span>
<span data-ttu-id="74dd1-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="74dd1-128">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.locateDeviceActionResult"
}-->
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








