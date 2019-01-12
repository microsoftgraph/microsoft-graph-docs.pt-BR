---
title: Tipo de recurso roleDefinition
description: 'O recurso de Definição de Função. A definição da função é a base do acesso baseado em função no Intune. A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso. Existem dois tipos de funções: internas e personalizadas. Funções internas não podem ser modificadas. Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas. Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.'
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: e2394fdd260f895d9da3dc36df8579490f0382b4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982901"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="b93e5-109">Tipo de recurso roleDefinition</span><span class="sxs-lookup"><span data-stu-id="b93e5-109">roleDefinition resource type</span></span>

> <span data-ttu-id="b93e5-110">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b93e5-110">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b93e5-111">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b93e5-111">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b93e5-112">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b93e5-112">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b93e5-113">O recurso de Definição de Função.</span><span class="sxs-lookup"><span data-stu-id="b93e5-113">The Role Definition resource.</span></span> <span data-ttu-id="b93e5-114">A definição da função é a base do acesso baseado em função no Intune.</span><span class="sxs-lookup"><span data-stu-id="b93e5-114">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="b93e5-115">A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso.</span><span class="sxs-lookup"><span data-stu-id="b93e5-115">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="b93e5-116">Existem dois tipos de funções: internas e personalizadas.</span><span class="sxs-lookup"><span data-stu-id="b93e5-116">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="b93e5-117">Funções internas não podem ser modificadas.</span><span class="sxs-lookup"><span data-stu-id="b93e5-117">Built-in roles cannot be modified.</span></span> <span data-ttu-id="b93e5-118">Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas.</span><span class="sxs-lookup"><span data-stu-id="b93e5-118">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="b93e5-119">Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.</span><span class="sxs-lookup"><span data-stu-id="b93e5-119">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>
## <a name="methods"></a><span data-ttu-id="b93e5-120">Métodos</span><span class="sxs-lookup"><span data-stu-id="b93e5-120">Methods</span></span>
|<span data-ttu-id="b93e5-121">Método</span><span class="sxs-lookup"><span data-stu-id="b93e5-121">Method</span></span>|<span data-ttu-id="b93e5-122">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b93e5-122">Return Type</span></span>|<span data-ttu-id="b93e5-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b93e5-123">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b93e5-124">Listar roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="b93e5-124">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="b93e5-125">Coleção [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b93e5-125">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="b93e5-126">Listar propriedades e relações dos objetos [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="b93e5-126">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="b93e5-127">Obter roleDefinition</span><span class="sxs-lookup"><span data-stu-id="b93e5-127">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|[<span data-ttu-id="b93e5-128">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="b93e5-128">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="b93e5-129">Ler propriedades e relações do objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="b93e5-129">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="b93e5-130">Criar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="b93e5-130">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|[<span data-ttu-id="b93e5-131">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="b93e5-131">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="b93e5-132">Criar um novo objeto [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b93e5-132">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="b93e5-133">Excluir roleDefinition</span><span class="sxs-lookup"><span data-stu-id="b93e5-133">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="b93e5-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b93e5-134">None</span></span>|<span data-ttu-id="b93e5-135">Excluir um [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b93e5-135">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="b93e5-136">Atualizar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="b93e5-136">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="b93e5-137">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="b93e5-137">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="b93e5-138">Atualizar as propriedades de um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="b93e5-138">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b93e5-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b93e5-139">Properties</span></span>
|<span data-ttu-id="b93e5-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b93e5-140">Property</span></span>|<span data-ttu-id="b93e5-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="b93e5-141">Type</span></span>|<span data-ttu-id="b93e5-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="b93e5-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b93e5-143">id</span><span class="sxs-lookup"><span data-stu-id="b93e5-143">id</span></span>|<span data-ttu-id="b93e5-144">String</span><span class="sxs-lookup"><span data-stu-id="b93e5-144">String</span></span>|<span data-ttu-id="b93e5-145">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b93e5-145">Key of the entity.</span></span> <span data-ttu-id="b93e5-146">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="b93e5-146">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="b93e5-147">displayName</span><span class="sxs-lookup"><span data-stu-id="b93e5-147">displayName</span></span>|<span data-ttu-id="b93e5-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b93e5-148">String</span></span>|<span data-ttu-id="b93e5-149">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="b93e5-149">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="b93e5-150">description</span><span class="sxs-lookup"><span data-stu-id="b93e5-150">description</span></span>|<span data-ttu-id="b93e5-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b93e5-151">String</span></span>|<span data-ttu-id="b93e5-152">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="b93e5-152">Description of the Role definition.</span></span>|
|<span data-ttu-id="b93e5-153">permissions</span><span class="sxs-lookup"><span data-stu-id="b93e5-153">permissions</span></span>|<span data-ttu-id="b93e5-154">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="b93e5-154">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="b93e5-155">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="b93e5-155">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="b93e5-156">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="b93e5-156">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="b93e5-157">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="b93e5-157">rolePermissions</span></span>|<span data-ttu-id="b93e5-158">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="b93e5-158">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="b93e5-159">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="b93e5-159">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="b93e5-160">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="b93e5-160">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="b93e5-161">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="b93e5-161">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="b93e5-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="b93e5-162">Boolean</span></span>|<span data-ttu-id="b93e5-163">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="b93e5-163">Type of Role.</span></span> <span data-ttu-id="b93e5-164">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="b93e5-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="b93e5-165">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="b93e5-165">isBuiltIn</span></span>|<span data-ttu-id="b93e5-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="b93e5-166">Boolean</span></span>|<span data-ttu-id="b93e5-167">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="b93e5-167">Type of Role.</span></span> <span data-ttu-id="b93e5-168">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="b93e5-168">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b93e5-169">Relações</span><span class="sxs-lookup"><span data-stu-id="b93e5-169">Relationships</span></span>
|<span data-ttu-id="b93e5-170">Relação</span><span class="sxs-lookup"><span data-stu-id="b93e5-170">Relationship</span></span>|<span data-ttu-id="b93e5-171">Tipo</span><span class="sxs-lookup"><span data-stu-id="b93e5-171">Type</span></span>|<span data-ttu-id="b93e5-172">Descrição</span><span class="sxs-lookup"><span data-stu-id="b93e5-172">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b93e5-173">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="b93e5-173">roleAssignments</span></span>|<span data-ttu-id="b93e5-174">Coleção [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b93e5-174">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="b93e5-175">Lista de atribuições de função para esta definição de função.</span><span class="sxs-lookup"><span data-stu-id="b93e5-175">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b93e5-176">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b93e5-176">JSON Representation</span></span>
<span data-ttu-id="b93e5-177">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b93e5-177">Here is a JSON representation of the resource.</span></span>
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
  "isBuiltIn": true
}
```





