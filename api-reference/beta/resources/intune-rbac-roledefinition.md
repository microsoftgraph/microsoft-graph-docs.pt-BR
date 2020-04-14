---
title: Tipo de recurso roleDefinition
description: 'O recurso de Definição de Função. A definição da função é a base do acesso baseado em função no Intune. A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso. Existem dois tipos de funções: internas e personalizadas. Funções internas não podem ser modificadas. Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas. Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.'
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8570b97edc71a86e5ade007a3d7d512683ca4332
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43356937"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="3be95-109">Tipo de recurso roleDefinition</span><span class="sxs-lookup"><span data-stu-id="3be95-109">roleDefinition resource type</span></span>

<span data-ttu-id="3be95-110">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3be95-110">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3be95-111">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3be95-111">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3be95-112">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3be95-112">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3be95-113">O recurso de Definição de Função.</span><span class="sxs-lookup"><span data-stu-id="3be95-113">The Role Definition resource.</span></span> <span data-ttu-id="3be95-114">A definição da função é a base do acesso baseado em função no Intune.</span><span class="sxs-lookup"><span data-stu-id="3be95-114">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="3be95-115">A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso.</span><span class="sxs-lookup"><span data-stu-id="3be95-115">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="3be95-116">Existem dois tipos de funções: internas e personalizadas.</span><span class="sxs-lookup"><span data-stu-id="3be95-116">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="3be95-117">Funções internas não podem ser modificadas.</span><span class="sxs-lookup"><span data-stu-id="3be95-117">Built-in roles cannot be modified.</span></span> <span data-ttu-id="3be95-118">Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas.</span><span class="sxs-lookup"><span data-stu-id="3be95-118">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="3be95-119">Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.</span><span class="sxs-lookup"><span data-stu-id="3be95-119">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

## <a name="methods"></a><span data-ttu-id="3be95-120">Métodos</span><span class="sxs-lookup"><span data-stu-id="3be95-120">Methods</span></span>
|<span data-ttu-id="3be95-121">Método</span><span class="sxs-lookup"><span data-stu-id="3be95-121">Method</span></span>|<span data-ttu-id="3be95-122">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3be95-122">Return Type</span></span>|<span data-ttu-id="3be95-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3be95-123">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3be95-124">Listar roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="3be95-124">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="3be95-125">Coleção [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3be95-125">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="3be95-126">Listar propriedades e relações dos objetos [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3be95-126">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="3be95-127">Obter roleDefinition</span><span class="sxs-lookup"><span data-stu-id="3be95-127">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|[<span data-ttu-id="3be95-128">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="3be95-128">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="3be95-129">Ler propriedades e relações do objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3be95-129">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="3be95-130">Criar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="3be95-130">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|[<span data-ttu-id="3be95-131">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="3be95-131">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="3be95-132">Criar um novo objeto [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3be95-132">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="3be95-133">Excluir roleDefinition</span><span class="sxs-lookup"><span data-stu-id="3be95-133">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="3be95-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3be95-134">None</span></span>|<span data-ttu-id="3be95-135">Excluir um [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3be95-135">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="3be95-136">Atualizar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="3be95-136">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="3be95-137">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="3be95-137">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="3be95-138">Atualizar as propriedades de um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3be95-138">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3be95-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3be95-139">Properties</span></span>
|<span data-ttu-id="3be95-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3be95-140">Property</span></span>|<span data-ttu-id="3be95-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="3be95-141">Type</span></span>|<span data-ttu-id="3be95-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="3be95-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3be95-143">id</span><span class="sxs-lookup"><span data-stu-id="3be95-143">id</span></span>|<span data-ttu-id="3be95-144">String</span><span class="sxs-lookup"><span data-stu-id="3be95-144">String</span></span>|<span data-ttu-id="3be95-145">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3be95-145">Key of the entity.</span></span> <span data-ttu-id="3be95-146">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="3be95-146">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="3be95-147">displayName</span><span class="sxs-lookup"><span data-stu-id="3be95-147">displayName</span></span>|<span data-ttu-id="3be95-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3be95-148">String</span></span>|<span data-ttu-id="3be95-149">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="3be95-149">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="3be95-150">description</span><span class="sxs-lookup"><span data-stu-id="3be95-150">description</span></span>|<span data-ttu-id="3be95-151">String</span><span class="sxs-lookup"><span data-stu-id="3be95-151">String</span></span>|<span data-ttu-id="3be95-152">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="3be95-152">Description of the Role definition.</span></span>|
|<span data-ttu-id="3be95-153">permissões</span><span class="sxs-lookup"><span data-stu-id="3be95-153">permissions</span></span>|<span data-ttu-id="3be95-154">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="3be95-154">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="3be95-155">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="3be95-155">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="3be95-156">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="3be95-156">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="3be95-157">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="3be95-157">rolePermissions</span></span>|<span data-ttu-id="3be95-158">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="3be95-158">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="3be95-159">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="3be95-159">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="3be95-160">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="3be95-160">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="3be95-161">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="3be95-161">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="3be95-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="3be95-162">Boolean</span></span>|<span data-ttu-id="3be95-163">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="3be95-163">Type of Role.</span></span> <span data-ttu-id="3be95-164">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="3be95-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="3be95-165">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="3be95-165">isBuiltIn</span></span>|<span data-ttu-id="3be95-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="3be95-166">Boolean</span></span>|<span data-ttu-id="3be95-167">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="3be95-167">Type of Role.</span></span> <span data-ttu-id="3be95-168">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="3be95-168">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="3be95-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3be95-169">roleScopeTagIds</span></span>|<span data-ttu-id="3be95-170">Coleção String</span><span class="sxs-lookup"><span data-stu-id="3be95-170">String collection</span></span>|<span data-ttu-id="3be95-171">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="3be95-171">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3be95-172">Relações</span><span class="sxs-lookup"><span data-stu-id="3be95-172">Relationships</span></span>
|<span data-ttu-id="3be95-173">Relação</span><span class="sxs-lookup"><span data-stu-id="3be95-173">Relationship</span></span>|<span data-ttu-id="3be95-174">Tipo</span><span class="sxs-lookup"><span data-stu-id="3be95-174">Type</span></span>|<span data-ttu-id="3be95-175">Descrição</span><span class="sxs-lookup"><span data-stu-id="3be95-175">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3be95-176">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="3be95-176">roleAssignments</span></span>|<span data-ttu-id="3be95-177">Coleção [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3be95-177">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="3be95-178">Lista de atribuições de função para esta definição de função.</span><span class="sxs-lookup"><span data-stu-id="3be95-178">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3be95-179">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3be95-179">JSON Representation</span></span>
<span data-ttu-id="3be95-180">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3be95-180">Here is a JSON representation of the resource.</span></span>
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



