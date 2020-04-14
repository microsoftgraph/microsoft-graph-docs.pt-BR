---
title: Tipo de recurso deviceAndAppManagementRoleDefinition
description: 'O recurso de Definição de Função. A definição da função é a base do acesso baseado em função no Intune. A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso. Existem dois tipos de funções: internas e personalizadas. Funções internas não podem ser modificadas. Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas. Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.'
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 76f9b2e88bc9d94d9c938f1884207d241257def2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43357734"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="c0c7e-109">Tipo de recurso deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c0c7e-109">deviceAndAppManagementRoleDefinition resource type</span></span>

<span data-ttu-id="c0c7e-110">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0c7e-110">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0c7e-111">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c0c7e-111">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0c7e-112">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c0c7e-112">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0c7e-113">O recurso de Definição de Função.</span><span class="sxs-lookup"><span data-stu-id="c0c7e-113">The Role Definition resource.</span></span> <span data-ttu-id="c0c7e-114">A definição da função é a base do acesso baseado em função no Intune.</span><span class="sxs-lookup"><span data-stu-id="c0c7e-114">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="c0c7e-115">A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso.</span><span class="sxs-lookup"><span data-stu-id="c0c7e-115">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="c0c7e-116">Existem dois tipos de funções: internas e personalizadas.</span><span class="sxs-lookup"><span data-stu-id="c0c7e-116">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="c0c7e-117">Funções internas não podem ser modificadas.</span><span class="sxs-lookup"><span data-stu-id="c0c7e-117">Built-in roles cannot be modified.</span></span> <span data-ttu-id="c0c7e-118">Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas.</span><span class="sxs-lookup"><span data-stu-id="c0c7e-118">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="c0c7e-119">Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.</span><span class="sxs-lookup"><span data-stu-id="c0c7e-119">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>


<span data-ttu-id="c0c7e-120">Herda de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0c7e-120">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c0c7e-121">Métodos</span><span class="sxs-lookup"><span data-stu-id="c0c7e-121">Methods</span></span>
|<span data-ttu-id="c0c7e-122">Método</span><span class="sxs-lookup"><span data-stu-id="c0c7e-122">Method</span></span>|<span data-ttu-id="c0c7e-123">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c0c7e-123">Return Type</span></span>|<span data-ttu-id="c0c7e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0c7e-124">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c0c7e-125">Listar deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="c0c7e-125">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="c0c7e-126">Coleção [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0c7e-126">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="c0c7e-127">Lista propriedades e relações dos objetos [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c0c7e-127">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="c0c7e-128">Obter deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c0c7e-128">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="c0c7e-129">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c0c7e-129">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="c0c7e-130">Propriedades de leitura e relações do objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c0c7e-130">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="c0c7e-131">Criar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c0c7e-131">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="c0c7e-132">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c0c7e-132">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="c0c7e-133">Cria um novo objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c0c7e-133">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="c0c7e-134">Excluir deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c0c7e-134">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="c0c7e-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c0c7e-135">None</span></span>|<span data-ttu-id="c0c7e-136">Exclui um [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c0c7e-136">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="c0c7e-137">Atualizar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c0c7e-137">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="c0c7e-138">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c0c7e-138">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="c0c7e-139">Atualiza as propriedades de um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c0c7e-139">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c0c7e-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c0c7e-140">Properties</span></span>
|<span data-ttu-id="c0c7e-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0c7e-141">Property</span></span>|<span data-ttu-id="c0c7e-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0c7e-142">Type</span></span>|<span data-ttu-id="c0c7e-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0c7e-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0c7e-144">id</span><span class="sxs-lookup"><span data-stu-id="c0c7e-144">id</span></span>|<span data-ttu-id="c0c7e-145">String</span><span class="sxs-lookup"><span data-stu-id="c0c7e-145">String</span></span>|<span data-ttu-id="c0c7e-146">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c0c7e-146">Key of the entity.</span></span> <span data-ttu-id="c0c7e-147">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="c0c7e-147">This is read-only and automatically generated.</span></span> <span data-ttu-id="c0c7e-148">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0c7e-148">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="c0c7e-149">displayName</span><span class="sxs-lookup"><span data-stu-id="c0c7e-149">displayName</span></span>|<span data-ttu-id="c0c7e-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0c7e-150">String</span></span>|<span data-ttu-id="c0c7e-151">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="c0c7e-151">Display Name of the Role definition.</span></span> <span data-ttu-id="c0c7e-152">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0c7e-152">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="c0c7e-153">description</span><span class="sxs-lookup"><span data-stu-id="c0c7e-153">description</span></span>|<span data-ttu-id="c0c7e-154">String</span><span class="sxs-lookup"><span data-stu-id="c0c7e-154">String</span></span>|<span data-ttu-id="c0c7e-155">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="c0c7e-155">Description of the Role definition.</span></span> <span data-ttu-id="c0c7e-156">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0c7e-156">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="c0c7e-157">permissões</span><span class="sxs-lookup"><span data-stu-id="c0c7e-157">permissions</span></span>|<span data-ttu-id="c0c7e-158">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="c0c7e-158">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="c0c7e-159">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="c0c7e-159">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="c0c7e-160">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="c0c7e-160">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="c0c7e-161">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0c7e-161">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="c0c7e-162">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="c0c7e-162">rolePermissions</span></span>|<span data-ttu-id="c0c7e-163">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="c0c7e-163">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="c0c7e-164">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="c0c7e-164">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="c0c7e-165">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="c0c7e-165">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="c0c7e-166">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0c7e-166">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="c0c7e-167">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c0c7e-167">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="c0c7e-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="c0c7e-168">Boolean</span></span>|<span data-ttu-id="c0c7e-169">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="c0c7e-169">Type of Role.</span></span> <span data-ttu-id="c0c7e-170">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="c0c7e-170">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="c0c7e-171">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0c7e-171">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="c0c7e-172">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="c0c7e-172">isBuiltIn</span></span>|<span data-ttu-id="c0c7e-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="c0c7e-173">Boolean</span></span>|<span data-ttu-id="c0c7e-174">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="c0c7e-174">Type of Role.</span></span> <span data-ttu-id="c0c7e-175">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="c0c7e-175">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="c0c7e-176">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0c7e-176">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="c0c7e-177">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c0c7e-177">roleScopeTagIds</span></span>|<span data-ttu-id="c0c7e-178">Coleção String</span><span class="sxs-lookup"><span data-stu-id="c0c7e-178">String collection</span></span>|<span data-ttu-id="c0c7e-179">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="c0c7e-179">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c0c7e-180">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0c7e-180">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0c7e-181">Relações</span><span class="sxs-lookup"><span data-stu-id="c0c7e-181">Relationships</span></span>
|<span data-ttu-id="c0c7e-182">Relação</span><span class="sxs-lookup"><span data-stu-id="c0c7e-182">Relationship</span></span>|<span data-ttu-id="c0c7e-183">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0c7e-183">Type</span></span>|<span data-ttu-id="c0c7e-184">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0c7e-184">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0c7e-185">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="c0c7e-185">roleAssignments</span></span>|<span data-ttu-id="c0c7e-186">Coleção [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c0c7e-186">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="c0c7e-187">Lista de atribuições de função para esta definição de função.</span><span class="sxs-lookup"><span data-stu-id="c0c7e-187">List of Role assignments for this role definition.</span></span> <span data-ttu-id="c0c7e-188">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0c7e-188">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c0c7e-189">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c0c7e-189">JSON Representation</span></span>
<span data-ttu-id="c0c7e-190">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c0c7e-190">Here is a JSON representation of the resource.</span></span>
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



