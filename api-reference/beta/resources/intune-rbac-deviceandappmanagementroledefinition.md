---
title: Tipo de recurso deviceAndAppManagementRoleDefinition
description: 'O recurso de Definição de Função. A definição da função é a base do acesso baseado em função no Intune. A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso. Existem dois tipos de funções: internas e personalizadas. Funções internas não podem ser modificadas. Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas. Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.'
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: abe28e4b36c62df049e5f85b910e27f787bce2bb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922890"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="7d5a2-109">Tipo de recurso deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7d5a2-109">deviceAndAppManagementRoleDefinition resource type</span></span>

> <span data-ttu-id="7d5a2-110">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7d5a2-110">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d5a2-111">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7d5a2-111">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7d5a2-112">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7d5a2-112">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d5a2-113">O recurso de Definição de Função.</span><span class="sxs-lookup"><span data-stu-id="7d5a2-113">The Role Definition resource.</span></span> <span data-ttu-id="7d5a2-114">A definição da função é a base do acesso baseado em função no Intune.</span><span class="sxs-lookup"><span data-stu-id="7d5a2-114">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="7d5a2-115">A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso.</span><span class="sxs-lookup"><span data-stu-id="7d5a2-115">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="7d5a2-116">Existem dois tipos de funções: internas e personalizadas.</span><span class="sxs-lookup"><span data-stu-id="7d5a2-116">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="7d5a2-117">Funções internas não podem ser modificadas.</span><span class="sxs-lookup"><span data-stu-id="7d5a2-117">Built-in roles cannot be modified.</span></span> <span data-ttu-id="7d5a2-118">Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas.</span><span class="sxs-lookup"><span data-stu-id="7d5a2-118">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="7d5a2-119">Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.</span><span class="sxs-lookup"><span data-stu-id="7d5a2-119">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

<span data-ttu-id="7d5a2-120">Herda de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7d5a2-120">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="7d5a2-121">Métodos</span><span class="sxs-lookup"><span data-stu-id="7d5a2-121">Methods</span></span>
|<span data-ttu-id="7d5a2-122">Método</span><span class="sxs-lookup"><span data-stu-id="7d5a2-122">Method</span></span>|<span data-ttu-id="7d5a2-123">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7d5a2-123">Return Type</span></span>|<span data-ttu-id="7d5a2-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d5a2-124">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7d5a2-125">Listar deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="7d5a2-125">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="7d5a2-126">Coleção [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7d5a2-126">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="7d5a2-127">Lista propriedades e relações dos objetos [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7d5a2-127">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="7d5a2-128">Obter deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7d5a2-128">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="7d5a2-129">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7d5a2-129">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="7d5a2-130">Propriedades de leitura e relações do objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7d5a2-130">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="7d5a2-131">Criar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7d5a2-131">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="7d5a2-132">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7d5a2-132">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="7d5a2-133">Cria um novo objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7d5a2-133">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="7d5a2-134">Excluir deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7d5a2-134">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="7d5a2-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7d5a2-135">None</span></span>|<span data-ttu-id="7d5a2-136">Exclui um [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7d5a2-136">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="7d5a2-137">Atualizar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7d5a2-137">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="7d5a2-138">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7d5a2-138">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="7d5a2-139">Atualiza as propriedades de um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7d5a2-139">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7d5a2-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7d5a2-140">Properties</span></span>
|<span data-ttu-id="7d5a2-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d5a2-141">Property</span></span>|<span data-ttu-id="7d5a2-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d5a2-142">Type</span></span>|<span data-ttu-id="7d5a2-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d5a2-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d5a2-144">id</span><span class="sxs-lookup"><span data-stu-id="7d5a2-144">id</span></span>|<span data-ttu-id="7d5a2-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d5a2-145">String</span></span>|<span data-ttu-id="7d5a2-146">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7d5a2-146">Key of the entity.</span></span> <span data-ttu-id="7d5a2-147">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="7d5a2-147">This is read-only and automatically generated.</span></span> <span data-ttu-id="7d5a2-148">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7d5a2-148">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="7d5a2-149">displayName</span><span class="sxs-lookup"><span data-stu-id="7d5a2-149">displayName</span></span>|<span data-ttu-id="7d5a2-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d5a2-150">String</span></span>|<span data-ttu-id="7d5a2-151">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="7d5a2-151">Display Name of the Role definition.</span></span> <span data-ttu-id="7d5a2-152">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7d5a2-152">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="7d5a2-153">description</span><span class="sxs-lookup"><span data-stu-id="7d5a2-153">description</span></span>|<span data-ttu-id="7d5a2-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d5a2-154">String</span></span>|<span data-ttu-id="7d5a2-155">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="7d5a2-155">Description of the Role definition.</span></span> <span data-ttu-id="7d5a2-156">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7d5a2-156">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="7d5a2-157">permissions</span><span class="sxs-lookup"><span data-stu-id="7d5a2-157">permissions</span></span>|<span data-ttu-id="7d5a2-158">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="7d5a2-158">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="7d5a2-159">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="7d5a2-159">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="7d5a2-160">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="7d5a2-160">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="7d5a2-161">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7d5a2-161">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="7d5a2-162">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="7d5a2-162">rolePermissions</span></span>|<span data-ttu-id="7d5a2-163">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="7d5a2-163">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="7d5a2-164">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="7d5a2-164">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="7d5a2-165">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="7d5a2-165">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="7d5a2-166">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7d5a2-166">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="7d5a2-167">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7d5a2-167">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="7d5a2-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d5a2-168">Boolean</span></span>|<span data-ttu-id="7d5a2-169">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="7d5a2-169">Type of Role.</span></span> <span data-ttu-id="7d5a2-170">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="7d5a2-170">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="7d5a2-171">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7d5a2-171">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="7d5a2-172">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="7d5a2-172">isBuiltIn</span></span>|<span data-ttu-id="7d5a2-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d5a2-173">Boolean</span></span>|<span data-ttu-id="7d5a2-174">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="7d5a2-174">Type of Role.</span></span> <span data-ttu-id="7d5a2-175">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="7d5a2-175">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="7d5a2-176">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7d5a2-176">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d5a2-177">Relações</span><span class="sxs-lookup"><span data-stu-id="7d5a2-177">Relationships</span></span>
|<span data-ttu-id="7d5a2-178">Relação</span><span class="sxs-lookup"><span data-stu-id="7d5a2-178">Relationship</span></span>|<span data-ttu-id="7d5a2-179">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d5a2-179">Type</span></span>|<span data-ttu-id="7d5a2-180">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d5a2-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d5a2-181">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="7d5a2-181">roleAssignments</span></span>|<span data-ttu-id="7d5a2-182">Coleção [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7d5a2-182">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="7d5a2-183">Lista de atribuições de função para esta definição de função.</span><span class="sxs-lookup"><span data-stu-id="7d5a2-183">List of Role assignments for this role definition.</span></span> <span data-ttu-id="7d5a2-184">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7d5a2-184">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7d5a2-185">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7d5a2-185">JSON Representation</span></span>
<span data-ttu-id="7d5a2-186">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7d5a2-186">Here is a JSON representation of the resource.</span></span>
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
  "isBuiltIn": true
}
```





