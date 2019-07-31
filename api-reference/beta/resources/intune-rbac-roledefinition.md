---
title: Tipo de recurso roleDefinition
description: 'O recurso de Definição de Função. A definição da função é a base do acesso baseado em função no Intune. A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso. Existem dois tipos de funções: internas e personalizadas. Funções internas não podem ser modificadas. Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas. Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.'
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 01f8c24fc536418e88677dbc11d742e6d8b64588
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967557"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="d2bbb-109">Tipo de recurso roleDefinition</span><span class="sxs-lookup"><span data-stu-id="d2bbb-109">roleDefinition resource type</span></span>

> <span data-ttu-id="d2bbb-110">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-110">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2bbb-111">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-111">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2bbb-112">O recurso de Definição de Função.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-112">The Role Definition resource.</span></span> <span data-ttu-id="d2bbb-113">A definição da função é a base do acesso baseado em função no Intune.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-113">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="d2bbb-114">A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-114">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="d2bbb-115">Existem dois tipos de funções: internas e personalizadas.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-115">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="d2bbb-116">Funções internas não podem ser modificadas.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-116">Built-in roles cannot be modified.</span></span> <span data-ttu-id="d2bbb-117">Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-117">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="d2bbb-118">Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-118">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

## <a name="methods"></a><span data-ttu-id="d2bbb-119">Métodos</span><span class="sxs-lookup"><span data-stu-id="d2bbb-119">Methods</span></span>
|<span data-ttu-id="d2bbb-120">Método</span><span class="sxs-lookup"><span data-stu-id="d2bbb-120">Method</span></span>|<span data-ttu-id="d2bbb-121">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d2bbb-121">Return Type</span></span>|<span data-ttu-id="d2bbb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2bbb-122">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d2bbb-123">Listar roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="d2bbb-123">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="d2bbb-124">Coleção [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d2bbb-124">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="d2bbb-125">Listar propriedades e relações dos objetos [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="d2bbb-125">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="d2bbb-126">Obter roleDefinition</span><span class="sxs-lookup"><span data-stu-id="d2bbb-126">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|[<span data-ttu-id="d2bbb-127">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="d2bbb-127">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="d2bbb-128">Ler propriedades e relações do objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="d2bbb-128">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="d2bbb-129">Criar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="d2bbb-129">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|[<span data-ttu-id="d2bbb-130">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="d2bbb-130">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="d2bbb-131">Criar um novo objeto [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d2bbb-131">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="d2bbb-132">Excluir roleDefinition</span><span class="sxs-lookup"><span data-stu-id="d2bbb-132">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="d2bbb-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d2bbb-133">None</span></span>|<span data-ttu-id="d2bbb-134">Excluir um [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d2bbb-134">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="d2bbb-135">Atualizar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="d2bbb-135">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="d2bbb-136">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="d2bbb-136">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="d2bbb-137">Atualizar as propriedades de um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="d2bbb-137">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d2bbb-138">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2bbb-138">Properties</span></span>
|<span data-ttu-id="d2bbb-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2bbb-139">Property</span></span>|<span data-ttu-id="d2bbb-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2bbb-140">Type</span></span>|<span data-ttu-id="d2bbb-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2bbb-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2bbb-142">id</span><span class="sxs-lookup"><span data-stu-id="d2bbb-142">id</span></span>|<span data-ttu-id="d2bbb-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2bbb-143">String</span></span>|<span data-ttu-id="d2bbb-144">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-144">Key of the entity.</span></span> <span data-ttu-id="d2bbb-145">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-145">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="d2bbb-146">displayName</span><span class="sxs-lookup"><span data-stu-id="d2bbb-146">displayName</span></span>|<span data-ttu-id="d2bbb-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2bbb-147">String</span></span>|<span data-ttu-id="d2bbb-148">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-148">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="d2bbb-149">descrição</span><span class="sxs-lookup"><span data-stu-id="d2bbb-149">description</span></span>|<span data-ttu-id="d2bbb-150">String</span><span class="sxs-lookup"><span data-stu-id="d2bbb-150">String</span></span>|<span data-ttu-id="d2bbb-151">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-151">Description of the Role definition.</span></span>|
|<span data-ttu-id="d2bbb-152">permissões</span><span class="sxs-lookup"><span data-stu-id="d2bbb-152">permissions</span></span>|<span data-ttu-id="d2bbb-153">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="d2bbb-153">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="d2bbb-154">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-154">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="d2bbb-155">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-155">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="d2bbb-156">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="d2bbb-156">rolePermissions</span></span>|<span data-ttu-id="d2bbb-157">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="d2bbb-157">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="d2bbb-158">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-158">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="d2bbb-159">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-159">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="d2bbb-160">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d2bbb-160">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="d2bbb-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="d2bbb-161">Boolean</span></span>|<span data-ttu-id="d2bbb-162">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-162">Type of Role.</span></span> <span data-ttu-id="d2bbb-163">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-163">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="d2bbb-164">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="d2bbb-164">isBuiltIn</span></span>|<span data-ttu-id="d2bbb-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="d2bbb-165">Boolean</span></span>|<span data-ttu-id="d2bbb-166">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-166">Type of Role.</span></span> <span data-ttu-id="d2bbb-167">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-167">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="d2bbb-168">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d2bbb-168">roleScopeTagIds</span></span>|<span data-ttu-id="d2bbb-169">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2bbb-169">String collection</span></span>|<span data-ttu-id="d2bbb-170">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-170">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2bbb-171">Relações</span><span class="sxs-lookup"><span data-stu-id="d2bbb-171">Relationships</span></span>
|<span data-ttu-id="d2bbb-172">Relação</span><span class="sxs-lookup"><span data-stu-id="d2bbb-172">Relationship</span></span>|<span data-ttu-id="d2bbb-173">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2bbb-173">Type</span></span>|<span data-ttu-id="d2bbb-174">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2bbb-174">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2bbb-175">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="d2bbb-175">roleAssignments</span></span>|<span data-ttu-id="d2bbb-176">Coleção [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d2bbb-176">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="d2bbb-177">Lista de atribuições de função para esta definição de função.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-177">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d2bbb-178">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2bbb-178">JSON Representation</span></span>
<span data-ttu-id="d2bbb-179">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-179">Here is a JSON representation of the resource.</span></span>
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





