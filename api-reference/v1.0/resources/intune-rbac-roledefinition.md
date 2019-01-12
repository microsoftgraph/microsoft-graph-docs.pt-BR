---
title: Tipo de recurso roleDefinition
description: 'O recurso de Definição de Função. A definição da função é a base do acesso baseado em função no Intune. A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso. Existem dois tipos de funções: internas e personalizadas. Funções internas não podem ser modificadas. Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas. Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.'
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: f09b94649f30909c2efc2d9851503b5b8db14127
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971869"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="1b501-109">Tipo de recurso roleDefinition</span><span class="sxs-lookup"><span data-stu-id="1b501-109">roleDefinition resource type</span></span>

> <span data-ttu-id="1b501-110">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1b501-110">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b501-111">O recurso de Definição de Função.</span><span class="sxs-lookup"><span data-stu-id="1b501-111">The Role Definition resource.</span></span> <span data-ttu-id="1b501-112">A definição da função é a base do acesso baseado em função no Intune.</span><span class="sxs-lookup"><span data-stu-id="1b501-112">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="1b501-113">A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso.</span><span class="sxs-lookup"><span data-stu-id="1b501-113">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="1b501-114">Existem dois tipos de funções: internas e personalizadas.</span><span class="sxs-lookup"><span data-stu-id="1b501-114">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="1b501-115">Funções internas não podem ser modificadas.</span><span class="sxs-lookup"><span data-stu-id="1b501-115">Built-in roles cannot be modified.</span></span> <span data-ttu-id="1b501-116">Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas.</span><span class="sxs-lookup"><span data-stu-id="1b501-116">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="1b501-117">Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.</span><span class="sxs-lookup"><span data-stu-id="1b501-117">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>
## <a name="methods"></a><span data-ttu-id="1b501-118">Métodos</span><span class="sxs-lookup"><span data-stu-id="1b501-118">Methods</span></span>
|<span data-ttu-id="1b501-119">Método</span><span class="sxs-lookup"><span data-stu-id="1b501-119">Method</span></span>|<span data-ttu-id="1b501-120">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1b501-120">Return Type</span></span>|<span data-ttu-id="1b501-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b501-121">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1b501-122">Listar roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="1b501-122">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="1b501-123">Coleção [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1b501-123">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="1b501-124">Listar propriedades e relações dos objetos [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="1b501-124">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="1b501-125">Obter roleDefinition</span><span class="sxs-lookup"><span data-stu-id="1b501-125">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|[<span data-ttu-id="1b501-126">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="1b501-126">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="1b501-127">Ler propriedades e relações do objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="1b501-127">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="1b501-128">Criar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="1b501-128">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|[<span data-ttu-id="1b501-129">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="1b501-129">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="1b501-130">Criar um novo objeto [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1b501-130">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="1b501-131">Excluir roleDefinition</span><span class="sxs-lookup"><span data-stu-id="1b501-131">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="1b501-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1b501-132">None</span></span>|<span data-ttu-id="1b501-133">Excluir um [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1b501-133">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="1b501-134">Atualizar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="1b501-134">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="1b501-135">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="1b501-135">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="1b501-136">Atualizar as propriedades de um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="1b501-136">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1b501-137">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b501-137">Properties</span></span>
|<span data-ttu-id="1b501-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b501-138">Property</span></span>|<span data-ttu-id="1b501-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b501-139">Type</span></span>|<span data-ttu-id="1b501-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b501-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b501-141">id</span><span class="sxs-lookup"><span data-stu-id="1b501-141">id</span></span>|<span data-ttu-id="1b501-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b501-142">String</span></span>|<span data-ttu-id="1b501-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1b501-143">Key of the entity.</span></span> <span data-ttu-id="1b501-144">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="1b501-144">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="1b501-145">displayName</span><span class="sxs-lookup"><span data-stu-id="1b501-145">displayName</span></span>|<span data-ttu-id="1b501-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b501-146">String</span></span>|<span data-ttu-id="1b501-147">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="1b501-147">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="1b501-148">description</span><span class="sxs-lookup"><span data-stu-id="1b501-148">description</span></span>|<span data-ttu-id="1b501-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b501-149">String</span></span>|<span data-ttu-id="1b501-150">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="1b501-150">Description of the Role definition.</span></span>|
|<span data-ttu-id="1b501-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="1b501-151">rolePermissions</span></span>|<span data-ttu-id="1b501-152">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="1b501-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="1b501-153">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="1b501-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="1b501-154">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="1b501-154">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="1b501-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="1b501-155">isBuiltIn</span></span>|<span data-ttu-id="1b501-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="1b501-156">Boolean</span></span>|<span data-ttu-id="1b501-157">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="1b501-157">Type of Role.</span></span> <span data-ttu-id="1b501-158">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="1b501-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b501-159">Relações</span><span class="sxs-lookup"><span data-stu-id="1b501-159">Relationships</span></span>
|<span data-ttu-id="1b501-160">Relação</span><span class="sxs-lookup"><span data-stu-id="1b501-160">Relationship</span></span>|<span data-ttu-id="1b501-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b501-161">Type</span></span>|<span data-ttu-id="1b501-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b501-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b501-163">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="1b501-163">roleAssignments</span></span>|<span data-ttu-id="1b501-164">Coleção [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1b501-164">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="1b501-165">Lista de atribuições de função para esta definição de função.</span><span class="sxs-lookup"><span data-stu-id="1b501-165">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1b501-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1b501-166">JSON Representation</span></span>
<span data-ttu-id="1b501-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1b501-167">Here is a JSON representation of the resource.</span></span>
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



