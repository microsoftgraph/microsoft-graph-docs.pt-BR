# <a name="devicemanagement-resource-type"></a><span data-ttu-id="7e645-101">Tipo de recurso deviceManagement</span><span class="sxs-lookup"><span data-stu-id="7e645-101">deviceManagement resource type</span></span>

> <span data-ttu-id="7e645-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7e645-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e645-103">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="7e645-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="7e645-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="7e645-104">Methods</span></span>
|<span data-ttu-id="7e645-105">Método</span><span class="sxs-lookup"><span data-stu-id="7e645-105">Method</span></span>|<span data-ttu-id="7e645-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7e645-106">Return Type</span></span>|<span data-ttu-id="7e645-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e645-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7e645-108">Obter deviceManagement</span><span class="sxs-lookup"><span data-stu-id="7e645-108">Get deviceManagement</span></span>](../api/intune_devices_devicemanagement_get.md)|[<span data-ttu-id="7e645-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="7e645-109">deviceManagement</span></span>](../resources/intune_devices_devicemanagement.md)|<span data-ttu-id="7e645-110">Ler propriedades e relações de objetos de [deviceManagement](../resources/intune_devices_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="7e645-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_devices_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="7e645-111">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="7e645-111">Update deviceManagement</span></span>](../api/intune_devices_devicemanagement_update.md)|[<span data-ttu-id="7e645-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="7e645-112">deviceManagement</span></span>](../resources/intune_devices_devicemanagement.md)|<span data-ttu-id="7e645-113">Atualizar as propriedades de um objeto de [deviceManagement](../resources/intune_devices_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="7e645-113">Update the properties of a [calendar](../resources/intune_devices_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7e645-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7e645-114">Properties</span></span>
|<span data-ttu-id="7e645-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7e645-115">Property</span></span>|<span data-ttu-id="7e645-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e645-116">Type</span></span>|<span data-ttu-id="7e645-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e645-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e645-118">id</span><span class="sxs-lookup"><span data-stu-id="7e645-118">id</span></span>|<span data-ttu-id="7e645-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e645-119">String</span></span>|<span data-ttu-id="7e645-120">O identificador exclusivo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7e645-120">Unique Identifier for the device</span></span>|
|<span data-ttu-id="7e645-121">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="7e645-121">subscriptionState</span></span>|<span data-ttu-id="7e645-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e645-122">String</span></span>|<span data-ttu-id="7e645-123">Estado de assinatura de gerenciamento de dispositivo móvel do locatário.</span><span class="sxs-lookup"><span data-stu-id="7e645-123">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="7e645-124">Os valores possíveis são: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="7e645-124">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e645-125">Relações</span><span class="sxs-lookup"><span data-stu-id="7e645-125">Relationships</span></span>
|<span data-ttu-id="7e645-126">Relação</span><span class="sxs-lookup"><span data-stu-id="7e645-126">Relationship</span></span>|<span data-ttu-id="7e645-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e645-127">Type</span></span>|<span data-ttu-id="7e645-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e645-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e645-129">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="7e645-129">applePushNotificationCertificate</span></span>|[<span data-ttu-id="7e645-130">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="7e645-130">applePushNotificationCertificate</span></span>](../resources/intune_devices_applepushnotificationcertificate.md)|<span data-ttu-id="7e645-131">Certificado de notificação por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="7e645-131">Apple push notification certificate.</span></span>|
|<span data-ttu-id="7e645-132">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7e645-132">managedDeviceOverview</span></span>|[<span data-ttu-id="7e645-133">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7e645-133">managedDeviceOverview</span></span>](../resources/intune_devices_manageddeviceoverview.md)|<span data-ttu-id="7e645-134">Visão geral do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7e645-134">Device overview</span></span>|
|<span data-ttu-id="7e645-135">detectedApps</span><span class="sxs-lookup"><span data-stu-id="7e645-135">detectedApps</span></span>|<span data-ttu-id="7e645-136">Conjunto [detectedApp](../resources/intune_devices_detectedapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e645-136">[detectedApp](../resources/intune_devices_detectedapp.md) collection</span></span>|<span data-ttu-id="7e645-137">A lista de aplicativos detectados associados a um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7e645-137">The list of detected apps associated with a device.</span></span>|
|<span data-ttu-id="7e645-138">managedDevices</span><span class="sxs-lookup"><span data-stu-id="7e645-138">managedDevices</span></span>|<span data-ttu-id="7e645-139">Conjunto [managedDevice](../resources/intune_devices_manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="7e645-139">[managedDevice](../resources/intune_devices_manageddevice.md) collection</span></span>|<span data-ttu-id="7e645-140">A lista de dispositivos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="7e645-140">The list of managed devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7e645-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7e645-141">JSON Representation</span></span>
<span data-ttu-id="7e645-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7e645-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "subscriptionState": "String"
}
```



