---
title: Tipo de recurso deviceAndAppManagementRoleAssignment
description: O recurso de Atribuição de Função. Atribuições de função unem uma definição de função a membros e escopos. Pode haver uma ou mais atribuições de função por função. Aplica-se às funções internas e personalizadas
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bfbb4e3b51f56e447ba69caefbf2b0b5226a5d4f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567484"
---
# <a name="deviceandappmanagementroleassignment-resource-type"></a><span data-ttu-id="71d94-106">Tipo de recurso deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="71d94-106">deviceAndAppManagementRoleAssignment resource type</span></span>

> <span data-ttu-id="71d94-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="71d94-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71d94-108">O recurso de Atribuição de Função.</span><span class="sxs-lookup"><span data-stu-id="71d94-108">The Role Assignment resource.</span></span> <span data-ttu-id="71d94-109">Atribuições de função unem uma definição de função a membros e escopos.</span><span class="sxs-lookup"><span data-stu-id="71d94-109">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="71d94-110">Pode haver uma ou mais atribuições de função por função.</span><span class="sxs-lookup"><span data-stu-id="71d94-110">There can be one or more role assignments per role.</span></span> <span data-ttu-id="71d94-111">Aplica-se às funções internas e personalizadas.</span><span class="sxs-lookup"><span data-stu-id="71d94-111">This applies to custom and built-in roles.</span></span>


<span data-ttu-id="71d94-112">Herda de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="71d94-112">Inherits from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>

## <a name="methods"></a><span data-ttu-id="71d94-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="71d94-113">Methods</span></span>
|<span data-ttu-id="71d94-114">Método</span><span class="sxs-lookup"><span data-stu-id="71d94-114">Method</span></span>|<span data-ttu-id="71d94-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="71d94-115">Return Type</span></span>|<span data-ttu-id="71d94-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="71d94-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="71d94-117">Listar deviceAndAppManagementRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="71d94-117">List deviceAndAppManagementRoleAssignments</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-list.md)|<span data-ttu-id="71d94-118">Coleção [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="71d94-118">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) collection</span></span>|<span data-ttu-id="71d94-119">Lista propriedades e relações dos objetos [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="71d94-119">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>|
|[<span data-ttu-id="71d94-120">Obter deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="71d94-120">Get deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-get.md)|[<span data-ttu-id="71d94-121">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="71d94-121">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="71d94-122">Propriedades de leitura e relações do objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="71d94-122">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="71d94-123">Criar deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="71d94-123">Create deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-create.md)|[<span data-ttu-id="71d94-124">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="71d94-124">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="71d94-125">Cria um novo objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="71d94-125">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="71d94-126">Excluir deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="71d94-126">Delete deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-delete.md)|<span data-ttu-id="71d94-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="71d94-127">None</span></span>|<span data-ttu-id="71d94-128">Exclui um [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="71d94-128">Deletes a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>|
|[<span data-ttu-id="71d94-129">Atualizar deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="71d94-129">Update deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-update.md)|[<span data-ttu-id="71d94-130">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="71d94-130">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="71d94-131">Atualiza as propriedades de um objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="71d94-131">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="71d94-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71d94-132">Properties</span></span>
|<span data-ttu-id="71d94-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71d94-133">Property</span></span>|<span data-ttu-id="71d94-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="71d94-134">Type</span></span>|<span data-ttu-id="71d94-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="71d94-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71d94-136">id</span><span class="sxs-lookup"><span data-stu-id="71d94-136">id</span></span>|<span data-ttu-id="71d94-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71d94-137">String</span></span>|<span data-ttu-id="71d94-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="71d94-138">Key of the entity.</span></span> <span data-ttu-id="71d94-139">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="71d94-139">This is read-only and automatically generated.</span></span> <span data-ttu-id="71d94-140">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="71d94-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="71d94-141">displayName</span><span class="sxs-lookup"><span data-stu-id="71d94-141">displayName</span></span>|<span data-ttu-id="71d94-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71d94-142">String</span></span>|<span data-ttu-id="71d94-143">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="71d94-143">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="71d94-144">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="71d94-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="71d94-145">description</span><span class="sxs-lookup"><span data-stu-id="71d94-145">description</span></span>|<span data-ttu-id="71d94-146">String</span><span class="sxs-lookup"><span data-stu-id="71d94-146">String</span></span>|<span data-ttu-id="71d94-147">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="71d94-147">Description of the Role Assignment.</span></span> <span data-ttu-id="71d94-148">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="71d94-148">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="71d94-149">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="71d94-149">resourceScopes</span></span>|<span data-ttu-id="71d94-150">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71d94-150">String collection</span></span>|<span data-ttu-id="71d94-151">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="71d94-151">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="71d94-152">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="71d94-152">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="71d94-153">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="71d94-153">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="71d94-154">members</span><span class="sxs-lookup"><span data-stu-id="71d94-154">members</span></span>|<span data-ttu-id="71d94-155">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="71d94-155">String collection</span></span>|<span data-ttu-id="71d94-156">A lista de IDs de grupos de segurança de membros da função.</span><span class="sxs-lookup"><span data-stu-id="71d94-156">The list of ids of role member security groups.</span></span> <span data-ttu-id="71d94-157">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="71d94-157">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71d94-158">Relações</span><span class="sxs-lookup"><span data-stu-id="71d94-158">Relationships</span></span>
|<span data-ttu-id="71d94-159">Relação</span><span class="sxs-lookup"><span data-stu-id="71d94-159">Relationship</span></span>|<span data-ttu-id="71d94-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="71d94-160">Type</span></span>|<span data-ttu-id="71d94-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="71d94-161">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71d94-162">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="71d94-162">roleDefinition</span></span>|[<span data-ttu-id="71d94-163">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="71d94-163">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="71d94-164">A definição de função da qual essa atribuição faz parte.</span><span class="sxs-lookup"><span data-stu-id="71d94-164">Role definition this assignment is part of.</span></span> <span data-ttu-id="71d94-165">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="71d94-165">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="71d94-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71d94-166">JSON Representation</span></span>
<span data-ttu-id="71d94-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="71d94-167">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "resourceScopes": [
    "String"
  ],
  "members": [
    "String"
  ]
}
```



