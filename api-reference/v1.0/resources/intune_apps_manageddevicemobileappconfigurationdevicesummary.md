# <a name="manageddevicemobileappconfigurationdevicesummary-resource-type"></a><span data-ttu-id="f74b9-101">Tipo de recurso managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="f74b9-101">managedDeviceMobileAppConfigurationDeviceSummary resource type</span></span>

> <span data-ttu-id="f74b9-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f74b9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f74b9-103">Contém propriedades, propriedades herdadas e ações para um resumo de status do dispositivo de configuração de aplicativo móvel de MDM.</span><span class="sxs-lookup"><span data-stu-id="f74b9-103">Contains properties, inherited properties and actions for an MDM mobile app configuration device status summary.</span></span>
## <a name="methods"></a><span data-ttu-id="f74b9-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="f74b9-104">Methods</span></span>
|<span data-ttu-id="f74b9-105">Método</span><span class="sxs-lookup"><span data-stu-id="f74b9-105">Method</span></span>|<span data-ttu-id="f74b9-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f74b9-106">Return Type</span></span>|<span data-ttu-id="f74b9-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="f74b9-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f74b9-108">Obter managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="f74b9-108">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationdevicesummary_get.md)|[<span data-ttu-id="f74b9-109">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="f74b9-109">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="f74b9-110">Ler propriedades e relações de objetos de [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="f74b9-110">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|
|[<span data-ttu-id="f74b9-111">Atualizar managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="f74b9-111">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationdevicesummary_update.md)|[<span data-ttu-id="f74b9-112">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="f74b9-112">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="f74b9-113">Atualizar as propriedades de um objeto de [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="f74b9-113">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f74b9-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f74b9-114">Properties</span></span>
|<span data-ttu-id="f74b9-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f74b9-115">Property</span></span>|<span data-ttu-id="f74b9-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="f74b9-116">Type</span></span>|<span data-ttu-id="f74b9-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="f74b9-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f74b9-118">id</span><span class="sxs-lookup"><span data-stu-id="f74b9-118">id</span></span>|<span data-ttu-id="f74b9-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f74b9-119">String</span></span>|<span data-ttu-id="f74b9-120">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f74b9-120">Key of the entity.</span></span>|
|<span data-ttu-id="f74b9-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="f74b9-121">pendingCount</span></span>|<span data-ttu-id="f74b9-122">Int32</span><span class="sxs-lookup"><span data-stu-id="f74b9-122">Int32</span></span>|<span data-ttu-id="f74b9-123">Número de dispositivos pendentes</span><span class="sxs-lookup"><span data-stu-id="f74b9-123">Number of pending devices</span></span>|
|<span data-ttu-id="f74b9-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="f74b9-124">notApplicableCount</span></span>|<span data-ttu-id="f74b9-125">Int32</span><span class="sxs-lookup"><span data-stu-id="f74b9-125">Int32</span></span>|<span data-ttu-id="f74b9-126">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="f74b9-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="f74b9-127">successCount</span><span class="sxs-lookup"><span data-stu-id="f74b9-127">successCount</span></span>|<span data-ttu-id="f74b9-128">Int32</span><span class="sxs-lookup"><span data-stu-id="f74b9-128">Int32</span></span>|<span data-ttu-id="f74b9-129">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="f74b9-129">Number of succeeded devices</span></span>|
|<span data-ttu-id="f74b9-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="f74b9-130">errorCount</span></span>|<span data-ttu-id="f74b9-131">Int32</span><span class="sxs-lookup"><span data-stu-id="f74b9-131">Int32</span></span>|<span data-ttu-id="f74b9-132">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="f74b9-132">Number of error devices</span></span>|
|<span data-ttu-id="f74b9-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="f74b9-133">failedCount</span></span>|<span data-ttu-id="f74b9-134">Int32</span><span class="sxs-lookup"><span data-stu-id="f74b9-134">Int32</span></span>|<span data-ttu-id="f74b9-135">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="f74b9-135">Number of failed devices</span></span>|
|<span data-ttu-id="f74b9-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f74b9-136">lastUpdateDateTime</span></span>|<span data-ttu-id="f74b9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f74b9-137">DateTimeOffset</span></span>|<span data-ttu-id="f74b9-138">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="f74b9-138">Last update time</span></span>|
|<span data-ttu-id="f74b9-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="f74b9-139">configurationVersion</span></span>|<span data-ttu-id="f74b9-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f74b9-140">Int32</span></span>|<span data-ttu-id="f74b9-141">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="f74b9-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="f74b9-142">Relações</span><span class="sxs-lookup"><span data-stu-id="f74b9-142">Relationships</span></span>
<span data-ttu-id="f74b9-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f74b9-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f74b9-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f74b9-144">JSON Representation</span></span>
<span data-ttu-id="f74b9-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f74b9-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary"
}-->
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



