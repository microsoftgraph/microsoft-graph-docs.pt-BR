# <a name="roledefinition-resource-type"></a><span data-ttu-id="c7cac-101">Tipo de recurso roleDefinition</span><span class="sxs-lookup"><span data-stu-id="c7cac-101">roleDefinition resource type</span></span>

> <span data-ttu-id="c7cac-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c7cac-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7cac-103">O recurso de Definição de Função.</span><span class="sxs-lookup"><span data-stu-id="c7cac-103">The Role Definition resource.</span></span> <span data-ttu-id="c7cac-104">A definição da função é a base do acesso baseado em função no Intune.</span><span class="sxs-lookup"><span data-stu-id="c7cac-104">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="c7cac-105">A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso.</span><span class="sxs-lookup"><span data-stu-id="c7cac-105">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="c7cac-106">Existem dois tipos de funções: internas e personalizadas.</span><span class="sxs-lookup"><span data-stu-id="c7cac-106">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="c7cac-107">Funções internas não podem ser modificadas.</span><span class="sxs-lookup"><span data-stu-id="c7cac-107">Built-in roles cannot be modified.</span></span> <span data-ttu-id="c7cac-108">Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas.</span><span class="sxs-lookup"><span data-stu-id="c7cac-108">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="c7cac-109">Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.</span><span class="sxs-lookup"><span data-stu-id="c7cac-109">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>
## <a name="methods"></a><span data-ttu-id="c7cac-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="c7cac-110">Methods</span></span>
|<span data-ttu-id="c7cac-111">Método</span><span class="sxs-lookup"><span data-stu-id="c7cac-111">Method</span></span>|<span data-ttu-id="c7cac-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c7cac-112">Return Type</span></span>|<span data-ttu-id="c7cac-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7cac-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c7cac-114">Listar roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="c7cac-114">List roleDefinitions</span></span>](../api/intune_rbac_roledefinition_list.md)|<span data-ttu-id="c7cac-115">Coleção [roleDefinition](../resources/intune_rbac_roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c7cac-115">[roleDefinition](../resources/intune_rbac_roledefinition.md) collection</span></span>|<span data-ttu-id="c7cac-116">Listar propriedades e relações dos objetos [roleDefinition](../resources/intune_rbac_roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7cac-116">List properties and relationships of the [roleDefinition](../resources/intune_rbac_roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="c7cac-117">Obter roleDefinition</span><span class="sxs-lookup"><span data-stu-id="c7cac-117">Get roleDefinition</span></span>](../api/intune_rbac_roledefinition_get.md)|[<span data-ttu-id="c7cac-118">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="c7cac-118">roleDefinition</span></span>](../resources/intune_rbac_roledefinition.md)|<span data-ttu-id="c7cac-119">Ler propriedades e relações do objeto [roleDefinition](../resources/intune_rbac_roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7cac-119">Read properties and relationships of the [roleDefinition](../resources/intune_rbac_roledefinition.md) object.</span></span>|
|[<span data-ttu-id="c7cac-120">Criar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="c7cac-120">Create roleDefinition</span></span>](../api/intune_rbac_roledefinition_create.md)|[<span data-ttu-id="c7cac-121">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="c7cac-121">roleDefinition</span></span>](../resources/intune_rbac_roledefinition.md)|<span data-ttu-id="c7cac-122">Criar um novo objeto [roleDefinition](../resources/intune_rbac_roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c7cac-122">Create a new [roleDefinition](../resources/intune_rbac_roledefinition.md) object.</span></span>|
|[<span data-ttu-id="c7cac-123">Excluir roleDefinition</span><span class="sxs-lookup"><span data-stu-id="c7cac-123">Delete roleDefinition</span></span>](../api/intune_rbac_roledefinition_delete.md)|<span data-ttu-id="c7cac-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c7cac-124">None</span></span>|<span data-ttu-id="c7cac-125">Excluir um [roleDefinition](../resources/intune_rbac_roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c7cac-125">Deletes a [roleDefinition](../resources/intune_rbac_roledefinition.md).</span></span>|
|[<span data-ttu-id="c7cac-126">Atualizar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="c7cac-126">Update roleDefinition</span></span>](../api/intune_rbac_roledefinition_update.md)|[<span data-ttu-id="c7cac-127">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="c7cac-127">roleDefinition</span></span>](../resources/intune_rbac_roledefinition.md)|<span data-ttu-id="c7cac-128">Atualizar as propriedades de um objeto [roleDefinition](../resources/intune_rbac_roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7cac-128">Update the properties of a [roleDefinition](../resources/intune_rbac_roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c7cac-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c7cac-129">Properties</span></span>
|<span data-ttu-id="c7cac-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7cac-130">Property</span></span>|<span data-ttu-id="c7cac-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7cac-131">Type</span></span>|<span data-ttu-id="c7cac-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7cac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7cac-133">id</span><span class="sxs-lookup"><span data-stu-id="c7cac-133">id</span></span>|<span data-ttu-id="c7cac-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7cac-134">String</span></span>|<span data-ttu-id="c7cac-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c7cac-135">Key of the entity.</span></span> <span data-ttu-id="c7cac-136">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="c7cac-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="c7cac-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c7cac-137">displayName</span></span>|<span data-ttu-id="c7cac-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7cac-138">String</span></span>|<span data-ttu-id="c7cac-139">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="c7cac-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="c7cac-140">description</span><span class="sxs-lookup"><span data-stu-id="c7cac-140">description</span></span>|<span data-ttu-id="c7cac-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7cac-141">String</span></span>|<span data-ttu-id="c7cac-142">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="c7cac-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="c7cac-143">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="c7cac-143">rolePermissions</span></span>|<span data-ttu-id="c7cac-144">Coleção [rolePermission](../resources/intune_rbac_rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="c7cac-144">[rolePermission](../resources/intune_rbac_rolepermission.md) collection</span></span>|<span data-ttu-id="c7cac-145">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="c7cac-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="c7cac-146">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="c7cac-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="c7cac-147">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="c7cac-147">isBuiltIn</span></span>|<span data-ttu-id="c7cac-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="c7cac-148">Boolean</span></span>|<span data-ttu-id="c7cac-149">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="c7cac-149">Type of Role.</span></span> <span data-ttu-id="c7cac-150">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="c7cac-150">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7cac-151">Relações</span><span class="sxs-lookup"><span data-stu-id="c7cac-151">Relationships</span></span>
|<span data-ttu-id="c7cac-152">Relação</span><span class="sxs-lookup"><span data-stu-id="c7cac-152">Relationship</span></span>|<span data-ttu-id="c7cac-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7cac-153">Type</span></span>|<span data-ttu-id="c7cac-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7cac-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7cac-155">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="c7cac-155">roleAssignments</span></span>|<span data-ttu-id="c7cac-156">Coleção [roleAssignment](../resources/intune_rbac_roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c7cac-156">[roleAssignment](../resources/intune_rbac_roleassignment.md) collection</span></span>|<span data-ttu-id="c7cac-157">Lista de atribuições de função para esta definição de função.</span><span class="sxs-lookup"><span data-stu-id="c7cac-157">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c7cac-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c7cac-158">JSON Representation</span></span>
<span data-ttu-id="c7cac-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c7cac-159">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleDefinition"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "String"
          ],
          "notAllowedResourceActions": [
            "String"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```








