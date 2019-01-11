---
title: Tipo de recurso deviceAndAppManagementRoleDefinition
description: 'O recurso de Definição de Função. A definição da função é a base do acesso baseado em função no Intune. A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso. Existem dois tipos de funções: internas e personalizadas. Funções internas não podem ser modificadas. Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas. Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.'
localization_priority: Normal
ms.openlocfilehash: a7bdf06be22c2efb11e7fbccf2bd76e5bb9459a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805254"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="75766-109">Tipo de recurso deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="75766-109">deviceAndAppManagementRoleDefinition resource type</span></span>

> <span data-ttu-id="75766-110">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="75766-110">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75766-111">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="75766-111">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="75766-112">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="75766-112">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="75766-113">O recurso de Definição de Função.</span><span class="sxs-lookup"><span data-stu-id="75766-113">The Role Definition resource.</span></span> <span data-ttu-id="75766-114">A definição da função é a base do acesso baseado em função no Intune.</span><span class="sxs-lookup"><span data-stu-id="75766-114">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="75766-115">A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso.</span><span class="sxs-lookup"><span data-stu-id="75766-115">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="75766-116">Existem dois tipos de funções: internas e personalizadas.</span><span class="sxs-lookup"><span data-stu-id="75766-116">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="75766-117">Funções internas não podem ser modificadas.</span><span class="sxs-lookup"><span data-stu-id="75766-117">Built-in roles cannot be modified.</span></span> <span data-ttu-id="75766-118">Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas.</span><span class="sxs-lookup"><span data-stu-id="75766-118">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="75766-119">Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.</span><span class="sxs-lookup"><span data-stu-id="75766-119">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

<span data-ttu-id="75766-120">Herda de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="75766-120">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="75766-121">Métodos</span><span class="sxs-lookup"><span data-stu-id="75766-121">Methods</span></span>
|<span data-ttu-id="75766-122">Método</span><span class="sxs-lookup"><span data-stu-id="75766-122">Method</span></span>|<span data-ttu-id="75766-123">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="75766-123">Return Type</span></span>|<span data-ttu-id="75766-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="75766-124">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="75766-125">Listar deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="75766-125">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="75766-126">Coleção [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="75766-126">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="75766-127">Lista propriedades e relações dos objetos [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="75766-127">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="75766-128">Obter deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="75766-128">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="75766-129">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="75766-129">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="75766-130">Propriedades de leitura e relações do objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="75766-130">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="75766-131">Criar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="75766-131">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="75766-132">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="75766-132">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="75766-133">Cria um novo objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="75766-133">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="75766-134">Excluir deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="75766-134">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="75766-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="75766-135">None</span></span>|<span data-ttu-id="75766-136">Exclui um [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="75766-136">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="75766-137">Atualizar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="75766-137">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="75766-138">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="75766-138">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="75766-139">Atualiza as propriedades de um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="75766-139">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="75766-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="75766-140">Properties</span></span>
|<span data-ttu-id="75766-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75766-141">Property</span></span>|<span data-ttu-id="75766-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="75766-142">Type</span></span>|<span data-ttu-id="75766-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="75766-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75766-144">id</span><span class="sxs-lookup"><span data-stu-id="75766-144">id</span></span>|<span data-ttu-id="75766-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75766-145">String</span></span>|<span data-ttu-id="75766-146">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="75766-146">Key of the entity.</span></span> <span data-ttu-id="75766-147">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="75766-147">This is read-only and automatically generated.</span></span> <span data-ttu-id="75766-148">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="75766-148">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="75766-149">displayName</span><span class="sxs-lookup"><span data-stu-id="75766-149">displayName</span></span>|<span data-ttu-id="75766-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75766-150">String</span></span>|<span data-ttu-id="75766-151">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="75766-151">Display Name of the Role definition.</span></span> <span data-ttu-id="75766-152">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="75766-152">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="75766-153">description</span><span class="sxs-lookup"><span data-stu-id="75766-153">description</span></span>|<span data-ttu-id="75766-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75766-154">String</span></span>|<span data-ttu-id="75766-155">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="75766-155">Description of the Role definition.</span></span> <span data-ttu-id="75766-156">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="75766-156">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="75766-157">permissions</span><span class="sxs-lookup"><span data-stu-id="75766-157">permissions</span></span>|<span data-ttu-id="75766-158">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="75766-158">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="75766-159">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="75766-159">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="75766-160">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="75766-160">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="75766-161">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="75766-161">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="75766-162">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="75766-162">rolePermissions</span></span>|<span data-ttu-id="75766-163">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="75766-163">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="75766-164">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="75766-164">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="75766-165">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="75766-165">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="75766-166">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="75766-166">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="75766-167">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="75766-167">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="75766-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="75766-168">Boolean</span></span>|<span data-ttu-id="75766-169">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="75766-169">Type of Role.</span></span> <span data-ttu-id="75766-170">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="75766-170">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="75766-171">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="75766-171">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="75766-172">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="75766-172">isBuiltIn</span></span>|<span data-ttu-id="75766-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="75766-173">Boolean</span></span>|<span data-ttu-id="75766-174">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="75766-174">Type of Role.</span></span> <span data-ttu-id="75766-175">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="75766-175">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="75766-176">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="75766-176">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="75766-177">Relações</span><span class="sxs-lookup"><span data-stu-id="75766-177">Relationships</span></span>
|<span data-ttu-id="75766-178">Relação</span><span class="sxs-lookup"><span data-stu-id="75766-178">Relationship</span></span>|<span data-ttu-id="75766-179">Tipo</span><span class="sxs-lookup"><span data-stu-id="75766-179">Type</span></span>|<span data-ttu-id="75766-180">Descrição</span><span class="sxs-lookup"><span data-stu-id="75766-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75766-181">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="75766-181">roleAssignments</span></span>|<span data-ttu-id="75766-182">Coleção [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="75766-182">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="75766-183">Lista de atribuições de função para esta definição de função.</span><span class="sxs-lookup"><span data-stu-id="75766-183">List of Role assignments for this role definition.</span></span> <span data-ttu-id="75766-184">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="75766-184">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="75766-185">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75766-185">JSON Representation</span></span>
<span data-ttu-id="75766-186">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="75766-186">Here is a JSON representation of the resource.</span></span>
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





