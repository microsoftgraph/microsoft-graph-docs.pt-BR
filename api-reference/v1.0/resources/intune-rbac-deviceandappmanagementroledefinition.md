---
title: Tipo de recurso deviceAndAppManagementRoleDefinition
description: 'O recurso de Definição de Função. A definição da função é a base do acesso baseado em função no Intune. A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso. Existem dois tipos de funções: internas e personalizadas. Funções internas não podem ser modificadas. Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas. Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.'
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e703909f818535eac7ae00284d15620bce55ba80
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253425"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="45a7e-109">Tipo de recurso deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="45a7e-109">deviceAndAppManagementRoleDefinition resource type</span></span>

> <span data-ttu-id="45a7e-110">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45a7e-110">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45a7e-111">O recurso de Definição de Função.</span><span class="sxs-lookup"><span data-stu-id="45a7e-111">The Role Definition resource.</span></span> <span data-ttu-id="45a7e-112">A definição da função é a base do acesso baseado em função no Intune.</span><span class="sxs-lookup"><span data-stu-id="45a7e-112">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="45a7e-113">A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso.</span><span class="sxs-lookup"><span data-stu-id="45a7e-113">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="45a7e-114">Existem dois tipos de funções: internas e personalizadas.</span><span class="sxs-lookup"><span data-stu-id="45a7e-114">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="45a7e-115">Funções internas não podem ser modificadas.</span><span class="sxs-lookup"><span data-stu-id="45a7e-115">Built-in roles cannot be modified.</span></span> <span data-ttu-id="45a7e-116">Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas.</span><span class="sxs-lookup"><span data-stu-id="45a7e-116">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="45a7e-117">Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.</span><span class="sxs-lookup"><span data-stu-id="45a7e-117">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>


<span data-ttu-id="45a7e-118">Herda de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="45a7e-118">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="45a7e-119">Métodos</span><span class="sxs-lookup"><span data-stu-id="45a7e-119">Methods</span></span>
|<span data-ttu-id="45a7e-120">Método</span><span class="sxs-lookup"><span data-stu-id="45a7e-120">Method</span></span>|<span data-ttu-id="45a7e-121">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="45a7e-121">Return Type</span></span>|<span data-ttu-id="45a7e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="45a7e-122">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="45a7e-123">Listar deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="45a7e-123">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="45a7e-124">Coleção [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="45a7e-124">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="45a7e-125">Lista propriedades e relações dos objetos [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="45a7e-125">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="45a7e-126">Obter deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="45a7e-126">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="45a7e-127">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="45a7e-127">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="45a7e-128">Propriedades de leitura e relações do objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="45a7e-128">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="45a7e-129">Criar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="45a7e-129">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="45a7e-130">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="45a7e-130">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="45a7e-131">Cria um novo objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="45a7e-131">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="45a7e-132">Excluir deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="45a7e-132">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="45a7e-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="45a7e-133">None</span></span>|<span data-ttu-id="45a7e-134">Exclui um [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="45a7e-134">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="45a7e-135">Atualizar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="45a7e-135">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="45a7e-136">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="45a7e-136">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="45a7e-137">Atualiza as propriedades de um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="45a7e-137">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="45a7e-138">Propriedades</span><span class="sxs-lookup"><span data-stu-id="45a7e-138">Properties</span></span>
|<span data-ttu-id="45a7e-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45a7e-139">Property</span></span>|<span data-ttu-id="45a7e-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="45a7e-140">Type</span></span>|<span data-ttu-id="45a7e-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="45a7e-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45a7e-142">id</span><span class="sxs-lookup"><span data-stu-id="45a7e-142">id</span></span>|<span data-ttu-id="45a7e-143">String</span><span class="sxs-lookup"><span data-stu-id="45a7e-143">String</span></span>|<span data-ttu-id="45a7e-144">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="45a7e-144">Key of the entity.</span></span> <span data-ttu-id="45a7e-145">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="45a7e-145">This is read-only and automatically generated.</span></span> <span data-ttu-id="45a7e-146">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="45a7e-146">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="45a7e-147">displayName</span><span class="sxs-lookup"><span data-stu-id="45a7e-147">displayName</span></span>|<span data-ttu-id="45a7e-148">String</span><span class="sxs-lookup"><span data-stu-id="45a7e-148">String</span></span>|<span data-ttu-id="45a7e-149">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="45a7e-149">Display Name of the Role definition.</span></span> <span data-ttu-id="45a7e-150">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="45a7e-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="45a7e-151">description</span><span class="sxs-lookup"><span data-stu-id="45a7e-151">description</span></span>|<span data-ttu-id="45a7e-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45a7e-152">String</span></span>|<span data-ttu-id="45a7e-153">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="45a7e-153">Description of the Role definition.</span></span> <span data-ttu-id="45a7e-154">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="45a7e-154">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="45a7e-155">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="45a7e-155">rolePermissions</span></span>|<span data-ttu-id="45a7e-156">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="45a7e-156">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="45a7e-157">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="45a7e-157">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="45a7e-158">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="45a7e-158">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="45a7e-159">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="45a7e-159">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="45a7e-160">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="45a7e-160">isBuiltIn</span></span>|<span data-ttu-id="45a7e-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="45a7e-161">Boolean</span></span>|<span data-ttu-id="45a7e-162">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="45a7e-162">Type of Role.</span></span> <span data-ttu-id="45a7e-163">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="45a7e-163">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="45a7e-164">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="45a7e-164">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="45a7e-165">Relações</span><span class="sxs-lookup"><span data-stu-id="45a7e-165">Relationships</span></span>
|<span data-ttu-id="45a7e-166">Relação</span><span class="sxs-lookup"><span data-stu-id="45a7e-166">Relationship</span></span>|<span data-ttu-id="45a7e-167">Tipo</span><span class="sxs-lookup"><span data-stu-id="45a7e-167">Type</span></span>|<span data-ttu-id="45a7e-168">Descrição</span><span class="sxs-lookup"><span data-stu-id="45a7e-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45a7e-169">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="45a7e-169">roleAssignments</span></span>|<span data-ttu-id="45a7e-170">Coleção [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="45a7e-170">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="45a7e-171">Lista de atribuições de função para esta definição de função.</span><span class="sxs-lookup"><span data-stu-id="45a7e-171">List of Role assignments for this role definition.</span></span> <span data-ttu-id="45a7e-172">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="45a7e-172">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="45a7e-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="45a7e-173">JSON Representation</span></span>
<span data-ttu-id="45a7e-174">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="45a7e-174">Here is a JSON representation of the resource.</span></span>
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



