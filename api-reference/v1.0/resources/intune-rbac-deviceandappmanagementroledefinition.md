---
title: Tipo de recurso deviceAndAppManagementRoleDefinition
description: 'O recurso de Definição de Função. A definição da função é a base do acesso baseado em função no Intune. A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso. Existem dois tipos de funções: internas e personalizadas. Funções internas não podem ser modificadas. Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas. Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.'
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4a1334686fc694cf968aa1319920649fdbc56347
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037784"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="2f57a-109">Tipo de recurso deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="2f57a-109">deviceAndAppManagementRoleDefinition resource type</span></span>

<span data-ttu-id="2f57a-110">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f57a-110">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f57a-111">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f57a-111">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f57a-112">O recurso de Definição de Função.</span><span class="sxs-lookup"><span data-stu-id="2f57a-112">The Role Definition resource.</span></span> <span data-ttu-id="2f57a-113">A definição da função é a base do acesso baseado em função no Intune.</span><span class="sxs-lookup"><span data-stu-id="2f57a-113">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="2f57a-114">A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso.</span><span class="sxs-lookup"><span data-stu-id="2f57a-114">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="2f57a-115">Existem dois tipos de funções: internas e personalizadas.</span><span class="sxs-lookup"><span data-stu-id="2f57a-115">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="2f57a-116">Funções internas não podem ser modificadas.</span><span class="sxs-lookup"><span data-stu-id="2f57a-116">Built-in roles cannot be modified.</span></span> <span data-ttu-id="2f57a-117">Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas.</span><span class="sxs-lookup"><span data-stu-id="2f57a-117">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="2f57a-118">Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.</span><span class="sxs-lookup"><span data-stu-id="2f57a-118">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>


<span data-ttu-id="2f57a-119">Herda de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2f57a-119">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="2f57a-120">Methods</span><span class="sxs-lookup"><span data-stu-id="2f57a-120">Methods</span></span>
|<span data-ttu-id="2f57a-121">Método</span><span class="sxs-lookup"><span data-stu-id="2f57a-121">Method</span></span>|<span data-ttu-id="2f57a-122">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2f57a-122">Return Type</span></span>|<span data-ttu-id="2f57a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f57a-123">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2f57a-124">Listar deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="2f57a-124">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="2f57a-125">Coleção [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2f57a-125">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="2f57a-126">Lista propriedades e relações dos objetos [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="2f57a-126">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="2f57a-127">Obter deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="2f57a-127">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="2f57a-128">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="2f57a-128">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="2f57a-129">Propriedades de leitura e relações do objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="2f57a-129">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="2f57a-130">Criar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="2f57a-130">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="2f57a-131">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="2f57a-131">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="2f57a-132">Cria um novo objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="2f57a-132">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="2f57a-133">Excluir deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="2f57a-133">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="2f57a-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2f57a-134">None</span></span>|<span data-ttu-id="2f57a-135">Exclui um [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="2f57a-135">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="2f57a-136">Atualizar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="2f57a-136">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="2f57a-137">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="2f57a-137">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="2f57a-138">Atualiza as propriedades de um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="2f57a-138">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2f57a-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2f57a-139">Properties</span></span>
|<span data-ttu-id="2f57a-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f57a-140">Property</span></span>|<span data-ttu-id="2f57a-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f57a-141">Type</span></span>|<span data-ttu-id="2f57a-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f57a-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f57a-143">id</span><span class="sxs-lookup"><span data-stu-id="2f57a-143">id</span></span>|<span data-ttu-id="2f57a-144">String</span><span class="sxs-lookup"><span data-stu-id="2f57a-144">String</span></span>|<span data-ttu-id="2f57a-145">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2f57a-145">Key of the entity.</span></span> <span data-ttu-id="2f57a-146">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="2f57a-146">This is read-only and automatically generated.</span></span> <span data-ttu-id="2f57a-147">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2f57a-147">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="2f57a-148">displayName</span><span class="sxs-lookup"><span data-stu-id="2f57a-148">displayName</span></span>|<span data-ttu-id="2f57a-149">String</span><span class="sxs-lookup"><span data-stu-id="2f57a-149">String</span></span>|<span data-ttu-id="2f57a-150">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="2f57a-150">Display Name of the Role definition.</span></span> <span data-ttu-id="2f57a-151">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2f57a-151">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="2f57a-152">description</span><span class="sxs-lookup"><span data-stu-id="2f57a-152">description</span></span>|<span data-ttu-id="2f57a-153">String</span><span class="sxs-lookup"><span data-stu-id="2f57a-153">String</span></span>|<span data-ttu-id="2f57a-154">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="2f57a-154">Description of the Role definition.</span></span> <span data-ttu-id="2f57a-155">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2f57a-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="2f57a-156">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="2f57a-156">rolePermissions</span></span>|<span data-ttu-id="2f57a-157">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="2f57a-157">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="2f57a-158">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="2f57a-158">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="2f57a-159">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="2f57a-159">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="2f57a-160">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2f57a-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="2f57a-161">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="2f57a-161">isBuiltIn</span></span>|<span data-ttu-id="2f57a-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f57a-162">Boolean</span></span>|<span data-ttu-id="2f57a-163">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="2f57a-163">Type of Role.</span></span> <span data-ttu-id="2f57a-164">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="2f57a-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="2f57a-165">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2f57a-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f57a-166">Relações</span><span class="sxs-lookup"><span data-stu-id="2f57a-166">Relationships</span></span>
|<span data-ttu-id="2f57a-167">Relação</span><span class="sxs-lookup"><span data-stu-id="2f57a-167">Relationship</span></span>|<span data-ttu-id="2f57a-168">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f57a-168">Type</span></span>|<span data-ttu-id="2f57a-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f57a-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f57a-170">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="2f57a-170">roleAssignments</span></span>|<span data-ttu-id="2f57a-171">Coleção [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2f57a-171">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="2f57a-172">Lista de atribuições de função para esta definição de função.</span><span class="sxs-lookup"><span data-stu-id="2f57a-172">List of Role assignments for this role definition.</span></span> <span data-ttu-id="2f57a-173">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2f57a-173">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2f57a-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2f57a-174">JSON Representation</span></span>
<span data-ttu-id="2f57a-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2f57a-175">Here is a JSON representation of the resource.</span></span>
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









