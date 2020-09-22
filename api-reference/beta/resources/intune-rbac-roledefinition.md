---
title: Tipo de recurso roleDefinition
description: 'O recurso de Definição de Função. A definição da função é a base do acesso baseado em função no Intune. A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso. Existem dois tipos de funções: internas e personalizadas. Funções internas não podem ser modificadas. Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas. Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.'
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d8ec600773f90aba8ecc86bc509efc8da2992fdb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039500"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="7e57c-109">Tipo de recurso roleDefinition</span><span class="sxs-lookup"><span data-stu-id="7e57c-109">roleDefinition resource type</span></span>

<span data-ttu-id="7e57c-110">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e57c-110">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7e57c-111">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7e57c-111">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e57c-112">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7e57c-112">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e57c-113">O recurso de Definição de Função.</span><span class="sxs-lookup"><span data-stu-id="7e57c-113">The Role Definition resource.</span></span> <span data-ttu-id="7e57c-114">A definição da função é a base do acesso baseado em função no Intune.</span><span class="sxs-lookup"><span data-stu-id="7e57c-114">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="7e57c-115">A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso.</span><span class="sxs-lookup"><span data-stu-id="7e57c-115">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="7e57c-116">Existem dois tipos de funções: internas e personalizadas.</span><span class="sxs-lookup"><span data-stu-id="7e57c-116">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="7e57c-117">Funções internas não podem ser modificadas.</span><span class="sxs-lookup"><span data-stu-id="7e57c-117">Built-in roles cannot be modified.</span></span> <span data-ttu-id="7e57c-118">Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas.</span><span class="sxs-lookup"><span data-stu-id="7e57c-118">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="7e57c-119">Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.</span><span class="sxs-lookup"><span data-stu-id="7e57c-119">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

## <a name="methods"></a><span data-ttu-id="7e57c-120">Métodos</span><span class="sxs-lookup"><span data-stu-id="7e57c-120">Methods</span></span>
|<span data-ttu-id="7e57c-121">Método</span><span class="sxs-lookup"><span data-stu-id="7e57c-121">Method</span></span>|<span data-ttu-id="7e57c-122">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7e57c-122">Return Type</span></span>|<span data-ttu-id="7e57c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e57c-123">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7e57c-124">Listar roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="7e57c-124">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="7e57c-125">Coleção [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7e57c-125">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="7e57c-126">Listar propriedades e relações dos objetos [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7e57c-126">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="7e57c-127">Obter roleDefinition</span><span class="sxs-lookup"><span data-stu-id="7e57c-127">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|[<span data-ttu-id="7e57c-128">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="7e57c-128">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="7e57c-129">Ler propriedades e relações do objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7e57c-129">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="7e57c-130">Criar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="7e57c-130">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|[<span data-ttu-id="7e57c-131">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="7e57c-131">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="7e57c-132">Criar um novo objeto [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7e57c-132">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="7e57c-133">Excluir roleDefinition</span><span class="sxs-lookup"><span data-stu-id="7e57c-133">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="7e57c-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7e57c-134">None</span></span>|<span data-ttu-id="7e57c-135">Excluir um [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7e57c-135">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="7e57c-136">Atualizar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="7e57c-136">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="7e57c-137">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="7e57c-137">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="7e57c-138">Atualizar as propriedades de um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7e57c-138">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7e57c-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7e57c-139">Properties</span></span>
|<span data-ttu-id="7e57c-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7e57c-140">Property</span></span>|<span data-ttu-id="7e57c-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e57c-141">Type</span></span>|<span data-ttu-id="7e57c-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e57c-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e57c-143">id</span><span class="sxs-lookup"><span data-stu-id="7e57c-143">id</span></span>|<span data-ttu-id="7e57c-144">String</span><span class="sxs-lookup"><span data-stu-id="7e57c-144">String</span></span>|<span data-ttu-id="7e57c-145">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7e57c-145">Key of the entity.</span></span> <span data-ttu-id="7e57c-146">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="7e57c-146">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="7e57c-147">displayName</span><span class="sxs-lookup"><span data-stu-id="7e57c-147">displayName</span></span>|<span data-ttu-id="7e57c-148">String</span><span class="sxs-lookup"><span data-stu-id="7e57c-148">String</span></span>|<span data-ttu-id="7e57c-149">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="7e57c-149">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="7e57c-150">description</span><span class="sxs-lookup"><span data-stu-id="7e57c-150">description</span></span>|<span data-ttu-id="7e57c-151">String</span><span class="sxs-lookup"><span data-stu-id="7e57c-151">String</span></span>|<span data-ttu-id="7e57c-152">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="7e57c-152">Description of the Role definition.</span></span>|
|<span data-ttu-id="7e57c-153">permissões</span><span class="sxs-lookup"><span data-stu-id="7e57c-153">permissions</span></span>|<span data-ttu-id="7e57c-154">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="7e57c-154">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="7e57c-155">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="7e57c-155">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="7e57c-156">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="7e57c-156">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="7e57c-157">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="7e57c-157">rolePermissions</span></span>|<span data-ttu-id="7e57c-158">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="7e57c-158">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="7e57c-159">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="7e57c-159">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="7e57c-160">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="7e57c-160">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="7e57c-161">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7e57c-161">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="7e57c-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="7e57c-162">Boolean</span></span>|<span data-ttu-id="7e57c-163">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="7e57c-163">Type of Role.</span></span> <span data-ttu-id="7e57c-164">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="7e57c-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="7e57c-165">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="7e57c-165">isBuiltIn</span></span>|<span data-ttu-id="7e57c-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="7e57c-166">Boolean</span></span>|<span data-ttu-id="7e57c-167">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="7e57c-167">Type of Role.</span></span> <span data-ttu-id="7e57c-168">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="7e57c-168">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="7e57c-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7e57c-169">roleScopeTagIds</span></span>|<span data-ttu-id="7e57c-170">Coleção String</span><span class="sxs-lookup"><span data-stu-id="7e57c-170">String collection</span></span>|<span data-ttu-id="7e57c-171">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="7e57c-171">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e57c-172">Relações</span><span class="sxs-lookup"><span data-stu-id="7e57c-172">Relationships</span></span>
|<span data-ttu-id="7e57c-173">Relação</span><span class="sxs-lookup"><span data-stu-id="7e57c-173">Relationship</span></span>|<span data-ttu-id="7e57c-174">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e57c-174">Type</span></span>|<span data-ttu-id="7e57c-175">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e57c-175">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e57c-176">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="7e57c-176">roleAssignments</span></span>|<span data-ttu-id="7e57c-177">Coleção [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7e57c-177">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="7e57c-178">Lista de atribuições de função para esta definição de função.</span><span class="sxs-lookup"><span data-stu-id="7e57c-178">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7e57c-179">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7e57c-179">JSON Representation</span></span>
<span data-ttu-id="7e57c-180">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7e57c-180">Here is a JSON representation of the resource.</span></span>
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






