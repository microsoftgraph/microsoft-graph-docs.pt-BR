# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="842c6-101">Tipo de recurso windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="842c6-101">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="842c6-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="842c6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="842c6-103">Resultado da última verificação do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="842c6-103">Windows Defender last scan result</span></span>

<span data-ttu-id="842c6-104">Herda de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="842c6-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="842c6-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="842c6-105">Properties</span></span>
|<span data-ttu-id="842c6-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="842c6-106">Property</span></span>|<span data-ttu-id="842c6-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="842c6-107">Type</span></span>|<span data-ttu-id="842c6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="842c6-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="842c6-109">actionName</span><span class="sxs-lookup"><span data-stu-id="842c6-109">actionName</span></span>|<span data-ttu-id="842c6-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="842c6-110">String</span></span>|<span data-ttu-id="842c6-111">Nome da ação Herdado de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="842c6-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="842c6-112">actionState</span><span class="sxs-lookup"><span data-stu-id="842c6-112">actionState</span></span>|<span data-ttu-id="842c6-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="842c6-113">String</span></span>|<span data-ttu-id="842c6-114">Estado da ação Herdado de [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="842c6-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="842c6-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="842c6-115">startDateTime</span></span>|<span data-ttu-id="842c6-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="842c6-116">DateTimeOffset</span></span>|<span data-ttu-id="842c6-117">Hora de início da ação Herdada de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="842c6-117">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="842c6-118">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="842c6-118">lastUpdatedDateTime</span></span>|<span data-ttu-id="842c6-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="842c6-119">DateTimeOffset</span></span>|<span data-ttu-id="842c6-120">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="842c6-120">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="842c6-121">scanType</span><span class="sxs-lookup"><span data-stu-id="842c6-121">scanType</span></span>|<span data-ttu-id="842c6-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="842c6-122">String</span></span>|<span data-ttu-id="842c6-123">Tipo de verificação, seja verificação completa ou verificação rápida</span><span class="sxs-lookup"><span data-stu-id="842c6-123">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="842c6-124">Relações</span><span class="sxs-lookup"><span data-stu-id="842c6-124">Relationships</span></span>
<span data-ttu-id="842c6-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="842c6-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="842c6-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="842c6-126">JSON Representation</span></span>
<span data-ttu-id="842c6-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="842c6-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDefenderScanActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderScanActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "scanType": "String"
}
```



