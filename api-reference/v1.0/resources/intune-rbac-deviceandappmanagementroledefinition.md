---
title: Tipo de recurso deviceAndAppManagementRoleDefinition
description: 'O recurso de Definição de Função. A definição da função é a base do acesso baseado em função no Intune. A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso. Existem dois tipos de funções: internas e personalizadas. Funções internas não podem ser modificadas. Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas. Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.'
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8b3241a8cdd909f6e267b5016167c89aaa6fb7b3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447952"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="f0b97-109">Tipo de recurso deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="f0b97-109">deviceAndAppManagementRoleDefinition resource type</span></span>

<span data-ttu-id="f0b97-110">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f0b97-110">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0b97-111">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f0b97-111">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0b97-112">O recurso de Definição de Função.</span><span class="sxs-lookup"><span data-stu-id="f0b97-112">The Role Definition resource.</span></span> <span data-ttu-id="f0b97-113">A definição da função é a base do acesso baseado em função no Intune.</span><span class="sxs-lookup"><span data-stu-id="f0b97-113">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="f0b97-114">A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso.</span><span class="sxs-lookup"><span data-stu-id="f0b97-114">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="f0b97-115">Existem dois tipos de funções: internas e personalizadas.</span><span class="sxs-lookup"><span data-stu-id="f0b97-115">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="f0b97-116">Funções internas não podem ser modificadas.</span><span class="sxs-lookup"><span data-stu-id="f0b97-116">Built-in roles cannot be modified.</span></span> <span data-ttu-id="f0b97-117">Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas.</span><span class="sxs-lookup"><span data-stu-id="f0b97-117">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="f0b97-118">Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.</span><span class="sxs-lookup"><span data-stu-id="f0b97-118">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>


<span data-ttu-id="f0b97-119">Herda de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f0b97-119">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="f0b97-120">Métodos</span><span class="sxs-lookup"><span data-stu-id="f0b97-120">Methods</span></span>
|<span data-ttu-id="f0b97-121">Método</span><span class="sxs-lookup"><span data-stu-id="f0b97-121">Method</span></span>|<span data-ttu-id="f0b97-122">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f0b97-122">Return Type</span></span>|<span data-ttu-id="f0b97-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0b97-123">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f0b97-124">Listar deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="f0b97-124">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="f0b97-125">Coleção [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f0b97-125">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="f0b97-126">Lista propriedades e relações dos objetos [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f0b97-126">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="f0b97-127">Obter deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="f0b97-127">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="f0b97-128">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="f0b97-128">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="f0b97-129">Propriedades de leitura e relações do objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f0b97-129">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="f0b97-130">Criar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="f0b97-130">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="f0b97-131">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="f0b97-131">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="f0b97-132">Cria um novo objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f0b97-132">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="f0b97-133">Excluir deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="f0b97-133">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="f0b97-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f0b97-134">None</span></span>|<span data-ttu-id="f0b97-135">Exclui um [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f0b97-135">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="f0b97-136">Atualizar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="f0b97-136">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="f0b97-137">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="f0b97-137">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="f0b97-138">Atualiza as propriedades de um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f0b97-138">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f0b97-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0b97-139">Properties</span></span>
|<span data-ttu-id="f0b97-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0b97-140">Property</span></span>|<span data-ttu-id="f0b97-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0b97-141">Type</span></span>|<span data-ttu-id="f0b97-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0b97-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0b97-143">id</span><span class="sxs-lookup"><span data-stu-id="f0b97-143">id</span></span>|<span data-ttu-id="f0b97-144">String</span><span class="sxs-lookup"><span data-stu-id="f0b97-144">String</span></span>|<span data-ttu-id="f0b97-145">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f0b97-145">Key of the entity.</span></span> <span data-ttu-id="f0b97-146">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="f0b97-146">This is read-only and automatically generated.</span></span> <span data-ttu-id="f0b97-147">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f0b97-147">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="f0b97-148">displayName</span><span class="sxs-lookup"><span data-stu-id="f0b97-148">displayName</span></span>|<span data-ttu-id="f0b97-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0b97-149">String</span></span>|<span data-ttu-id="f0b97-150">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="f0b97-150">Display Name of the Role definition.</span></span> <span data-ttu-id="f0b97-151">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f0b97-151">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="f0b97-152">description</span><span class="sxs-lookup"><span data-stu-id="f0b97-152">description</span></span>|<span data-ttu-id="f0b97-153">String</span><span class="sxs-lookup"><span data-stu-id="f0b97-153">String</span></span>|<span data-ttu-id="f0b97-154">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="f0b97-154">Description of the Role definition.</span></span> <span data-ttu-id="f0b97-155">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f0b97-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="f0b97-156">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="f0b97-156">rolePermissions</span></span>|<span data-ttu-id="f0b97-157">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="f0b97-157">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="f0b97-158">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="f0b97-158">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="f0b97-159">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="f0b97-159">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="f0b97-160">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f0b97-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="f0b97-161">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="f0b97-161">isBuiltIn</span></span>|<span data-ttu-id="f0b97-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="f0b97-162">Boolean</span></span>|<span data-ttu-id="f0b97-163">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="f0b97-163">Type of Role.</span></span> <span data-ttu-id="f0b97-164">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="f0b97-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="f0b97-165">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f0b97-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0b97-166">Relações</span><span class="sxs-lookup"><span data-stu-id="f0b97-166">Relationships</span></span>
|<span data-ttu-id="f0b97-167">Relação</span><span class="sxs-lookup"><span data-stu-id="f0b97-167">Relationship</span></span>|<span data-ttu-id="f0b97-168">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0b97-168">Type</span></span>|<span data-ttu-id="f0b97-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0b97-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0b97-170">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="f0b97-170">roleAssignments</span></span>|<span data-ttu-id="f0b97-171">Coleção [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f0b97-171">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="f0b97-172">Lista de atribuições de função para esta definição de função.</span><span class="sxs-lookup"><span data-stu-id="f0b97-172">List of Role assignments for this role definition.</span></span> <span data-ttu-id="f0b97-173">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f0b97-173">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0b97-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0b97-174">JSON Representation</span></span>
<span data-ttu-id="f0b97-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f0b97-175">Here is a JSON representation of the resource.</span></span>
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




