# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="ebc31-101">Tipo de recurso managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ebc31-101">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="ebc31-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ebc31-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ebc31-103">Dados de resumo de dispositivos gerenciados</span><span class="sxs-lookup"><span data-stu-id="ebc31-103">Summary data for managed devices</span></span>
## <a name="methods"></a><span data-ttu-id="ebc31-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="ebc31-104">Methods</span></span>
|<span data-ttu-id="ebc31-105">Método</span><span class="sxs-lookup"><span data-stu-id="ebc31-105">Method</span></span>|<span data-ttu-id="ebc31-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ebc31-106">Return Type</span></span>|<span data-ttu-id="ebc31-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebc31-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ebc31-108">Obter managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ebc31-108">Get managedDeviceOverview</span></span>](../api/intune_devices_manageddeviceoverview_get.md)|[<span data-ttu-id="ebc31-109">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ebc31-109">managedDeviceOverview</span></span>](../resources/intune_devices_manageddeviceoverview.md)|<span data-ttu-id="ebc31-110">Ler propriedades e relações de objetos de [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="ebc31-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_devices_manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="ebc31-111">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ebc31-111">Update managedDeviceOverview</span></span>](../api/intune_devices_manageddeviceoverview_update.md)|[<span data-ttu-id="ebc31-112">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ebc31-112">managedDeviceOverview</span></span>](../resources/intune_devices_manageddeviceoverview.md)|<span data-ttu-id="ebc31-113">Atualizar as propriedades de um objeto de [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="ebc31-113">Update the properties of a [calendar](../resources/intune_devices_manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ebc31-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ebc31-114">Properties</span></span>
|<span data-ttu-id="ebc31-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ebc31-115">Property</span></span>|<span data-ttu-id="ebc31-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebc31-116">Type</span></span>|<span data-ttu-id="ebc31-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebc31-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebc31-118">id</span><span class="sxs-lookup"><span data-stu-id="ebc31-118">id</span></span>|<span data-ttu-id="ebc31-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ebc31-119">String</span></span>|<span data-ttu-id="ebc31-120">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="ebc31-120">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="ebc31-121">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ebc31-121">enrolledDeviceCount</span></span>|<span data-ttu-id="ebc31-122">Int32</span><span class="sxs-lookup"><span data-stu-id="ebc31-122">Int32</span></span>|<span data-ttu-id="ebc31-123">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="ebc31-123">Total enrolled device count.</span></span> <span data-ttu-id="ebc31-124">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="ebc31-124">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="ebc31-125">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="ebc31-125">mdmEnrolledCount</span></span>|<span data-ttu-id="ebc31-126">Int32</span><span class="sxs-lookup"><span data-stu-id="ebc31-126">Int32</span></span>|<span data-ttu-id="ebc31-127">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="ebc31-127">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="ebc31-128">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ebc31-128">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="ebc31-129">Int32</span><span class="sxs-lookup"><span data-stu-id="ebc31-129">Int32</span></span>|<span data-ttu-id="ebc31-130">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="ebc31-130">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="ebc31-131">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="ebc31-131">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="ebc31-132">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="ebc31-132">deviceOperatingSystemSummary</span></span>](../resources/intune_devices_deviceoperatingsystemsummary.md)|<span data-ttu-id="ebc31-133">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ebc31-133">Device operating system summary.</span></span>|
|<span data-ttu-id="ebc31-134">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="ebc31-134">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="ebc31-135">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="ebc31-135">deviceExchangeAccessStateSummary</span></span>](../resources/intune_devices_deviceexchangeaccessstatesummary.md)|<span data-ttu-id="ebc31-136">Distribuição do estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="ebc31-136">Distribution of Exchange Access State in Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebc31-137">Relações</span><span class="sxs-lookup"><span data-stu-id="ebc31-137">Relationships</span></span>
<span data-ttu-id="ebc31-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ebc31-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ebc31-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ebc31-139">JSON Representation</span></span>
<span data-ttu-id="ebc31-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ebc31-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "id": "String (identifier)",
  "enrolledDeviceCount": 1024,
  "mdmEnrolledCount": 1024,
  "dualEnrolledDeviceCount": 1024,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 1024,
    "iosCount": 1024,
    "macOSCount": 1024,
    "windowsMobileCount": 1024,
    "windowsCount": 1024,
    "unknownCount": 1024
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 1024,
    "blockedDeviceCount": 1024,
    "quarantinedDeviceCount": 1024,
    "unknownDeviceCount": 1024,
    "unavailableDeviceCount": 1024
  }
}
```



