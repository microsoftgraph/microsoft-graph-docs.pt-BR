# <a name="devicemanagement-resource-type"></a><span data-ttu-id="959d6-101">Tipo de recurso deviceManagement</span><span class="sxs-lookup"><span data-stu-id="959d6-101">deviceManagement resource type</span></span>

> <span data-ttu-id="959d6-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="959d6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="959d6-103">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="959d6-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="959d6-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="959d6-104">Methods</span></span>
|<span data-ttu-id="959d6-105">Método</span><span class="sxs-lookup"><span data-stu-id="959d6-105">Method</span></span>|<span data-ttu-id="959d6-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="959d6-106">Return Type</span></span>|<span data-ttu-id="959d6-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="959d6-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="959d6-108">Obter deviceManagement</span><span class="sxs-lookup"><span data-stu-id="959d6-108">Get deviceManagement</span></span>](../api/intune_rbac_devicemanagement_get.md)|[<span data-ttu-id="959d6-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="959d6-109">deviceManagement</span></span>](../resources/intune_rbac_devicemanagement.md)|<span data-ttu-id="959d6-110">Ler propriedades e relações de objetos de [deviceManagement](../resources/intune_rbac_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="959d6-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_rbac_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="959d6-111">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="959d6-111">Update deviceManagement</span></span>](../api/intune_rbac_devicemanagement_update.md)|[<span data-ttu-id="959d6-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="959d6-112">deviceManagement</span></span>](../resources/intune_rbac_devicemanagement.md)|<span data-ttu-id="959d6-113">Atualizar as propriedades de um objeto de [deviceManagement](../resources/intune_rbac_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="959d6-113">Update the properties of a [calendar](../resources/intune_rbac_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="959d6-114">Função getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="959d6-114">getEffectivePermissions function</span></span>](../api/intune_rbac_devicemanagement_geteffectivepermissions.md)|<span data-ttu-id="959d6-115">Conjunto [rolePermission](../resources/intune_rbac_rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="959d6-115">[rolePermission](../resources/intune_rbac_rolepermission.md) collection</span></span>|<span data-ttu-id="959d6-116">Recupera permissões efetivas de usuário autenticado no momento</span><span class="sxs-lookup"><span data-stu-id="959d6-116">Retrieves the effective permissions of the currently authenticated user</span></span>|

## <a name="properties"></a><span data-ttu-id="959d6-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="959d6-117">Properties</span></span>
|<span data-ttu-id="959d6-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="959d6-118">Property</span></span>|<span data-ttu-id="959d6-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="959d6-119">Type</span></span>|<span data-ttu-id="959d6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="959d6-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="959d6-121">id</span><span class="sxs-lookup"><span data-stu-id="959d6-121">id</span></span>|<span data-ttu-id="959d6-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="959d6-122">String</span></span>|<span data-ttu-id="959d6-123">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="959d6-123">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="959d6-124">Relações</span><span class="sxs-lookup"><span data-stu-id="959d6-124">Relationships</span></span>
|<span data-ttu-id="959d6-125">Relação</span><span class="sxs-lookup"><span data-stu-id="959d6-125">Relationship</span></span>|<span data-ttu-id="959d6-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="959d6-126">Type</span></span>|<span data-ttu-id="959d6-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="959d6-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="959d6-128">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="959d6-128">roleDefinitions</span></span>|<span data-ttu-id="959d6-129">Conjunto [roleDefinition](../resources/intune_rbac_roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="959d6-129">[roleDefinition](../resources/intune_rbac_roledefinition.md) collection</span></span>|<span data-ttu-id="959d6-130">As definições da função.</span><span class="sxs-lookup"><span data-stu-id="959d6-130">The Role Definitions.</span></span>|
|<span data-ttu-id="959d6-131">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="959d6-131">roleAssignments</span></span>|<span data-ttu-id="959d6-132">Conjunto [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="959d6-132">[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) collection</span></span>|<span data-ttu-id="959d6-133">As atribuições da função</span><span class="sxs-lookup"><span data-stu-id="959d6-133">The Role Assignments.</span></span>|
|<span data-ttu-id="959d6-134">resourceOperations</span><span class="sxs-lookup"><span data-stu-id="959d6-134">resourceOperations</span></span>|<span data-ttu-id="959d6-135">Conjunto [resourceOperation](../resources/intune_rbac_resourceoperation.md)</span><span class="sxs-lookup"><span data-stu-id="959d6-135">[resourceOperation](../resources/intune_rbac_resourceoperation.md) collection</span></span>|<span data-ttu-id="959d6-136">As operações de recurso.</span><span class="sxs-lookup"><span data-stu-id="959d6-136">The Resource Operations.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="959d6-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="959d6-137">JSON Representation</span></span>
<span data-ttu-id="959d6-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="959d6-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```



