---
title: Tipo de recurso deviceAndAppManagementRoleDefinition
description: 'O recurso de Definição de Função. A definição da função é a base do acesso baseado em função no Intune. A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso. Existem dois tipos de funções: internas e personalizadas. Funções internas não podem ser modificadas. Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas. Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.'
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 52d6360299e4dfc1a3f2d54ebdd64ca6374c15de
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441651"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="d2ed0-109">Tipo de recurso deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d2ed0-109">deviceAndAppManagementRoleDefinition resource type</span></span>

<span data-ttu-id="d2ed0-110">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2ed0-110">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2ed0-111">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d2ed0-111">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2ed0-112">O recurso de Definição de Função.</span><span class="sxs-lookup"><span data-stu-id="d2ed0-112">The Role Definition resource.</span></span> <span data-ttu-id="d2ed0-113">A definição da função é a base do acesso baseado em função no Intune.</span><span class="sxs-lookup"><span data-stu-id="d2ed0-113">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="d2ed0-114">A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso.</span><span class="sxs-lookup"><span data-stu-id="d2ed0-114">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="d2ed0-115">Existem dois tipos de funções: internas e personalizadas.</span><span class="sxs-lookup"><span data-stu-id="d2ed0-115">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="d2ed0-116">Funções internas não podem ser modificadas.</span><span class="sxs-lookup"><span data-stu-id="d2ed0-116">Built-in roles cannot be modified.</span></span> <span data-ttu-id="d2ed0-117">Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas.</span><span class="sxs-lookup"><span data-stu-id="d2ed0-117">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="d2ed0-118">Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.</span><span class="sxs-lookup"><span data-stu-id="d2ed0-118">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>


<span data-ttu-id="d2ed0-119">Herda de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d2ed0-119">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="d2ed0-120">Métodos</span><span class="sxs-lookup"><span data-stu-id="d2ed0-120">Methods</span></span>
|<span data-ttu-id="d2ed0-121">Método</span><span class="sxs-lookup"><span data-stu-id="d2ed0-121">Method</span></span>|<span data-ttu-id="d2ed0-122">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d2ed0-122">Return Type</span></span>|<span data-ttu-id="d2ed0-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2ed0-123">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d2ed0-124">Listar deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="d2ed0-124">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="d2ed0-125">Coleção [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d2ed0-125">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="d2ed0-126">Lista propriedades e relações dos objetos [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="d2ed0-126">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="d2ed0-127">Obter deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d2ed0-127">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="d2ed0-128">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d2ed0-128">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="d2ed0-129">Propriedades de leitura e relações do objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="d2ed0-129">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="d2ed0-130">Criar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d2ed0-130">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="d2ed0-131">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d2ed0-131">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="d2ed0-132">Cria um novo objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="d2ed0-132">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="d2ed0-133">Excluir deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d2ed0-133">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="d2ed0-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d2ed0-134">None</span></span>|<span data-ttu-id="d2ed0-135">Exclui um [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="d2ed0-135">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="d2ed0-136">Atualizar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d2ed0-136">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="d2ed0-137">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d2ed0-137">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="d2ed0-138">Atualiza as propriedades de um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="d2ed0-138">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d2ed0-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2ed0-139">Properties</span></span>
|<span data-ttu-id="d2ed0-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2ed0-140">Property</span></span>|<span data-ttu-id="d2ed0-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2ed0-141">Type</span></span>|<span data-ttu-id="d2ed0-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2ed0-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2ed0-143">id</span><span class="sxs-lookup"><span data-stu-id="d2ed0-143">id</span></span>|<span data-ttu-id="d2ed0-144">String</span><span class="sxs-lookup"><span data-stu-id="d2ed0-144">String</span></span>|<span data-ttu-id="d2ed0-145">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d2ed0-145">Key of the entity.</span></span> <span data-ttu-id="d2ed0-146">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="d2ed0-146">This is read-only and automatically generated.</span></span> <span data-ttu-id="d2ed0-147">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d2ed0-147">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="d2ed0-148">displayName</span><span class="sxs-lookup"><span data-stu-id="d2ed0-148">displayName</span></span>|<span data-ttu-id="d2ed0-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2ed0-149">String</span></span>|<span data-ttu-id="d2ed0-150">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="d2ed0-150">Display Name of the Role definition.</span></span> <span data-ttu-id="d2ed0-151">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d2ed0-151">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="d2ed0-152">description</span><span class="sxs-lookup"><span data-stu-id="d2ed0-152">description</span></span>|<span data-ttu-id="d2ed0-153">String</span><span class="sxs-lookup"><span data-stu-id="d2ed0-153">String</span></span>|<span data-ttu-id="d2ed0-154">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="d2ed0-154">Description of the Role definition.</span></span> <span data-ttu-id="d2ed0-155">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d2ed0-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="d2ed0-156">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="d2ed0-156">rolePermissions</span></span>|<span data-ttu-id="d2ed0-157">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="d2ed0-157">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="d2ed0-158">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="d2ed0-158">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="d2ed0-159">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="d2ed0-159">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="d2ed0-160">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d2ed0-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="d2ed0-161">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="d2ed0-161">isBuiltIn</span></span>|<span data-ttu-id="d2ed0-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="d2ed0-162">Boolean</span></span>|<span data-ttu-id="d2ed0-163">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="d2ed0-163">Type of Role.</span></span> <span data-ttu-id="d2ed0-164">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="d2ed0-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="d2ed0-165">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d2ed0-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2ed0-166">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="d2ed0-166">Relationships</span></span>
|<span data-ttu-id="d2ed0-167">Relação</span><span class="sxs-lookup"><span data-stu-id="d2ed0-167">Relationship</span></span>|<span data-ttu-id="d2ed0-168">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2ed0-168">Type</span></span>|<span data-ttu-id="d2ed0-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2ed0-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2ed0-170">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="d2ed0-170">roleAssignments</span></span>|<span data-ttu-id="d2ed0-171">Coleção [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d2ed0-171">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="d2ed0-172">Lista de atribuições de função para esta definição de função.</span><span class="sxs-lookup"><span data-stu-id="d2ed0-172">List of Role assignments for this role definition.</span></span> <span data-ttu-id="d2ed0-173">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d2ed0-173">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d2ed0-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2ed0-174">JSON Representation</span></span>
<span data-ttu-id="d2ed0-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d2ed0-175">Here is a JSON representation of the resource.</span></span>
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
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
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
  "isBuiltIn": true
}
```







