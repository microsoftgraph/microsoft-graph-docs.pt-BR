---
title: Tipo de recurso deviceAndAppManagementRoleDefinition
description: 'O recurso de Definição de Função. A definição da função é a base do acesso baseado em função no Intune. A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso. Existem dois tipos de funções: internas e personalizadas. Funções internas não podem ser modificadas. Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas. Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.'
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 59efe22098f5da0f95da848b1f64a6545c7680f7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42773767"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="3de98-109">Tipo de recurso deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="3de98-109">deviceAndAppManagementRoleDefinition resource type</span></span>

> <span data-ttu-id="3de98-110">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3de98-110">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3de98-111">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3de98-111">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3de98-112">O recurso de Definição de Função.</span><span class="sxs-lookup"><span data-stu-id="3de98-112">The Role Definition resource.</span></span> <span data-ttu-id="3de98-113">A definição da função é a base do acesso baseado em função no Intune.</span><span class="sxs-lookup"><span data-stu-id="3de98-113">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="3de98-114">A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso.</span><span class="sxs-lookup"><span data-stu-id="3de98-114">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="3de98-115">Existem dois tipos de funções: internas e personalizadas.</span><span class="sxs-lookup"><span data-stu-id="3de98-115">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="3de98-116">Funções internas não podem ser modificadas.</span><span class="sxs-lookup"><span data-stu-id="3de98-116">Built-in roles cannot be modified.</span></span> <span data-ttu-id="3de98-117">Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas.</span><span class="sxs-lookup"><span data-stu-id="3de98-117">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="3de98-118">Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.</span><span class="sxs-lookup"><span data-stu-id="3de98-118">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>


<span data-ttu-id="3de98-119">Herda de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3de98-119">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="3de98-120">Métodos</span><span class="sxs-lookup"><span data-stu-id="3de98-120">Methods</span></span>
|<span data-ttu-id="3de98-121">Método</span><span class="sxs-lookup"><span data-stu-id="3de98-121">Method</span></span>|<span data-ttu-id="3de98-122">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3de98-122">Return Type</span></span>|<span data-ttu-id="3de98-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3de98-123">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3de98-124">Listar deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="3de98-124">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="3de98-125">Coleção [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3de98-125">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="3de98-126">Lista propriedades e relações dos objetos [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3de98-126">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="3de98-127">Obter deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="3de98-127">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="3de98-128">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="3de98-128">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="3de98-129">Propriedades de leitura e relações do objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3de98-129">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="3de98-130">Criar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="3de98-130">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="3de98-131">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="3de98-131">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="3de98-132">Cria um novo objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3de98-132">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="3de98-133">Excluir deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="3de98-133">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="3de98-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3de98-134">None</span></span>|<span data-ttu-id="3de98-135">Exclui um [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3de98-135">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="3de98-136">Atualizar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="3de98-136">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="3de98-137">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="3de98-137">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="3de98-138">Atualiza as propriedades de um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3de98-138">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3de98-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3de98-139">Properties</span></span>
|<span data-ttu-id="3de98-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3de98-140">Property</span></span>|<span data-ttu-id="3de98-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="3de98-141">Type</span></span>|<span data-ttu-id="3de98-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="3de98-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3de98-143">id</span><span class="sxs-lookup"><span data-stu-id="3de98-143">id</span></span>|<span data-ttu-id="3de98-144">String</span><span class="sxs-lookup"><span data-stu-id="3de98-144">String</span></span>|<span data-ttu-id="3de98-145">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3de98-145">Key of the entity.</span></span> <span data-ttu-id="3de98-146">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="3de98-146">This is read-only and automatically generated.</span></span> <span data-ttu-id="3de98-147">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3de98-147">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3de98-148">displayName</span><span class="sxs-lookup"><span data-stu-id="3de98-148">displayName</span></span>|<span data-ttu-id="3de98-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3de98-149">String</span></span>|<span data-ttu-id="3de98-150">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="3de98-150">Display Name of the Role definition.</span></span> <span data-ttu-id="3de98-151">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3de98-151">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3de98-152">description</span><span class="sxs-lookup"><span data-stu-id="3de98-152">description</span></span>|<span data-ttu-id="3de98-153">String</span><span class="sxs-lookup"><span data-stu-id="3de98-153">String</span></span>|<span data-ttu-id="3de98-154">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="3de98-154">Description of the Role definition.</span></span> <span data-ttu-id="3de98-155">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3de98-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3de98-156">permissões</span><span class="sxs-lookup"><span data-stu-id="3de98-156">permissions</span></span>|<span data-ttu-id="3de98-157">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="3de98-157">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="3de98-158">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="3de98-158">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="3de98-159">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="3de98-159">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="3de98-160">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3de98-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3de98-161">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="3de98-161">rolePermissions</span></span>|<span data-ttu-id="3de98-162">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="3de98-162">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="3de98-163">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="3de98-163">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="3de98-164">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="3de98-164">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="3de98-165">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3de98-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3de98-166">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="3de98-166">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="3de98-167">Booliano</span><span class="sxs-lookup"><span data-stu-id="3de98-167">Boolean</span></span>|<span data-ttu-id="3de98-168">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="3de98-168">Type of Role.</span></span> <span data-ttu-id="3de98-169">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="3de98-169">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="3de98-170">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3de98-170">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3de98-171">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="3de98-171">isBuiltIn</span></span>|<span data-ttu-id="3de98-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="3de98-172">Boolean</span></span>|<span data-ttu-id="3de98-173">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="3de98-173">Type of Role.</span></span> <span data-ttu-id="3de98-174">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="3de98-174">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="3de98-175">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3de98-175">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3de98-176">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3de98-176">roleScopeTagIds</span></span>|<span data-ttu-id="3de98-177">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3de98-177">String collection</span></span>|<span data-ttu-id="3de98-178">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="3de98-178">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3de98-179">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3de98-179">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="3de98-180">Relações</span><span class="sxs-lookup"><span data-stu-id="3de98-180">Relationships</span></span>
|<span data-ttu-id="3de98-181">Relação</span><span class="sxs-lookup"><span data-stu-id="3de98-181">Relationship</span></span>|<span data-ttu-id="3de98-182">Tipo</span><span class="sxs-lookup"><span data-stu-id="3de98-182">Type</span></span>|<span data-ttu-id="3de98-183">Descrição</span><span class="sxs-lookup"><span data-stu-id="3de98-183">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3de98-184">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="3de98-184">roleAssignments</span></span>|<span data-ttu-id="3de98-185">Coleção [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3de98-185">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="3de98-186">Lista de atribuições de função para esta definição de função.</span><span class="sxs-lookup"><span data-stu-id="3de98-186">List of Role assignments for this role definition.</span></span> <span data-ttu-id="3de98-187">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3de98-187">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3de98-188">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3de98-188">JSON Representation</span></span>
<span data-ttu-id="3de98-189">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3de98-189">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "permissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "String"
      ],
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
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "String"
      ],
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
  "isBuiltInRoleDefinition": true,
  "isBuiltIn": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```



