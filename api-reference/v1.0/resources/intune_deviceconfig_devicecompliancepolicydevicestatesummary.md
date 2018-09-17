# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="b399e-101">Tipo de recurso deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="b399e-101">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="b399e-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b399e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b399e-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b399e-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="b399e-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="b399e-104">Methods</span></span>
|<span data-ttu-id="b399e-105">Método</span><span class="sxs-lookup"><span data-stu-id="b399e-105">Method</span></span>|<span data-ttu-id="b399e-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b399e-106">Return Type</span></span>|<span data-ttu-id="b399e-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="b399e-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b399e-108">Obter deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="b399e-108">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune_deviceconfig_devicecompliancepolicydevicestatesummary_get.md)|[<span data-ttu-id="b399e-109">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="b399e-109">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="b399e-110">Ler propriedades e relações de objetos de [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="b399e-110">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="b399e-111">Atualizar deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="b399e-111">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune_deviceconfig_devicecompliancepolicydevicestatesummary_update.md)|[<span data-ttu-id="b399e-112">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="b399e-112">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="b399e-113">Atualizar as propriedades de um objeto de [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="b399e-113">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b399e-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b399e-114">Properties</span></span>
|<span data-ttu-id="b399e-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b399e-115">Property</span></span>|<span data-ttu-id="b399e-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="b399e-116">Type</span></span>|<span data-ttu-id="b399e-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="b399e-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b399e-118">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="b399e-118">inGracePeriodCount</span></span>|<span data-ttu-id="b399e-119">Int32</span><span class="sxs-lookup"><span data-stu-id="b399e-119">Int32</span></span>|<span data-ttu-id="b399e-120">Quantidade de dispositivos que estão no período de cortesia</span><span class="sxs-lookup"><span data-stu-id="b399e-120">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="b399e-121">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="b399e-121">configManagerCount</span></span>|<span data-ttu-id="b399e-122">Int32</span><span class="sxs-lookup"><span data-stu-id="b399e-122">Int32</span></span>|<span data-ttu-id="b399e-123">Quantidade de dispositivos que estão em conformidade gerenciada pelo System Center Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="b399e-123">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="b399e-124">id</span><span class="sxs-lookup"><span data-stu-id="b399e-124">id</span></span>|<span data-ttu-id="b399e-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b399e-125">String</span></span>|<span data-ttu-id="b399e-126">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b399e-126">Key of the entity.</span></span>|
|<span data-ttu-id="b399e-127">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b399e-127">unknownDeviceCount</span></span>|<span data-ttu-id="b399e-128">Int32</span><span class="sxs-lookup"><span data-stu-id="b399e-128">Int32</span></span>|<span data-ttu-id="b399e-129">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="b399e-129">Number of unknown devices</span></span>|
|<span data-ttu-id="b399e-130">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b399e-130">notApplicableDeviceCount</span></span>|<span data-ttu-id="b399e-131">Int32</span><span class="sxs-lookup"><span data-stu-id="b399e-131">Int32</span></span>|<span data-ttu-id="b399e-132">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="b399e-132">Number of not applicable devices</span></span>|
|<span data-ttu-id="b399e-133">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b399e-133">compliantDeviceCount</span></span>|<span data-ttu-id="b399e-134">Int32</span><span class="sxs-lookup"><span data-stu-id="b399e-134">Int32</span></span>|<span data-ttu-id="b399e-135">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="b399e-135">Number of compliant devices</span></span>|
|<span data-ttu-id="b399e-136">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b399e-136">remediatedDeviceCount</span></span>|<span data-ttu-id="b399e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b399e-137">Int32</span></span>|<span data-ttu-id="b399e-138">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="b399e-138">Number of remediated devices</span></span>|
|<span data-ttu-id="b399e-139">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b399e-139">nonCompliantDeviceCount</span></span>|<span data-ttu-id="b399e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b399e-140">Int32</span></span>|<span data-ttu-id="b399e-141">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="b399e-141">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="b399e-142">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b399e-142">errorDeviceCount</span></span>|<span data-ttu-id="b399e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b399e-143">Int32</span></span>|<span data-ttu-id="b399e-144">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="b399e-144">Number of error devices</span></span>|
|<span data-ttu-id="b399e-145">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b399e-145">conflictDeviceCount</span></span>|<span data-ttu-id="b399e-146">Int32</span><span class="sxs-lookup"><span data-stu-id="b399e-146">Int32</span></span>|<span data-ttu-id="b399e-147">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="b399e-147">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="b399e-148">Relações</span><span class="sxs-lookup"><span data-stu-id="b399e-148">Relationships</span></span>
<span data-ttu-id="b399e-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b399e-149">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b399e-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b399e-150">JSON Representation</span></span>
<span data-ttu-id="b399e-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b399e-151">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyDeviceStateSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 1024,
  "configManagerCount": 1024,
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```








