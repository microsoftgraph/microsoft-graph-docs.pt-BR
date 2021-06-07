---
title: Tipo de recurso roleDefinition
description: 'O recurso de Definição de Função. A definição da função é a base do acesso baseado em função no Intune. A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso. Existem dois tipos de funções: internas e personalizadas. Funções internas não podem ser modificadas. Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas. Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.'
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ff5403f7741191021d45aeb6dfb87b2a299f4b85
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751185"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="a14c6-109">Tipo de recurso roleDefinition</span><span class="sxs-lookup"><span data-stu-id="a14c6-109">roleDefinition resource type</span></span>

<span data-ttu-id="a14c6-110">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a14c6-110">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a14c6-111">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a14c6-111">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a14c6-112">O recurso de Definição de Função.</span><span class="sxs-lookup"><span data-stu-id="a14c6-112">The Role Definition resource.</span></span> <span data-ttu-id="a14c6-113">A definição da função é a base do acesso baseado em função no Intune.</span><span class="sxs-lookup"><span data-stu-id="a14c6-113">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="a14c6-114">A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso.</span><span class="sxs-lookup"><span data-stu-id="a14c6-114">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="a14c6-115">Existem dois tipos de funções: internas e personalizadas.</span><span class="sxs-lookup"><span data-stu-id="a14c6-115">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="a14c6-116">Funções internas não podem ser modificadas.</span><span class="sxs-lookup"><span data-stu-id="a14c6-116">Built-in roles cannot be modified.</span></span> <span data-ttu-id="a14c6-117">Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas.</span><span class="sxs-lookup"><span data-stu-id="a14c6-117">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="a14c6-118">Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.</span><span class="sxs-lookup"><span data-stu-id="a14c6-118">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

## <a name="methods"></a><span data-ttu-id="a14c6-119">Methods</span><span class="sxs-lookup"><span data-stu-id="a14c6-119">Methods</span></span>
|<span data-ttu-id="a14c6-120">Método</span><span class="sxs-lookup"><span data-stu-id="a14c6-120">Method</span></span>|<span data-ttu-id="a14c6-121">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a14c6-121">Return Type</span></span>|<span data-ttu-id="a14c6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a14c6-122">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a14c6-123">Listar roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="a14c6-123">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="a14c6-124">Coleção [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a14c6-124">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="a14c6-125">Listar propriedades e relações dos objetos [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a14c6-125">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="a14c6-126">Obter roleDefinition</span><span class="sxs-lookup"><span data-stu-id="a14c6-126">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|[<span data-ttu-id="a14c6-127">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="a14c6-127">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="a14c6-128">Ler propriedades e relações do objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a14c6-128">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="a14c6-129">Criar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="a14c6-129">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|[<span data-ttu-id="a14c6-130">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="a14c6-130">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="a14c6-131">Criar um novo objeto [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a14c6-131">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="a14c6-132">Excluir roleDefinition</span><span class="sxs-lookup"><span data-stu-id="a14c6-132">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="a14c6-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a14c6-133">None</span></span>|<span data-ttu-id="a14c6-134">Excluir um [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a14c6-134">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="a14c6-135">Atualizar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="a14c6-135">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="a14c6-136">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="a14c6-136">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="a14c6-137">Atualizar as propriedades de um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a14c6-137">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a14c6-138">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a14c6-138">Properties</span></span>
|<span data-ttu-id="a14c6-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a14c6-139">Property</span></span>|<span data-ttu-id="a14c6-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="a14c6-140">Type</span></span>|<span data-ttu-id="a14c6-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="a14c6-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a14c6-142">id</span><span class="sxs-lookup"><span data-stu-id="a14c6-142">id</span></span>|<span data-ttu-id="a14c6-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a14c6-143">String</span></span>|<span data-ttu-id="a14c6-144">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a14c6-144">Key of the entity.</span></span> <span data-ttu-id="a14c6-145">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="a14c6-145">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="a14c6-146">displayName</span><span class="sxs-lookup"><span data-stu-id="a14c6-146">displayName</span></span>|<span data-ttu-id="a14c6-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a14c6-147">String</span></span>|<span data-ttu-id="a14c6-148">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="a14c6-148">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="a14c6-149">descrição</span><span class="sxs-lookup"><span data-stu-id="a14c6-149">description</span></span>|<span data-ttu-id="a14c6-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a14c6-150">String</span></span>|<span data-ttu-id="a14c6-151">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="a14c6-151">Description of the Role definition.</span></span>|
|<span data-ttu-id="a14c6-152">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="a14c6-152">rolePermissions</span></span>|<span data-ttu-id="a14c6-153">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="a14c6-153">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="a14c6-154">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="a14c6-154">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="a14c6-155">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="a14c6-155">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="a14c6-156">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="a14c6-156">isBuiltIn</span></span>|<span data-ttu-id="a14c6-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="a14c6-157">Boolean</span></span>|<span data-ttu-id="a14c6-158">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="a14c6-158">Type of Role.</span></span> <span data-ttu-id="a14c6-159">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="a14c6-159">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a14c6-160">Relações</span><span class="sxs-lookup"><span data-stu-id="a14c6-160">Relationships</span></span>
|<span data-ttu-id="a14c6-161">Relação</span><span class="sxs-lookup"><span data-stu-id="a14c6-161">Relationship</span></span>|<span data-ttu-id="a14c6-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="a14c6-162">Type</span></span>|<span data-ttu-id="a14c6-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="a14c6-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a14c6-164">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="a14c6-164">roleAssignments</span></span>|<span data-ttu-id="a14c6-165">Coleção [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a14c6-165">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="a14c6-166">Lista de atribuições de função para esta definição de função.</span><span class="sxs-lookup"><span data-stu-id="a14c6-166">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a14c6-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a14c6-167">JSON Representation</span></span>
<span data-ttu-id="a14c6-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a14c6-168">Here is a JSON representation of the resource.</span></span>
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




