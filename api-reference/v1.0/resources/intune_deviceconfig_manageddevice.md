# <a name="manageddevice-resource-type"></a><span data-ttu-id="48e5f-101">Tipo de recurso managedDevice</span><span class="sxs-lookup"><span data-stu-id="48e5f-101">managedDevice resource type</span></span>

> <span data-ttu-id="48e5f-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="48e5f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="48e5f-103">Dispositivos gerenciados ou pré-registrados pelo Intune</span><span class="sxs-lookup"><span data-stu-id="48e5f-103">Devices that are managed or pre-enrolled through Intune</span></span>
## <a name="methods"></a><span data-ttu-id="48e5f-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="48e5f-104">Methods</span></span>
|<span data-ttu-id="48e5f-105">Método</span><span class="sxs-lookup"><span data-stu-id="48e5f-105">Method</span></span>|<span data-ttu-id="48e5f-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="48e5f-106">Return Type</span></span>|<span data-ttu-id="48e5f-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="48e5f-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="48e5f-108">Listar managedDevices</span><span class="sxs-lookup"><span data-stu-id="48e5f-108">List managedDevices</span></span>](../api/intune_deviceconfig_manageddevice_list.md)|<span data-ttu-id="48e5f-109">Conjunto [managedDevice](../resources/intune_deviceconfig_manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="48e5f-109">[managedDevice](../resources/intune_deviceconfig_manageddevice.md) collection</span></span>|<span data-ttu-id="48e5f-110">Listar propriedades e relações de objetos de [managedDevice](../resources/intune_deviceconfig_manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="48e5f-110">List properties and relationships of the [managedDevice](../resources/intune_deviceconfig_manageddevice.md) objects.</span></span>|
|[<span data-ttu-id="48e5f-111">Obter managedDevice</span><span class="sxs-lookup"><span data-stu-id="48e5f-111">Get managedDevice</span></span>](../api/intune_deviceconfig_manageddevice_get.md)|[<span data-ttu-id="48e5f-112">managedDevice</span><span class="sxs-lookup"><span data-stu-id="48e5f-112">managedDevice</span></span>](../resources/intune_deviceconfig_manageddevice.md)|<span data-ttu-id="48e5f-113">Ler propriedades e relações de objetos de [managedDevice](../resources/intune_deviceconfig_manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="48e5f-113">Read properties and relationships of [plannerPlanDetails](../resources/intune_deviceconfig_manageddevice.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="48e5f-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48e5f-114">Properties</span></span>
|<span data-ttu-id="48e5f-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48e5f-115">Property</span></span>|<span data-ttu-id="48e5f-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="48e5f-116">Type</span></span>|<span data-ttu-id="48e5f-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="48e5f-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48e5f-118">id</span><span class="sxs-lookup"><span data-stu-id="48e5f-118">id</span></span>|<span data-ttu-id="48e5f-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="48e5f-119">String</span></span>|<span data-ttu-id="48e5f-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="48e5f-120">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="48e5f-121">Relações</span><span class="sxs-lookup"><span data-stu-id="48e5f-121">Relationships</span></span>
|<span data-ttu-id="48e5f-122">Relação</span><span class="sxs-lookup"><span data-stu-id="48e5f-122">Relationship</span></span>|<span data-ttu-id="48e5f-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="48e5f-123">Type</span></span>|<span data-ttu-id="48e5f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="48e5f-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48e5f-125">deviceConfigurationStates</span><span class="sxs-lookup"><span data-stu-id="48e5f-125">deviceConfigurationStates</span></span>|<span data-ttu-id="48e5f-126">Conjunto [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)</span><span class="sxs-lookup"><span data-stu-id="48e5f-126">[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) collection</span></span>|<span data-ttu-id="48e5f-127">Estados de configuração deste dispositivo.</span><span class="sxs-lookup"><span data-stu-id="48e5f-127">Device configuration states for this device.</span></span>|
|<span data-ttu-id="48e5f-128">deviceCompliancePolicyStates</span><span class="sxs-lookup"><span data-stu-id="48e5f-128">deviceCompliancePolicyStates</span></span>|<span data-ttu-id="48e5f-129">Conjunto [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md)</span><span class="sxs-lookup"><span data-stu-id="48e5f-129">[deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md) collection</span></span>|<span data-ttu-id="48e5f-130">Estados de política de conformidade deste dispositivo.</span><span class="sxs-lookup"><span data-stu-id="48e5f-130">Device compliance policy states for this device.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="48e5f-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48e5f-131">JSON Representation</span></span>
<span data-ttu-id="48e5f-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="48e5f-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "String (identifier)"
}
```



