# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="119ad-101">Tipo de recurso deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="119ad-101">deviceComplianceUserOverview resource type</span></span>

> <span data-ttu-id="119ad-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="119ad-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="119ad-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="119ad-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="119ad-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="119ad-104">Methods</span></span>
|<span data-ttu-id="119ad-105">Método</span><span class="sxs-lookup"><span data-stu-id="119ad-105">Method</span></span>|<span data-ttu-id="119ad-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="119ad-106">Return Type</span></span>|<span data-ttu-id="119ad-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="119ad-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="119ad-108">Obter deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="119ad-108">Get deviceComplianceUserOverview</span></span>](../api/intune_deviceconfig_devicecomplianceuseroverview_get.md)|[<span data-ttu-id="119ad-109">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="119ad-109">deviceComplianceUserOverview</span></span>](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|<span data-ttu-id="119ad-110">Ler propriedades e relações de objetos de [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="119ad-110">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="119ad-111">Atualizar deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="119ad-111">Update deviceComplianceUserOverview</span></span>](../api/intune_deviceconfig_devicecomplianceuseroverview_update.md)|[<span data-ttu-id="119ad-112">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="119ad-112">deviceComplianceUserOverview</span></span>](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|<span data-ttu-id="119ad-113">Atualizar as propriedades de um objeto de [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="119ad-113">Update the properties of a [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="119ad-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="119ad-114">Properties</span></span>
|<span data-ttu-id="119ad-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="119ad-115">Property</span></span>|<span data-ttu-id="119ad-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="119ad-116">Type</span></span>|<span data-ttu-id="119ad-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="119ad-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="119ad-118">id</span><span class="sxs-lookup"><span data-stu-id="119ad-118">id</span></span>|<span data-ttu-id="119ad-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="119ad-119">String</span></span>|<span data-ttu-id="119ad-120">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="119ad-120">Key of the entity.</span></span>|
|<span data-ttu-id="119ad-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="119ad-121">pendingCount</span></span>|<span data-ttu-id="119ad-122">Int32</span><span class="sxs-lookup"><span data-stu-id="119ad-122">Int32</span></span>|<span data-ttu-id="119ad-123">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="119ad-123">Number of pending Users</span></span>|
|<span data-ttu-id="119ad-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="119ad-124">notApplicableCount</span></span>|<span data-ttu-id="119ad-125">Int32</span><span class="sxs-lookup"><span data-stu-id="119ad-125">Int32</span></span>|<span data-ttu-id="119ad-126">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="119ad-126">Number of not applicable users.</span></span>|
|<span data-ttu-id="119ad-127">successCount</span><span class="sxs-lookup"><span data-stu-id="119ad-127">successCount</span></span>|<span data-ttu-id="119ad-128">Int32</span><span class="sxs-lookup"><span data-stu-id="119ad-128">Int32</span></span>|<span data-ttu-id="119ad-129">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="119ad-129">Number of succeeded Users</span></span>|
|<span data-ttu-id="119ad-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="119ad-130">errorCount</span></span>|<span data-ttu-id="119ad-131">Int32</span><span class="sxs-lookup"><span data-stu-id="119ad-131">Int32</span></span>|<span data-ttu-id="119ad-132">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="119ad-132">Number of error Users</span></span>|
|<span data-ttu-id="119ad-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="119ad-133">failedCount</span></span>|<span data-ttu-id="119ad-134">Int32</span><span class="sxs-lookup"><span data-stu-id="119ad-134">Int32</span></span>|<span data-ttu-id="119ad-135">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="119ad-135">Number of failed Users</span></span>|
|<span data-ttu-id="119ad-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="119ad-136">lastUpdateDateTime</span></span>|<span data-ttu-id="119ad-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="119ad-137">DateTimeOffset</span></span>|<span data-ttu-id="119ad-138">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="119ad-138">Last update time</span></span>|
|<span data-ttu-id="119ad-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="119ad-139">configurationVersion</span></span>|<span data-ttu-id="119ad-140">Int32</span><span class="sxs-lookup"><span data-stu-id="119ad-140">Int32</span></span>|<span data-ttu-id="119ad-141">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="119ad-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="119ad-142">Relações</span><span class="sxs-lookup"><span data-stu-id="119ad-142">Relationships</span></span>
<span data-ttu-id="119ad-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="119ad-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="119ad-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="119ad-144">JSON Representation</span></span>
<span data-ttu-id="119ad-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="119ad-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceComplianceUserOverview"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
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



