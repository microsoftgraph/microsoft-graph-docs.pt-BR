# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="8ddb8-101">Tipo de recurso managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ddb8-101">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="8ddb8-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8ddb8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ddb8-103">Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="8ddb8-103">An abstract class for Mobile app configuration for enrolled devices.</span></span>
## <a name="methods"></a><span data-ttu-id="8ddb8-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="8ddb8-104">Methods</span></span>
|<span data-ttu-id="8ddb8-105">Método</span><span class="sxs-lookup"><span data-stu-id="8ddb8-105">Method</span></span>|<span data-ttu-id="8ddb8-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8ddb8-106">Return Type</span></span>|<span data-ttu-id="8ddb8-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ddb8-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8ddb8-108">Listar managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="8ddb8-108">List managedDeviceMobileAppConfigurations</span></span>](../api/intune_apps_manageddevicemobileappconfiguration_list.md)|<span data-ttu-id="8ddb8-109">Coleção [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ddb8-109">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="8ddb8-110">Lista propriedades e relações dos objetos [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ddb8-110">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="8ddb8-111">Obter managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ddb8-111">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune_apps_manageddevicemobileappconfiguration_get.md)|[<span data-ttu-id="8ddb8-112">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ddb8-112">managedDeviceMobileAppConfiguration</span></span>](../resources/intune_apps_manageddevicemobileappconfiguration.md)|<span data-ttu-id="8ddb8-113">Propriedades de leitura e relações do objeto [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ddb8-113">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8ddb8-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ddb8-114">Properties</span></span>
|<span data-ttu-id="8ddb8-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ddb8-115">Property</span></span>|<span data-ttu-id="8ddb8-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ddb8-116">Type</span></span>|<span data-ttu-id="8ddb8-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ddb8-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ddb8-118">id</span><span class="sxs-lookup"><span data-stu-id="8ddb8-118">id</span></span>|<span data-ttu-id="8ddb8-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ddb8-119">String</span></span>|<span data-ttu-id="8ddb8-120">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8ddb8-120">Key of the entity.</span></span>|
|<span data-ttu-id="8ddb8-121">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="8ddb8-121">targetedMobileApps</span></span>|<span data-ttu-id="8ddb8-122">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ddb8-122">String collection</span></span>|<span data-ttu-id="8ddb8-123">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="8ddb8-123">the associated app.</span></span>|
|<span data-ttu-id="8ddb8-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ddb8-124">createdDateTime</span></span>|<span data-ttu-id="8ddb8-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ddb8-125">DateTimeOffset</span></span>|<span data-ttu-id="8ddb8-126">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="8ddb8-126">DateTime the object was created.</span></span>|
|<span data-ttu-id="8ddb8-127">description</span><span class="sxs-lookup"><span data-stu-id="8ddb8-127">description</span></span>|<span data-ttu-id="8ddb8-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ddb8-128">String</span></span>|<span data-ttu-id="8ddb8-129">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8ddb8-129">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="8ddb8-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ddb8-130">lastModifiedDateTime</span></span>|<span data-ttu-id="8ddb8-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ddb8-131">DateTimeOffset</span></span>|<span data-ttu-id="8ddb8-132">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="8ddb8-132">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="8ddb8-133">displayName</span><span class="sxs-lookup"><span data-stu-id="8ddb8-133">displayName</span></span>|<span data-ttu-id="8ddb8-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ddb8-134">String</span></span>|<span data-ttu-id="8ddb8-135">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8ddb8-135">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="8ddb8-136">version</span><span class="sxs-lookup"><span data-stu-id="8ddb8-136">version</span></span>|<span data-ttu-id="8ddb8-137">Int32</span><span class="sxs-lookup"><span data-stu-id="8ddb8-137">Int32</span></span>|<span data-ttu-id="8ddb8-138">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8ddb8-138">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ddb8-139">Relações</span><span class="sxs-lookup"><span data-stu-id="8ddb8-139">Relationships</span></span>
|<span data-ttu-id="8ddb8-140">Relação</span><span class="sxs-lookup"><span data-stu-id="8ddb8-140">Relationship</span></span>|<span data-ttu-id="8ddb8-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ddb8-141">Type</span></span>|<span data-ttu-id="8ddb8-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ddb8-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ddb8-143">assignments</span><span class="sxs-lookup"><span data-stu-id="8ddb8-143">assignments</span></span>|<span data-ttu-id="8ddb8-144">Coleção [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8ddb8-144">[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="8ddb8-145">A lista de atribuições de grupo para configuração de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="8ddb8-145">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="8ddb8-146">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="8ddb8-146">deviceStatuses</span></span>|<span data-ttu-id="8ddb8-147">coleção [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="8ddb8-147">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="8ddb8-148">Lista de ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="8ddb8-148">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="8ddb8-149">userStatuses</span><span class="sxs-lookup"><span data-stu-id="8ddb8-149">userStatuses</span></span>|<span data-ttu-id="8ddb8-150">Coleção [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="8ddb8-150">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="8ddb8-151">Lista de ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="8ddb8-151">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="8ddb8-152">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="8ddb8-152">deviceStatusSummary</span></span>|[<span data-ttu-id="8ddb8-153">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="8ddb8-153">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="8ddb8-154">Resumo do status do dispositivo de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8ddb8-154">App configuration device status summary.</span></span>|
|<span data-ttu-id="8ddb8-155">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="8ddb8-155">userStatusSummary</span></span>|[<span data-ttu-id="8ddb8-156">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="8ddb8-156">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="8ddb8-157">Resumo do status do usuário de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8ddb8-157">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8ddb8-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ddb8-158">JSON Representation</span></span>
<span data-ttu-id="8ddb8-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ddb8-159">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
  "id": "String (identifier)",
  "targetedMobileApps": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```








