# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="e13e2-101">Tipo de recurso deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e13e2-101">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="e13e2-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e13e2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e13e2-103">A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="e13e2-103">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="e13e2-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="e13e2-104">Methods</span></span>
|<span data-ttu-id="e13e2-105">Método</span><span class="sxs-lookup"><span data-stu-id="e13e2-105">Method</span></span>|<span data-ttu-id="e13e2-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e13e2-106">Return Type</span></span>|<span data-ttu-id="e13e2-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="e13e2-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e13e2-108">Listar deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="e13e2-108">List deviceConfigurationAssignments</span></span>](../api/intune_deviceconfig_deviceconfigurationassignment_list.md)|<span data-ttu-id="e13e2-109">Conjunto [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e13e2-109">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="e13e2-110">Listar propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e13e2-110">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="e13e2-111">Obter deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e13e2-111">Get deviceConfigurationAssignment</span></span>](../api/intune_deviceconfig_deviceconfigurationassignment_get.md)|[<span data-ttu-id="e13e2-112">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e13e2-112">deviceConfigurationAssignment</span></span>](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|<span data-ttu-id="e13e2-113">Ler propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e13e2-113">Read properties and relationships of [plannerTaskDetails](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="e13e2-114">Criar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e13e2-114">Create deviceConfigurationAssignment</span></span>](../api/intune_deviceconfig_deviceconfigurationassignment_create.md)|[<span data-ttu-id="e13e2-115">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e13e2-115">deviceConfigurationAssignment</span></span>](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|<span data-ttu-id="e13e2-116">Criar um novo objeto de [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e13e2-116">Create a new [plannerBucket](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="e13e2-117">Excluir deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e13e2-117">Delete deviceConfigurationAssignment</span></span>](../api/intune_deviceconfig_deviceconfigurationassignment_delete.md)|<span data-ttu-id="e13e2-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e13e2-118">None</span></span>|<span data-ttu-id="e13e2-119">Excluir [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e13e2-119">Deletes a [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="e13e2-120">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e13e2-120">Update deviceConfigurationAssignment</span></span>](../api/intune_deviceconfig_deviceconfigurationassignment_update.md)|[<span data-ttu-id="e13e2-121">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e13e2-121">deviceConfigurationAssignment</span></span>](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|<span data-ttu-id="e13e2-122">Atualizar as propriedades de um objeto de [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e13e2-122">Update the properties of a [calendar](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e13e2-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e13e2-123">Properties</span></span>
|<span data-ttu-id="e13e2-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e13e2-124">Property</span></span>|<span data-ttu-id="e13e2-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="e13e2-125">Type</span></span>|<span data-ttu-id="e13e2-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="e13e2-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e13e2-127">id</span><span class="sxs-lookup"><span data-stu-id="e13e2-127">id</span></span>|<span data-ttu-id="e13e2-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e13e2-128">String</span></span>|<span data-ttu-id="e13e2-129">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="e13e2-129">The key of the setting.</span></span>|
|<span data-ttu-id="e13e2-130">destino</span><span class="sxs-lookup"><span data-stu-id="e13e2-130">target</span></span>|[<span data-ttu-id="e13e2-131">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e13e2-131">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_deviceconfig_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e13e2-132">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e13e2-132">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e13e2-133">Relações</span><span class="sxs-lookup"><span data-stu-id="e13e2-133">Relationships</span></span>
<span data-ttu-id="e13e2-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e13e2-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e13e2-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e13e2-135">JSON Representation</span></span>
<span data-ttu-id="e13e2-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e13e2-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



