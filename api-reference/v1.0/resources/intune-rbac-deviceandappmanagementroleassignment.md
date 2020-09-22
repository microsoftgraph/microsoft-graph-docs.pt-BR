---
title: Tipo de recurso deviceAndAppManagementRoleAssignment
description: O recurso de Atribuição de Função. Atribuições de função unem uma definição de função a membros e escopos. Pode haver uma ou mais atribuições de função por função. Aplica-se às funções internas e personalizadas
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 866b7ce675bc3b6765100d730db300eabdd7f0fb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037812"
---
# <a name="deviceandappmanagementroleassignment-resource-type"></a><span data-ttu-id="6192a-106">Tipo de recurso deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6192a-106">deviceAndAppManagementRoleAssignment resource type</span></span>

<span data-ttu-id="6192a-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6192a-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6192a-108">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6192a-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6192a-109">O recurso de Atribuição de Função.</span><span class="sxs-lookup"><span data-stu-id="6192a-109">The Role Assignment resource.</span></span> <span data-ttu-id="6192a-110">Atribuições de função unem uma definição de função a membros e escopos.</span><span class="sxs-lookup"><span data-stu-id="6192a-110">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="6192a-111">Pode haver uma ou mais atribuições de função por função.</span><span class="sxs-lookup"><span data-stu-id="6192a-111">There can be one or more role assignments per role.</span></span> <span data-ttu-id="6192a-112">Aplica-se às funções internas e personalizadas.</span><span class="sxs-lookup"><span data-stu-id="6192a-112">This applies to custom and built-in roles.</span></span>


<span data-ttu-id="6192a-113">Herda de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6192a-113">Inherits from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>

## <a name="methods"></a><span data-ttu-id="6192a-114">Methods</span><span class="sxs-lookup"><span data-stu-id="6192a-114">Methods</span></span>
|<span data-ttu-id="6192a-115">Método</span><span class="sxs-lookup"><span data-stu-id="6192a-115">Method</span></span>|<span data-ttu-id="6192a-116">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6192a-116">Return Type</span></span>|<span data-ttu-id="6192a-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="6192a-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6192a-118">Listar deviceAndAppManagementRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="6192a-118">List deviceAndAppManagementRoleAssignments</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-list.md)|<span data-ttu-id="6192a-119">Coleção [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6192a-119">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) collection</span></span>|<span data-ttu-id="6192a-120">Lista propriedades e relações dos objetos [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6192a-120">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>|
|[<span data-ttu-id="6192a-121">Obter deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6192a-121">Get deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-get.md)|[<span data-ttu-id="6192a-122">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6192a-122">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="6192a-123">Propriedades de leitura e relações do objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6192a-123">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="6192a-124">Criar deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6192a-124">Create deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-create.md)|[<span data-ttu-id="6192a-125">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6192a-125">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="6192a-126">Cria um novo objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6192a-126">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="6192a-127">Excluir deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6192a-127">Delete deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-delete.md)|<span data-ttu-id="6192a-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6192a-128">None</span></span>|<span data-ttu-id="6192a-129">Exclui um [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6192a-129">Deletes a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>|
|[<span data-ttu-id="6192a-130">Atualizar deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6192a-130">Update deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-update.md)|[<span data-ttu-id="6192a-131">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6192a-131">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="6192a-132">Atualiza as propriedades de um objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6192a-132">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6192a-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6192a-133">Properties</span></span>
|<span data-ttu-id="6192a-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6192a-134">Property</span></span>|<span data-ttu-id="6192a-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="6192a-135">Type</span></span>|<span data-ttu-id="6192a-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="6192a-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6192a-137">id</span><span class="sxs-lookup"><span data-stu-id="6192a-137">id</span></span>|<span data-ttu-id="6192a-138">String</span><span class="sxs-lookup"><span data-stu-id="6192a-138">String</span></span>|<span data-ttu-id="6192a-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6192a-139">Key of the entity.</span></span> <span data-ttu-id="6192a-140">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="6192a-140">This is read-only and automatically generated.</span></span> <span data-ttu-id="6192a-141">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6192a-141">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="6192a-142">displayName</span><span class="sxs-lookup"><span data-stu-id="6192a-142">displayName</span></span>|<span data-ttu-id="6192a-143">String</span><span class="sxs-lookup"><span data-stu-id="6192a-143">String</span></span>|<span data-ttu-id="6192a-144">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="6192a-144">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="6192a-145">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6192a-145">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="6192a-146">description</span><span class="sxs-lookup"><span data-stu-id="6192a-146">description</span></span>|<span data-ttu-id="6192a-147">String</span><span class="sxs-lookup"><span data-stu-id="6192a-147">String</span></span>|<span data-ttu-id="6192a-148">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="6192a-148">Description of the Role Assignment.</span></span> <span data-ttu-id="6192a-149">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6192a-149">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="6192a-150">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="6192a-150">resourceScopes</span></span>|<span data-ttu-id="6192a-151">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6192a-151">String collection</span></span>|<span data-ttu-id="6192a-152">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="6192a-152">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="6192a-153">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6192a-153">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="6192a-154">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6192a-154">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="6192a-155">members</span><span class="sxs-lookup"><span data-stu-id="6192a-155">members</span></span>|<span data-ttu-id="6192a-156">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6192a-156">String collection</span></span>|<span data-ttu-id="6192a-157">A lista de IDs de grupos de segurança de membros da função.</span><span class="sxs-lookup"><span data-stu-id="6192a-157">The list of ids of role member security groups.</span></span> <span data-ttu-id="6192a-158">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6192a-158">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6192a-159">Relações</span><span class="sxs-lookup"><span data-stu-id="6192a-159">Relationships</span></span>
|<span data-ttu-id="6192a-160">Relação</span><span class="sxs-lookup"><span data-stu-id="6192a-160">Relationship</span></span>|<span data-ttu-id="6192a-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="6192a-161">Type</span></span>|<span data-ttu-id="6192a-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="6192a-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6192a-163">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="6192a-163">roleDefinition</span></span>|[<span data-ttu-id="6192a-164">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="6192a-164">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="6192a-165">A definição de função da qual essa atribuição faz parte.</span><span class="sxs-lookup"><span data-stu-id="6192a-165">Role definition this assignment is part of.</span></span> <span data-ttu-id="6192a-166">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6192a-166">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6192a-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6192a-167">JSON Representation</span></span>
<span data-ttu-id="6192a-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6192a-168">Here is a JSON representation of the resource.</span></span>
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









