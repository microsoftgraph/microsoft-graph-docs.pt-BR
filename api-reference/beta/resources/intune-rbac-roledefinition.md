---
title: Tipo de recurso roleDefinition
description: 'O recurso de Definição de Função. A definição da função é a base do acesso baseado em função no Intune. A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso. Existem dois tipos de funções: internas e personalizadas. Funções internas não podem ser modificadas. Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas. Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.'
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba38f9293ce4a21d031a3c70e8d3bdbe5667f997
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173714"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="50224-109">Tipo de recurso roleDefinition</span><span class="sxs-lookup"><span data-stu-id="50224-109">roleDefinition resource type</span></span>

> <span data-ttu-id="50224-110">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="50224-110">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50224-111">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="50224-111">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50224-112">O recurso de Definição de Função.</span><span class="sxs-lookup"><span data-stu-id="50224-112">The Role Definition resource.</span></span> <span data-ttu-id="50224-113">A definição da função é a base do acesso baseado em função no Intune.</span><span class="sxs-lookup"><span data-stu-id="50224-113">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="50224-114">A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso.</span><span class="sxs-lookup"><span data-stu-id="50224-114">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="50224-115">Existem dois tipos de funções: internas e personalizadas.</span><span class="sxs-lookup"><span data-stu-id="50224-115">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="50224-116">Funções internas não podem ser modificadas.</span><span class="sxs-lookup"><span data-stu-id="50224-116">Built-in roles cannot be modified.</span></span> <span data-ttu-id="50224-117">Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas.</span><span class="sxs-lookup"><span data-stu-id="50224-117">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="50224-118">Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.</span><span class="sxs-lookup"><span data-stu-id="50224-118">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

## <a name="methods"></a><span data-ttu-id="50224-119">Métodos</span><span class="sxs-lookup"><span data-stu-id="50224-119">Methods</span></span>
|<span data-ttu-id="50224-120">Método</span><span class="sxs-lookup"><span data-stu-id="50224-120">Method</span></span>|<span data-ttu-id="50224-121">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="50224-121">Return Type</span></span>|<span data-ttu-id="50224-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="50224-122">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="50224-123">Listar roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="50224-123">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="50224-124">Coleção [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50224-124">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="50224-125">Listar propriedades e relações dos objetos [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="50224-125">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="50224-126">Obter roleDefinition</span><span class="sxs-lookup"><span data-stu-id="50224-126">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|[<span data-ttu-id="50224-127">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="50224-127">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="50224-128">Ler propriedades e relações do objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="50224-128">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="50224-129">Criar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="50224-129">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|[<span data-ttu-id="50224-130">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="50224-130">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="50224-131">Criar um novo objeto [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50224-131">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="50224-132">Excluir roleDefinition</span><span class="sxs-lookup"><span data-stu-id="50224-132">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="50224-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="50224-133">None</span></span>|<span data-ttu-id="50224-134">Excluir um [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50224-134">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="50224-135">Atualizar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="50224-135">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="50224-136">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="50224-136">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="50224-137">Atualizar as propriedades de um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="50224-137">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="50224-138">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50224-138">Properties</span></span>
|<span data-ttu-id="50224-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50224-139">Property</span></span>|<span data-ttu-id="50224-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="50224-140">Type</span></span>|<span data-ttu-id="50224-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="50224-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50224-142">id</span><span class="sxs-lookup"><span data-stu-id="50224-142">id</span></span>|<span data-ttu-id="50224-143">String</span><span class="sxs-lookup"><span data-stu-id="50224-143">String</span></span>|<span data-ttu-id="50224-144">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="50224-144">Key of the entity.</span></span> <span data-ttu-id="50224-145">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="50224-145">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="50224-146">displayName</span><span class="sxs-lookup"><span data-stu-id="50224-146">displayName</span></span>|<span data-ttu-id="50224-147">String</span><span class="sxs-lookup"><span data-stu-id="50224-147">String</span></span>|<span data-ttu-id="50224-148">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="50224-148">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="50224-149">description</span><span class="sxs-lookup"><span data-stu-id="50224-149">description</span></span>|<span data-ttu-id="50224-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50224-150">String</span></span>|<span data-ttu-id="50224-151">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="50224-151">Description of the Role definition.</span></span>|
|<span data-ttu-id="50224-152">permissions</span><span class="sxs-lookup"><span data-stu-id="50224-152">permissions</span></span>|<span data-ttu-id="50224-153">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="50224-153">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="50224-154">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="50224-154">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="50224-155">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="50224-155">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="50224-156">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="50224-156">rolePermissions</span></span>|<span data-ttu-id="50224-157">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="50224-157">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="50224-158">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="50224-158">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="50224-159">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="50224-159">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="50224-160">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="50224-160">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="50224-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="50224-161">Boolean</span></span>|<span data-ttu-id="50224-162">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="50224-162">Type of Role.</span></span> <span data-ttu-id="50224-163">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="50224-163">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="50224-164">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="50224-164">isBuiltIn</span></span>|<span data-ttu-id="50224-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="50224-165">Boolean</span></span>|<span data-ttu-id="50224-166">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="50224-166">Type of Role.</span></span> <span data-ttu-id="50224-167">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="50224-167">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="50224-168">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="50224-168">roleScopeTagIds</span></span>|<span data-ttu-id="50224-169">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="50224-169">String collection</span></span>|<span data-ttu-id="50224-170">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="50224-170">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50224-171">Relações</span><span class="sxs-lookup"><span data-stu-id="50224-171">Relationships</span></span>
|<span data-ttu-id="50224-172">Relação</span><span class="sxs-lookup"><span data-stu-id="50224-172">Relationship</span></span>|<span data-ttu-id="50224-173">Tipo</span><span class="sxs-lookup"><span data-stu-id="50224-173">Type</span></span>|<span data-ttu-id="50224-174">Descrição</span><span class="sxs-lookup"><span data-stu-id="50224-174">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50224-175">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="50224-175">roleAssignments</span></span>|<span data-ttu-id="50224-176">Coleção [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="50224-176">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="50224-177">Lista de atribuições de função para esta definição de função.</span><span class="sxs-lookup"><span data-stu-id="50224-177">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50224-178">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50224-178">JSON Representation</span></span>
<span data-ttu-id="50224-179">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="50224-179">Here is a JSON representation of the resource.</span></span>
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




