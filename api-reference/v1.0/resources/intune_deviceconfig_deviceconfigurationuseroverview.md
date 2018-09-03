# <a name="deviceconfigurationuseroverview-resource-type"></a><span data-ttu-id="30916-101">Tipo de recurso deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="30916-101">deviceConfigurationUserOverview resource type</span></span>

> <span data-ttu-id="30916-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="30916-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="30916-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="30916-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="30916-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="30916-104">Methods</span></span>
|<span data-ttu-id="30916-105">Método</span><span class="sxs-lookup"><span data-stu-id="30916-105">Method</span></span>|<span data-ttu-id="30916-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="30916-106">Return Type</span></span>|<span data-ttu-id="30916-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="30916-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="30916-108">Obter deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="30916-108">Get deviceConfigurationUserOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationuseroverview_get.md)|[<span data-ttu-id="30916-109">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="30916-109">deviceConfigurationUserOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|<span data-ttu-id="30916-110">Ler propriedades e relações de objetos de [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="30916-110">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) object.</span></span>|
|[<span data-ttu-id="30916-111">Atualizar deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="30916-111">Update deviceConfigurationUserOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationuseroverview_update.md)|[<span data-ttu-id="30916-112">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="30916-112">deviceConfigurationUserOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|<span data-ttu-id="30916-113">Atualizar as propriedades de um objeto de [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="30916-113">Update the properties of a [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="30916-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="30916-114">Properties</span></span>
|<span data-ttu-id="30916-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="30916-115">Property</span></span>|<span data-ttu-id="30916-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="30916-116">Type</span></span>|<span data-ttu-id="30916-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="30916-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30916-118">id</span><span class="sxs-lookup"><span data-stu-id="30916-118">id</span></span>|<span data-ttu-id="30916-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="30916-119">String</span></span>|<span data-ttu-id="30916-120">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="30916-120">Key of the entity.</span></span>|
|<span data-ttu-id="30916-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="30916-121">pendingCount</span></span>|<span data-ttu-id="30916-122">Int32</span><span class="sxs-lookup"><span data-stu-id="30916-122">Int32</span></span>|<span data-ttu-id="30916-123">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="30916-123">Number of pending Users</span></span>|
|<span data-ttu-id="30916-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="30916-124">notApplicableCount</span></span>|<span data-ttu-id="30916-125">Int32</span><span class="sxs-lookup"><span data-stu-id="30916-125">Int32</span></span>|<span data-ttu-id="30916-126">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="30916-126">Number of not applicable users.</span></span>|
|<span data-ttu-id="30916-127">successCount</span><span class="sxs-lookup"><span data-stu-id="30916-127">successCount</span></span>|<span data-ttu-id="30916-128">Int32</span><span class="sxs-lookup"><span data-stu-id="30916-128">Int32</span></span>|<span data-ttu-id="30916-129">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="30916-129">Number of succeeded Users</span></span>|
|<span data-ttu-id="30916-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="30916-130">errorCount</span></span>|<span data-ttu-id="30916-131">Int32</span><span class="sxs-lookup"><span data-stu-id="30916-131">Int32</span></span>|<span data-ttu-id="30916-132">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="30916-132">Number of error Users</span></span>|
|<span data-ttu-id="30916-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="30916-133">failedCount</span></span>|<span data-ttu-id="30916-134">Int32</span><span class="sxs-lookup"><span data-stu-id="30916-134">Int32</span></span>|<span data-ttu-id="30916-135">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="30916-135">Number of failed Users</span></span>|
|<span data-ttu-id="30916-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="30916-136">lastUpdateDateTime</span></span>|<span data-ttu-id="30916-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30916-137">DateTimeOffset</span></span>|<span data-ttu-id="30916-138">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="30916-138">Last update time</span></span>|
|<span data-ttu-id="30916-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="30916-139">configurationVersion</span></span>|<span data-ttu-id="30916-140">Int32</span><span class="sxs-lookup"><span data-stu-id="30916-140">Int32</span></span>|<span data-ttu-id="30916-141">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="30916-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="30916-142">Relações</span><span class="sxs-lookup"><span data-stu-id="30916-142">Relationships</span></span>
<span data-ttu-id="30916-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="30916-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="30916-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="30916-144">JSON Representation</span></span>
<span data-ttu-id="30916-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="30916-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceConfigurationUserOverview"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
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



