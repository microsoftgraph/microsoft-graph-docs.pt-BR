# <a name="softwareupdatestatussummary-resource-type"></a><span data-ttu-id="296a4-101">Tipo de recurso softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="296a4-101">softwareUpdateStatusSummary resource type</span></span>

> <span data-ttu-id="296a4-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="296a4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="296a4-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="296a4-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="296a4-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="296a4-104">Methods</span></span>
|<span data-ttu-id="296a4-105">Método</span><span class="sxs-lookup"><span data-stu-id="296a4-105">Method</span></span>|<span data-ttu-id="296a4-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="296a4-106">Return Type</span></span>|<span data-ttu-id="296a4-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="296a4-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="296a4-108">Obter softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="296a4-108">Get softwareUpdateStatusSummary</span></span>](../api/intune_deviceconfig_softwareupdatestatussummary_get.md)|[<span data-ttu-id="296a4-109">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="296a4-109">softwareUpdateStatusSummary</span></span>](../resources/intune_deviceconfig_softwareupdatestatussummary.md)|<span data-ttu-id="296a4-110">Ler propriedades e relações de objetos de [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="296a4-110">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>|
|[<span data-ttu-id="296a4-111">Atualizar softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="296a4-111">Update softwareUpdateStatusSummary</span></span>](../api/intune_deviceconfig_softwareupdatestatussummary_update.md)|[<span data-ttu-id="296a4-112">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="296a4-112">softwareUpdateStatusSummary</span></span>](../resources/intune_deviceconfig_softwareupdatestatussummary.md)|<span data-ttu-id="296a4-113">Atualizar as propriedades de um objeto de [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="296a4-113">Update the properties of a [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="296a4-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="296a4-114">Properties</span></span>
|<span data-ttu-id="296a4-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="296a4-115">Property</span></span>|<span data-ttu-id="296a4-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="296a4-116">Type</span></span>|<span data-ttu-id="296a4-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="296a4-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="296a4-118">id</span><span class="sxs-lookup"><span data-stu-id="296a4-118">id</span></span>|<span data-ttu-id="296a4-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="296a4-119">String</span></span>|<span data-ttu-id="296a4-120">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="296a4-120">Key of the entity.</span></span>|
|<span data-ttu-id="296a4-121">displayName</span><span class="sxs-lookup"><span data-stu-id="296a4-121">displayName</span></span>|<span data-ttu-id="296a4-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="296a4-122">String</span></span>|<span data-ttu-id="296a4-123">O nome da política.</span><span class="sxs-lookup"><span data-stu-id="296a4-123">The name of the policy.</span></span>|
|<span data-ttu-id="296a4-124">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="296a4-124">compliantDeviceCount</span></span>|<span data-ttu-id="296a4-125">Int32</span><span class="sxs-lookup"><span data-stu-id="296a4-125">Int32</span></span>|<span data-ttu-id="296a4-126">Número de dispositivos em conformidade.</span><span class="sxs-lookup"><span data-stu-id="296a4-126">Number of compliant devices.</span></span>|
|<span data-ttu-id="296a4-127">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="296a4-127">nonCompliantDeviceCount</span></span>|<span data-ttu-id="296a4-128">Int32</span><span class="sxs-lookup"><span data-stu-id="296a4-128">Int32</span></span>|<span data-ttu-id="296a4-129">Número de dispositivos sem conformidade.</span><span class="sxs-lookup"><span data-stu-id="296a4-129">Number of non compliant devices.</span></span>|
|<span data-ttu-id="296a4-130">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="296a4-130">remediatedDeviceCount</span></span>|<span data-ttu-id="296a4-131">Int32</span><span class="sxs-lookup"><span data-stu-id="296a4-131">Int32</span></span>|<span data-ttu-id="296a4-132">Número de dispositivos corrigidos.</span><span class="sxs-lookup"><span data-stu-id="296a4-132">Number of remediated devices.</span></span>|
|<span data-ttu-id="296a4-133">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="296a4-133">errorDeviceCount</span></span>|<span data-ttu-id="296a4-134">Int32</span><span class="sxs-lookup"><span data-stu-id="296a4-134">Int32</span></span>|<span data-ttu-id="296a4-135">Número de dispositivos com erro.</span><span class="sxs-lookup"><span data-stu-id="296a4-135">Number of devices had error.</span></span>|
|<span data-ttu-id="296a4-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="296a4-136">unknownDeviceCount</span></span>|<span data-ttu-id="296a4-137">Int32</span><span class="sxs-lookup"><span data-stu-id="296a4-137">Int32</span></span>|<span data-ttu-id="296a4-138">Número de dispositivos desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="296a4-138">Number of unknown devices.</span></span>|
|<span data-ttu-id="296a4-139">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="296a4-139">conflictDeviceCount</span></span>|<span data-ttu-id="296a4-140">Int32</span><span class="sxs-lookup"><span data-stu-id="296a4-140">Int32</span></span>|<span data-ttu-id="296a4-141">Número de dispositivos em conflito.</span><span class="sxs-lookup"><span data-stu-id="296a4-141">Number of conflict devices.</span></span>|
|<span data-ttu-id="296a4-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="296a4-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="296a4-143">Int32</span><span class="sxs-lookup"><span data-stu-id="296a4-143">Int32</span></span>|<span data-ttu-id="296a4-144">Número de dispositivos não aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="296a4-144">Number of not applicable devices.</span></span>|
|<span data-ttu-id="296a4-145">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="296a4-145">compliantUserCount</span></span>|<span data-ttu-id="296a4-146">Int32</span><span class="sxs-lookup"><span data-stu-id="296a4-146">Int32</span></span>|<span data-ttu-id="296a4-147">Número de usuários em conformidade.</span><span class="sxs-lookup"><span data-stu-id="296a4-147">Number of compliant users.</span></span>|
|<span data-ttu-id="296a4-148">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="296a4-148">nonCompliantUserCount</span></span>|<span data-ttu-id="296a4-149">Int32</span><span class="sxs-lookup"><span data-stu-id="296a4-149">Int32</span></span>|<span data-ttu-id="296a4-150">Número de usuários em não conformidade.</span><span class="sxs-lookup"><span data-stu-id="296a4-150">Number of non compliant users.</span></span>|
|<span data-ttu-id="296a4-151">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="296a4-151">remediatedUserCount</span></span>|<span data-ttu-id="296a4-152">Int32</span><span class="sxs-lookup"><span data-stu-id="296a4-152">Int32</span></span>|<span data-ttu-id="296a4-153">Número de usuários corrigidos.</span><span class="sxs-lookup"><span data-stu-id="296a4-153">Number of remediated users.</span></span>|
|<span data-ttu-id="296a4-154">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="296a4-154">errorUserCount</span></span>|<span data-ttu-id="296a4-155">Int32</span><span class="sxs-lookup"><span data-stu-id="296a4-155">Int32</span></span>|<span data-ttu-id="296a4-156">Número de usuários com erro.</span><span class="sxs-lookup"><span data-stu-id="296a4-156">Number of users had error.</span></span>|
|<span data-ttu-id="296a4-157">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="296a4-157">unknownUserCount</span></span>|<span data-ttu-id="296a4-158">Int32</span><span class="sxs-lookup"><span data-stu-id="296a4-158">Int32</span></span>|<span data-ttu-id="296a4-159">Número de usuários desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="296a4-159">Number of unknown users.</span></span>|
|<span data-ttu-id="296a4-160">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="296a4-160">conflictUserCount</span></span>|<span data-ttu-id="296a4-161">Int32</span><span class="sxs-lookup"><span data-stu-id="296a4-161">Int32</span></span>|<span data-ttu-id="296a4-162">Número de usuários com conflitos.</span><span class="sxs-lookup"><span data-stu-id="296a4-162">Number of conflict users.</span></span>|
|<span data-ttu-id="296a4-163">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="296a4-163">notApplicableUserCount</span></span>|<span data-ttu-id="296a4-164">Int32</span><span class="sxs-lookup"><span data-stu-id="296a4-164">Int32</span></span>|<span data-ttu-id="296a4-165">Número de usuários não aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="296a4-165">Number of not applicable users.</span></span>|

## <a name="relationships"></a><span data-ttu-id="296a4-166">Relações</span><span class="sxs-lookup"><span data-stu-id="296a4-166">Relationships</span></span>
<span data-ttu-id="296a4-167">Nenhum</span><span class="sxs-lookup"><span data-stu-id="296a4-167">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="296a4-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="296a4-168">JSON Representation</span></span>
<span data-ttu-id="296a4-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="296a4-169">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.softwareUpdateStatusSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "String (identifier)",
  "displayName": "String",
  "compliantDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "conflictDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantUserCount": 1024,
  "nonCompliantUserCount": 1024,
  "remediatedUserCount": 1024,
  "errorUserCount": 1024,
  "unknownUserCount": 1024,
  "conflictUserCount": 1024,
  "notApplicableUserCount": 1024
}
```








