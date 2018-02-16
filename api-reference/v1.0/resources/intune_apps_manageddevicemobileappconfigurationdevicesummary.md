# <a name="manageddevicemobileappconfigurationdevicesummary-resource-type"></a><span data-ttu-id="f8e2c-101">Tipo de recurso managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="f8e2c-101">managedDeviceMobileAppConfigurationDeviceSummary resource type</span></span>

> <span data-ttu-id="f8e2c-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f8e2c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8e2c-103">Contém propriedades, propriedades herdadas e ações para um resumo de status do dispositivo de configuração de aplicativo móvel de MDM.</span><span class="sxs-lookup"><span data-stu-id="f8e2c-103">Contains properties, inherited properties and actions for an MDM mobile app configuration device status summary.</span></span>
## <a name="methods"></a><span data-ttu-id="f8e2c-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="f8e2c-104">Methods</span></span>
|<span data-ttu-id="f8e2c-105">Método</span><span class="sxs-lookup"><span data-stu-id="f8e2c-105">Method</span></span>|<span data-ttu-id="f8e2c-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f8e2c-106">Return Type</span></span>|<span data-ttu-id="f8e2c-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8e2c-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f8e2c-108">Obter managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="f8e2c-108">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationdevicesummary_get.md)|[<span data-ttu-id="f8e2c-109">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="f8e2c-109">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="f8e2c-110">Ler propriedades e relações de objetos de [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="f8e2c-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|
|[<span data-ttu-id="f8e2c-111">Atualizar managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="f8e2c-111">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationdevicesummary_update.md)|[<span data-ttu-id="f8e2c-112">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="f8e2c-112">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="f8e2c-113">Atualizar as propriedades de um objeto de [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="f8e2c-113">Update the properties of a [calendar](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f8e2c-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f8e2c-114">Properties</span></span>
|<span data-ttu-id="f8e2c-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8e2c-115">Property</span></span>|<span data-ttu-id="f8e2c-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8e2c-116">Type</span></span>|<span data-ttu-id="f8e2c-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8e2c-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8e2c-118">id</span><span class="sxs-lookup"><span data-stu-id="f8e2c-118">id</span></span>|<span data-ttu-id="f8e2c-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8e2c-119">String</span></span>|<span data-ttu-id="f8e2c-120">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f8e2c-120">Key of the setting.</span></span>|
|<span data-ttu-id="f8e2c-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="f8e2c-121">pendingCount</span></span>|<span data-ttu-id="f8e2c-122">Int32</span><span class="sxs-lookup"><span data-stu-id="f8e2c-122">Int32</span></span>|<span data-ttu-id="f8e2c-123">Número de dispositivos pendentes</span><span class="sxs-lookup"><span data-stu-id="f8e2c-123">Number of pending devices</span></span>|
|<span data-ttu-id="f8e2c-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="f8e2c-124">notApplicableCount</span></span>|<span data-ttu-id="f8e2c-125">Int32</span><span class="sxs-lookup"><span data-stu-id="f8e2c-125">Int32</span></span>|<span data-ttu-id="f8e2c-126">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="f8e2c-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="f8e2c-127">successCount</span><span class="sxs-lookup"><span data-stu-id="f8e2c-127">successCount</span></span>|<span data-ttu-id="f8e2c-128">Int32</span><span class="sxs-lookup"><span data-stu-id="f8e2c-128">Int32</span></span>|<span data-ttu-id="f8e2c-129">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="f8e2c-129">Number of succeeded devices</span></span>|
|<span data-ttu-id="f8e2c-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="f8e2c-130">errorCount</span></span>|<span data-ttu-id="f8e2c-131">Int32</span><span class="sxs-lookup"><span data-stu-id="f8e2c-131">Int32</span></span>|<span data-ttu-id="f8e2c-132">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="f8e2c-132">Number of error devices</span></span>|
|<span data-ttu-id="f8e2c-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="f8e2c-133">failedCount</span></span>|<span data-ttu-id="f8e2c-134">Int32</span><span class="sxs-lookup"><span data-stu-id="f8e2c-134">Int32</span></span>|<span data-ttu-id="f8e2c-135">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="f8e2c-135">Number of failed devices</span></span>|
|<span data-ttu-id="f8e2c-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f8e2c-136">lastUpdateDateTime</span></span>|<span data-ttu-id="f8e2c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8e2c-137">DateTimeOffset</span></span>|<span data-ttu-id="f8e2c-138">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="f8e2c-138">Last update time</span></span>|
|<span data-ttu-id="f8e2c-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="f8e2c-139">configurationVersion</span></span>|<span data-ttu-id="f8e2c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f8e2c-140">Int32</span></span>|<span data-ttu-id="f8e2c-141">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="f8e2c-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8e2c-142">Relações</span><span class="sxs-lookup"><span data-stu-id="f8e2c-142">Relationships</span></span>
<span data-ttu-id="f8e2c-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f8e2c-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f8e2c-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f8e2c-144">JSON Representation</span></span>
<span data-ttu-id="f8e2c-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f8e2c-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



