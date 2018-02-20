# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="22775-101">Tipo de recurso deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="22775-101">deviceAppManagement resource type</span></span>

> <span data-ttu-id="22775-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="22775-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22775-103">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de aplicativos de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="22775-103">Singleton entity that acts as a container for all device app management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="22775-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="22775-104">Methods</span></span>
|<span data-ttu-id="22775-105">Método</span><span class="sxs-lookup"><span data-stu-id="22775-105">Method</span></span>|<span data-ttu-id="22775-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="22775-106">Return Type</span></span>|<span data-ttu-id="22775-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="22775-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="22775-108">Obter deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="22775-108">Get deviceAppManagement</span></span>](../api/intune_apps_deviceappmanagement_get.md)|[<span data-ttu-id="22775-109">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="22775-109">deviceAppManagement</span></span>](../resources/intune_apps_deviceappmanagement.md)|<span data-ttu-id="22775-110">Propriedades de leitura e relações do objeto [deviceAppManagement](../resources/intune_apps_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="22775-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_apps_deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="22775-111">Atualizar deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="22775-111">Update deviceAppManagement</span></span>](../api/intune_apps_deviceappmanagement_update.md)|[<span data-ttu-id="22775-112">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="22775-112">deviceAppManagement</span></span>](../resources/intune_apps_deviceappmanagement.md)|<span data-ttu-id="22775-113">Atualiza as propriedades de um objeto [deviceAppManagement](../resources/intune_apps_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="22775-113">Update the properties of a [calendar](../resources/intune_apps_deviceappmanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="22775-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="22775-114">Properties</span></span>
|<span data-ttu-id="22775-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22775-115">Property</span></span>|<span data-ttu-id="22775-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="22775-116">Type</span></span>|<span data-ttu-id="22775-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="22775-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22775-118">id</span><span class="sxs-lookup"><span data-stu-id="22775-118">id</span></span>|<span data-ttu-id="22775-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22775-119">String</span></span>|<span data-ttu-id="22775-120">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="22775-120">Key of the setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22775-121">Relações</span><span class="sxs-lookup"><span data-stu-id="22775-121">Relationships</span></span>
|<span data-ttu-id="22775-122">Relação</span><span class="sxs-lookup"><span data-stu-id="22775-122">Relationship</span></span>|<span data-ttu-id="22775-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="22775-123">Type</span></span>|<span data-ttu-id="22775-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="22775-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22775-125">mobileApps</span><span class="sxs-lookup"><span data-stu-id="22775-125">mobileApps</span></span>|<span data-ttu-id="22775-126">Coleção [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="22775-126">[mobileApp](../resources/intune_apps_mobileapp.md) collection</span></span>|<span data-ttu-id="22775-127">Os aplicativos móveis.</span><span class="sxs-lookup"><span data-stu-id="22775-127">The mobile apps.</span></span>|
|<span data-ttu-id="22775-128">mobileAppCategories</span><span class="sxs-lookup"><span data-stu-id="22775-128">mobileAppCategories</span></span>|<span data-ttu-id="22775-129">Coleção [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="22775-129">[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) collection</span></span>|<span data-ttu-id="22775-130">As categorias dos aplicativos móveis.</span><span class="sxs-lookup"><span data-stu-id="22775-130">The mobile app categories.</span></span>|
|<span data-ttu-id="22775-131">mobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="22775-131">mobileAppConfigurations</span></span>|<span data-ttu-id="22775-132">Coleção [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22775-132">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="22775-133">As configurações de aplicativos móveis de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="22775-133">The Managed Device Mobile Application Configurations.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="22775-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="22775-134">JSON Representation</span></span>
<span data-ttu-id="22775-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="22775-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```



