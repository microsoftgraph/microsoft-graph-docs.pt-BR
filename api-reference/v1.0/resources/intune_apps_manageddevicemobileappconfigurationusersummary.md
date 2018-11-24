# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="bdb02-101">Tipo de recurso managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="bdb02-101">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

> <span data-ttu-id="bdb02-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bdb02-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bdb02-103">Contém propriedades, propriedades herdadas e ações para um resumo de status do usuário da configuração do aplicativo móvel de MDM.</span><span class="sxs-lookup"><span data-stu-id="bdb02-103">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>
## <a name="methods"></a><span data-ttu-id="bdb02-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="bdb02-104">Methods</span></span>
|<span data-ttu-id="bdb02-105">Método</span><span class="sxs-lookup"><span data-stu-id="bdb02-105">Method</span></span>|<span data-ttu-id="bdb02-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bdb02-106">Return Type</span></span>|<span data-ttu-id="bdb02-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdb02-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bdb02-108">Obter managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="bdb02-108">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationusersummary_get.md)|[<span data-ttu-id="bdb02-109">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="bdb02-109">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="bdb02-110">Ler propriedades e relações de objetos de [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="bdb02-110">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="bdb02-111">Atualizar managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="bdb02-111">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationusersummary_update.md)|[<span data-ttu-id="bdb02-112">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="bdb02-112">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="bdb02-113">Atualizar as propriedades de um objeto de [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="bdb02-113">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bdb02-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bdb02-114">Properties</span></span>
|<span data-ttu-id="bdb02-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bdb02-115">Property</span></span>|<span data-ttu-id="bdb02-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdb02-116">Type</span></span>|<span data-ttu-id="bdb02-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdb02-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdb02-118">id</span><span class="sxs-lookup"><span data-stu-id="bdb02-118">id</span></span>|<span data-ttu-id="bdb02-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bdb02-119">String</span></span>|<span data-ttu-id="bdb02-120">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bdb02-120">Key of the entity.</span></span>|
|<span data-ttu-id="bdb02-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="bdb02-121">pendingCount</span></span>|<span data-ttu-id="bdb02-122">Int32</span><span class="sxs-lookup"><span data-stu-id="bdb02-122">Int32</span></span>|<span data-ttu-id="bdb02-123">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="bdb02-123">Number of pending Users</span></span>|
|<span data-ttu-id="bdb02-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="bdb02-124">notApplicableCount</span></span>|<span data-ttu-id="bdb02-125">Int32</span><span class="sxs-lookup"><span data-stu-id="bdb02-125">Int32</span></span>|<span data-ttu-id="bdb02-126">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="bdb02-126">Number of not applicable users</span></span>|
|<span data-ttu-id="bdb02-127">successCount</span><span class="sxs-lookup"><span data-stu-id="bdb02-127">successCount</span></span>|<span data-ttu-id="bdb02-128">Int32</span><span class="sxs-lookup"><span data-stu-id="bdb02-128">Int32</span></span>|<span data-ttu-id="bdb02-129">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="bdb02-129">Number of succeeded Users</span></span>|
|<span data-ttu-id="bdb02-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="bdb02-130">errorCount</span></span>|<span data-ttu-id="bdb02-131">Int32</span><span class="sxs-lookup"><span data-stu-id="bdb02-131">Int32</span></span>|<span data-ttu-id="bdb02-132">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="bdb02-132">Number of error Users</span></span>|
|<span data-ttu-id="bdb02-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="bdb02-133">failedCount</span></span>|<span data-ttu-id="bdb02-134">Int32</span><span class="sxs-lookup"><span data-stu-id="bdb02-134">Int32</span></span>|<span data-ttu-id="bdb02-135">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="bdb02-135">Number of failed Users</span></span>|
|<span data-ttu-id="bdb02-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="bdb02-136">lastUpdateDateTime</span></span>|<span data-ttu-id="bdb02-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdb02-137">DateTimeOffset</span></span>|<span data-ttu-id="bdb02-138">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="bdb02-138">Last update time</span></span>|
|<span data-ttu-id="bdb02-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="bdb02-139">configurationVersion</span></span>|<span data-ttu-id="bdb02-140">Int32</span><span class="sxs-lookup"><span data-stu-id="bdb02-140">Int32</span></span>|<span data-ttu-id="bdb02-141">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="bdb02-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdb02-142">Relações</span><span class="sxs-lookup"><span data-stu-id="bdb02-142">Relationships</span></span>
<span data-ttu-id="bdb02-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bdb02-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bdb02-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bdb02-144">JSON Representation</span></span>
<span data-ttu-id="bdb02-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bdb02-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationUserSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
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



