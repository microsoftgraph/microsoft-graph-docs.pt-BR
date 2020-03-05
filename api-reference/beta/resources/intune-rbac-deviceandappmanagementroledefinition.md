---
title: Tipo de recurso deviceAndAppManagementRoleDefinition
description: 'O recurso de Definição de Função. A definição da função é a base do acesso baseado em função no Intune. A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso. Existem dois tipos de funções: internas e personalizadas. Funções internas não podem ser modificadas. Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas. Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.'
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 10b9aa204d18820cd7ecabfae23c2cad3d3ac30a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523904"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="9b2e0-109">Tipo de recurso deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="9b2e0-109">deviceAndAppManagementRoleDefinition resource type</span></span>

<span data-ttu-id="9b2e0-110">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9b2e0-110">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b2e0-111">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9b2e0-111">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b2e0-112">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9b2e0-112">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b2e0-113">O recurso de Definição de Função.</span><span class="sxs-lookup"><span data-stu-id="9b2e0-113">The Role Definition resource.</span></span> <span data-ttu-id="9b2e0-114">A definição da função é a base do acesso baseado em função no Intune.</span><span class="sxs-lookup"><span data-stu-id="9b2e0-114">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="9b2e0-115">A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso.</span><span class="sxs-lookup"><span data-stu-id="9b2e0-115">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="9b2e0-116">Existem dois tipos de funções: internas e personalizadas.</span><span class="sxs-lookup"><span data-stu-id="9b2e0-116">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="9b2e0-117">Funções internas não podem ser modificadas.</span><span class="sxs-lookup"><span data-stu-id="9b2e0-117">Built-in roles cannot be modified.</span></span> <span data-ttu-id="9b2e0-118">Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas.</span><span class="sxs-lookup"><span data-stu-id="9b2e0-118">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="9b2e0-119">Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.</span><span class="sxs-lookup"><span data-stu-id="9b2e0-119">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>


<span data-ttu-id="9b2e0-120">Herda de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9b2e0-120">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="9b2e0-121">Métodos</span><span class="sxs-lookup"><span data-stu-id="9b2e0-121">Methods</span></span>
|<span data-ttu-id="9b2e0-122">Método</span><span class="sxs-lookup"><span data-stu-id="9b2e0-122">Method</span></span>|<span data-ttu-id="9b2e0-123">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9b2e0-123">Return Type</span></span>|<span data-ttu-id="9b2e0-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b2e0-124">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9b2e0-125">Listar deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="9b2e0-125">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="9b2e0-126">Coleção [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9b2e0-126">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="9b2e0-127">Lista propriedades e relações dos objetos [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="9b2e0-127">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="9b2e0-128">Obter deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="9b2e0-128">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="9b2e0-129">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="9b2e0-129">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="9b2e0-130">Propriedades de leitura e relações do objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="9b2e0-130">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="9b2e0-131">Criar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="9b2e0-131">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="9b2e0-132">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="9b2e0-132">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="9b2e0-133">Cria um novo objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="9b2e0-133">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="9b2e0-134">Excluir deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="9b2e0-134">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="9b2e0-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9b2e0-135">None</span></span>|<span data-ttu-id="9b2e0-136">Exclui um [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="9b2e0-136">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="9b2e0-137">Atualizar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="9b2e0-137">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="9b2e0-138">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="9b2e0-138">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="9b2e0-139">Atualiza as propriedades de um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="9b2e0-139">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9b2e0-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9b2e0-140">Properties</span></span>
|<span data-ttu-id="9b2e0-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b2e0-141">Property</span></span>|<span data-ttu-id="9b2e0-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b2e0-142">Type</span></span>|<span data-ttu-id="9b2e0-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b2e0-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b2e0-144">id</span><span class="sxs-lookup"><span data-stu-id="9b2e0-144">id</span></span>|<span data-ttu-id="9b2e0-145">String</span><span class="sxs-lookup"><span data-stu-id="9b2e0-145">String</span></span>|<span data-ttu-id="9b2e0-146">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9b2e0-146">Key of the entity.</span></span> <span data-ttu-id="9b2e0-147">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="9b2e0-147">This is read-only and automatically generated.</span></span> <span data-ttu-id="9b2e0-148">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9b2e0-148">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="9b2e0-149">displayName</span><span class="sxs-lookup"><span data-stu-id="9b2e0-149">displayName</span></span>|<span data-ttu-id="9b2e0-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b2e0-150">String</span></span>|<span data-ttu-id="9b2e0-151">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="9b2e0-151">Display Name of the Role definition.</span></span> <span data-ttu-id="9b2e0-152">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9b2e0-152">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="9b2e0-153">description</span><span class="sxs-lookup"><span data-stu-id="9b2e0-153">description</span></span>|<span data-ttu-id="9b2e0-154">String</span><span class="sxs-lookup"><span data-stu-id="9b2e0-154">String</span></span>|<span data-ttu-id="9b2e0-155">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="9b2e0-155">Description of the Role definition.</span></span> <span data-ttu-id="9b2e0-156">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9b2e0-156">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="9b2e0-157">permissões</span><span class="sxs-lookup"><span data-stu-id="9b2e0-157">permissions</span></span>|<span data-ttu-id="9b2e0-158">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="9b2e0-158">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="9b2e0-159">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="9b2e0-159">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="9b2e0-160">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="9b2e0-160">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="9b2e0-161">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9b2e0-161">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="9b2e0-162">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="9b2e0-162">rolePermissions</span></span>|<span data-ttu-id="9b2e0-163">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="9b2e0-163">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="9b2e0-164">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="9b2e0-164">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="9b2e0-165">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="9b2e0-165">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="9b2e0-166">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9b2e0-166">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="9b2e0-167">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="9b2e0-167">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="9b2e0-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="9b2e0-168">Boolean</span></span>|<span data-ttu-id="9b2e0-169">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="9b2e0-169">Type of Role.</span></span> <span data-ttu-id="9b2e0-170">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="9b2e0-170">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="9b2e0-171">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9b2e0-171">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="9b2e0-172">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="9b2e0-172">isBuiltIn</span></span>|<span data-ttu-id="9b2e0-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="9b2e0-173">Boolean</span></span>|<span data-ttu-id="9b2e0-174">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="9b2e0-174">Type of Role.</span></span> <span data-ttu-id="9b2e0-175">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="9b2e0-175">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="9b2e0-176">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9b2e0-176">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="9b2e0-177">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9b2e0-177">roleScopeTagIds</span></span>|<span data-ttu-id="9b2e0-178">String collection</span><span class="sxs-lookup"><span data-stu-id="9b2e0-178">String collection</span></span>|<span data-ttu-id="9b2e0-179">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="9b2e0-179">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9b2e0-180">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9b2e0-180">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b2e0-181">Relações</span><span class="sxs-lookup"><span data-stu-id="9b2e0-181">Relationships</span></span>
|<span data-ttu-id="9b2e0-182">Relação</span><span class="sxs-lookup"><span data-stu-id="9b2e0-182">Relationship</span></span>|<span data-ttu-id="9b2e0-183">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b2e0-183">Type</span></span>|<span data-ttu-id="9b2e0-184">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b2e0-184">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b2e0-185">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="9b2e0-185">roleAssignments</span></span>|<span data-ttu-id="9b2e0-186">Coleção [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9b2e0-186">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="9b2e0-187">Lista de atribuições de função para esta definição de função.</span><span class="sxs-lookup"><span data-stu-id="9b2e0-187">List of Role assignments for this role definition.</span></span> <span data-ttu-id="9b2e0-188">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9b2e0-188">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9b2e0-189">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9b2e0-189">JSON Representation</span></span>
<span data-ttu-id="9b2e0-190">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9b2e0-190">Here is a JSON representation of the resource.</span></span>
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



