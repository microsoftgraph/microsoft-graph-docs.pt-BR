---
title: Tipo de recurso roleDefinition
description: 'O recurso de Definição de Função. A definição da função é a base do acesso baseado em função no Intune. A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso. Existem dois tipos de funções: internas e personalizadas. Funções internas não podem ser modificadas. Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas. Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.'
localization_priority: Normal
ms.openlocfilehash: d3f5ef8ddd67302b747b2f35b0e4f62f3f6c00d2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804813"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="93df5-109">Tipo de recurso roleDefinition</span><span class="sxs-lookup"><span data-stu-id="93df5-109">roleDefinition resource type</span></span>

> <span data-ttu-id="93df5-110">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="93df5-110">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="93df5-111">O recurso de Definição de Função.</span><span class="sxs-lookup"><span data-stu-id="93df5-111">The Role Definition resource.</span></span> <span data-ttu-id="93df5-112">A definição da função é a base do acesso baseado em função no Intune.</span><span class="sxs-lookup"><span data-stu-id="93df5-112">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="93df5-113">A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso.</span><span class="sxs-lookup"><span data-stu-id="93df5-113">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="93df5-114">Existem dois tipos de funções: internas e personalizadas.</span><span class="sxs-lookup"><span data-stu-id="93df5-114">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="93df5-115">Funções internas não podem ser modificadas.</span><span class="sxs-lookup"><span data-stu-id="93df5-115">Built-in roles cannot be modified.</span></span> <span data-ttu-id="93df5-116">Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas.</span><span class="sxs-lookup"><span data-stu-id="93df5-116">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="93df5-117">Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.</span><span class="sxs-lookup"><span data-stu-id="93df5-117">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>
## <a name="methods"></a><span data-ttu-id="93df5-118">Métodos</span><span class="sxs-lookup"><span data-stu-id="93df5-118">Methods</span></span>
|<span data-ttu-id="93df5-119">Método</span><span class="sxs-lookup"><span data-stu-id="93df5-119">Method</span></span>|<span data-ttu-id="93df5-120">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="93df5-120">Return Type</span></span>|<span data-ttu-id="93df5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="93df5-121">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="93df5-122">Listar roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="93df5-122">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="93df5-123">Coleção [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="93df5-123">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="93df5-124">Listar propriedades e relações dos objetos [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="93df5-124">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="93df5-125">Obter roleDefinition</span><span class="sxs-lookup"><span data-stu-id="93df5-125">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|[<span data-ttu-id="93df5-126">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="93df5-126">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="93df5-127">Ler propriedades e relações do objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="93df5-127">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="93df5-128">Criar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="93df5-128">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|[<span data-ttu-id="93df5-129">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="93df5-129">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="93df5-130">Criar um novo objeto [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="93df5-130">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="93df5-131">Excluir roleDefinition</span><span class="sxs-lookup"><span data-stu-id="93df5-131">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="93df5-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="93df5-132">None</span></span>|<span data-ttu-id="93df5-133">Excluir um [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="93df5-133">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="93df5-134">Atualizar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="93df5-134">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="93df5-135">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="93df5-135">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="93df5-136">Atualizar as propriedades de um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="93df5-136">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="93df5-137">Propriedades</span><span class="sxs-lookup"><span data-stu-id="93df5-137">Properties</span></span>
|<span data-ttu-id="93df5-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93df5-138">Property</span></span>|<span data-ttu-id="93df5-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="93df5-139">Type</span></span>|<span data-ttu-id="93df5-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="93df5-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93df5-141">id</span><span class="sxs-lookup"><span data-stu-id="93df5-141">id</span></span>|<span data-ttu-id="93df5-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93df5-142">String</span></span>|<span data-ttu-id="93df5-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="93df5-143">Key of the entity.</span></span> <span data-ttu-id="93df5-144">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="93df5-144">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="93df5-145">displayName</span><span class="sxs-lookup"><span data-stu-id="93df5-145">displayName</span></span>|<span data-ttu-id="93df5-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93df5-146">String</span></span>|<span data-ttu-id="93df5-147">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="93df5-147">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="93df5-148">description</span><span class="sxs-lookup"><span data-stu-id="93df5-148">description</span></span>|<span data-ttu-id="93df5-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93df5-149">String</span></span>|<span data-ttu-id="93df5-150">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="93df5-150">Description of the Role definition.</span></span>|
|<span data-ttu-id="93df5-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="93df5-151">rolePermissions</span></span>|<span data-ttu-id="93df5-152">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="93df5-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="93df5-153">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="93df5-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="93df5-154">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="93df5-154">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="93df5-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="93df5-155">isBuiltIn</span></span>|<span data-ttu-id="93df5-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="93df5-156">Boolean</span></span>|<span data-ttu-id="93df5-157">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="93df5-157">Type of Role.</span></span> <span data-ttu-id="93df5-158">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="93df5-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93df5-159">Relações</span><span class="sxs-lookup"><span data-stu-id="93df5-159">Relationships</span></span>
|<span data-ttu-id="93df5-160">Relação</span><span class="sxs-lookup"><span data-stu-id="93df5-160">Relationship</span></span>|<span data-ttu-id="93df5-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="93df5-161">Type</span></span>|<span data-ttu-id="93df5-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="93df5-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93df5-163">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="93df5-163">roleAssignments</span></span>|<span data-ttu-id="93df5-164">Coleção [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="93df5-164">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="93df5-165">Lista de atribuições de função para esta definição de função.</span><span class="sxs-lookup"><span data-stu-id="93df5-165">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="93df5-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="93df5-166">JSON Representation</span></span>
<span data-ttu-id="93df5-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="93df5-167">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleDefinition"
}
-->
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



