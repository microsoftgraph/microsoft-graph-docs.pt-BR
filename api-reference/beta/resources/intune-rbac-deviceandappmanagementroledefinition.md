---
title: Tipo de recurso deviceAndAppManagementRoleDefinition
description: 'O recurso de Definição de Função. A definição da função é a base do acesso baseado em função no Intune. A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso. Existem dois tipos de funções: internas e personalizadas. Funções internas não podem ser modificadas. Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas. Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.'
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5ec33dc83ab0e6389fb45b09b2873b9290aa55ee
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337563"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="8e6b6-109">Tipo de recurso deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="8e6b6-109">deviceAndAppManagementRoleDefinition resource type</span></span>

> <span data-ttu-id="8e6b6-110">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8e6b6-110">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e6b6-111">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8e6b6-111">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e6b6-112">O recurso de Definição de Função.</span><span class="sxs-lookup"><span data-stu-id="8e6b6-112">The Role Definition resource.</span></span> <span data-ttu-id="8e6b6-113">A definição da função é a base do acesso baseado em função no Intune.</span><span class="sxs-lookup"><span data-stu-id="8e6b6-113">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="8e6b6-114">A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso.</span><span class="sxs-lookup"><span data-stu-id="8e6b6-114">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="8e6b6-115">Existem dois tipos de funções: internas e personalizadas.</span><span class="sxs-lookup"><span data-stu-id="8e6b6-115">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="8e6b6-116">Funções internas não podem ser modificadas.</span><span class="sxs-lookup"><span data-stu-id="8e6b6-116">Built-in roles cannot be modified.</span></span> <span data-ttu-id="8e6b6-117">Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas.</span><span class="sxs-lookup"><span data-stu-id="8e6b6-117">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="8e6b6-118">Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.</span><span class="sxs-lookup"><span data-stu-id="8e6b6-118">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>


<span data-ttu-id="8e6b6-119">Herda de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8e6b6-119">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="8e6b6-120">Métodos</span><span class="sxs-lookup"><span data-stu-id="8e6b6-120">Methods</span></span>
|<span data-ttu-id="8e6b6-121">Método</span><span class="sxs-lookup"><span data-stu-id="8e6b6-121">Method</span></span>|<span data-ttu-id="8e6b6-122">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8e6b6-122">Return Type</span></span>|<span data-ttu-id="8e6b6-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e6b6-123">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8e6b6-124">Listar deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="8e6b6-124">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="8e6b6-125">Coleção [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8e6b6-125">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="8e6b6-126">Lista propriedades e relações dos objetos [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="8e6b6-126">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="8e6b6-127">Obter deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="8e6b6-127">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="8e6b6-128">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="8e6b6-128">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="8e6b6-129">Propriedades de leitura e relações do objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="8e6b6-129">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="8e6b6-130">Criar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="8e6b6-130">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="8e6b6-131">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="8e6b6-131">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="8e6b6-132">Cria um novo objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="8e6b6-132">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="8e6b6-133">Excluir deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="8e6b6-133">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="8e6b6-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8e6b6-134">None</span></span>|<span data-ttu-id="8e6b6-135">Exclui um [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="8e6b6-135">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="8e6b6-136">Atualizar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="8e6b6-136">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="8e6b6-137">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="8e6b6-137">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="8e6b6-138">Atualiza as propriedades de um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="8e6b6-138">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8e6b6-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8e6b6-139">Properties</span></span>
|<span data-ttu-id="8e6b6-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e6b6-140">Property</span></span>|<span data-ttu-id="8e6b6-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e6b6-141">Type</span></span>|<span data-ttu-id="8e6b6-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e6b6-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e6b6-143">id</span><span class="sxs-lookup"><span data-stu-id="8e6b6-143">id</span></span>|<span data-ttu-id="8e6b6-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e6b6-144">String</span></span>|<span data-ttu-id="8e6b6-145">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8e6b6-145">Key of the entity.</span></span> <span data-ttu-id="8e6b6-146">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="8e6b6-146">This is read-only and automatically generated.</span></span> <span data-ttu-id="8e6b6-147">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8e6b6-147">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="8e6b6-148">displayName</span><span class="sxs-lookup"><span data-stu-id="8e6b6-148">displayName</span></span>|<span data-ttu-id="8e6b6-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e6b6-149">String</span></span>|<span data-ttu-id="8e6b6-150">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="8e6b6-150">Display Name of the Role definition.</span></span> <span data-ttu-id="8e6b6-151">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8e6b6-151">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="8e6b6-152">descrição</span><span class="sxs-lookup"><span data-stu-id="8e6b6-152">description</span></span>|<span data-ttu-id="8e6b6-153">String</span><span class="sxs-lookup"><span data-stu-id="8e6b6-153">String</span></span>|<span data-ttu-id="8e6b6-154">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="8e6b6-154">Description of the Role definition.</span></span> <span data-ttu-id="8e6b6-155">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8e6b6-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="8e6b6-156">permissões</span><span class="sxs-lookup"><span data-stu-id="8e6b6-156">permissions</span></span>|<span data-ttu-id="8e6b6-157">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="8e6b6-157">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="8e6b6-158">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="8e6b6-158">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="8e6b6-159">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="8e6b6-159">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="8e6b6-160">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8e6b6-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="8e6b6-161">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="8e6b6-161">rolePermissions</span></span>|<span data-ttu-id="8e6b6-162">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="8e6b6-162">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="8e6b6-163">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="8e6b6-163">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="8e6b6-164">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="8e6b6-164">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="8e6b6-165">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8e6b6-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="8e6b6-166">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="8e6b6-166">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="8e6b6-167">Booliano</span><span class="sxs-lookup"><span data-stu-id="8e6b6-167">Boolean</span></span>|<span data-ttu-id="8e6b6-168">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="8e6b6-168">Type of Role.</span></span> <span data-ttu-id="8e6b6-169">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="8e6b6-169">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="8e6b6-170">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8e6b6-170">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="8e6b6-171">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="8e6b6-171">isBuiltIn</span></span>|<span data-ttu-id="8e6b6-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="8e6b6-172">Boolean</span></span>|<span data-ttu-id="8e6b6-173">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="8e6b6-173">Type of Role.</span></span> <span data-ttu-id="8e6b6-174">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="8e6b6-174">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="8e6b6-175">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8e6b6-175">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="8e6b6-176">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8e6b6-176">roleScopeTagIds</span></span>|<span data-ttu-id="8e6b6-177">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e6b6-177">String collection</span></span>|<span data-ttu-id="8e6b6-178">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="8e6b6-178">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8e6b6-179">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8e6b6-179">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e6b6-180">Relações</span><span class="sxs-lookup"><span data-stu-id="8e6b6-180">Relationships</span></span>
|<span data-ttu-id="8e6b6-181">Relação</span><span class="sxs-lookup"><span data-stu-id="8e6b6-181">Relationship</span></span>|<span data-ttu-id="8e6b6-182">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e6b6-182">Type</span></span>|<span data-ttu-id="8e6b6-183">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e6b6-183">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e6b6-184">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="8e6b6-184">roleAssignments</span></span>|<span data-ttu-id="8e6b6-185">Coleção [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8e6b6-185">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="8e6b6-186">Lista de atribuições de função para esta definição de função.</span><span class="sxs-lookup"><span data-stu-id="8e6b6-186">List of Role assignments for this role definition.</span></span> <span data-ttu-id="8e6b6-187">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8e6b6-187">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8e6b6-188">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8e6b6-188">JSON Representation</span></span>
<span data-ttu-id="8e6b6-189">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8e6b6-189">Here is a JSON representation of the resource.</span></span>
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



