---
title: Tipo de recurso roleAssignment
description: O recurso de Atribuição de Função. Atribuições de função unem uma definição de função a membros e escopos. Pode haver uma ou mais atribuições de função por função. Aplica-se às funções internas e personalizadas
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 82c4984de97a3e4f45623486bd6d5f3cd82936e9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259148"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="d5b7e-106">Tipo de recurso roleAssignment</span><span class="sxs-lookup"><span data-stu-id="d5b7e-106">roleAssignment resource type</span></span>

<span data-ttu-id="d5b7e-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5b7e-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5b7e-108">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d5b7e-108">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5b7e-109">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d5b7e-109">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5b7e-110">O recurso de Atribuição de Função.</span><span class="sxs-lookup"><span data-stu-id="d5b7e-110">The Role Assignment resource.</span></span> <span data-ttu-id="d5b7e-111">Atribuições de função unem uma definição de função a membros e escopos.</span><span class="sxs-lookup"><span data-stu-id="d5b7e-111">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="d5b7e-112">Pode haver uma ou mais atribuições de função por função.</span><span class="sxs-lookup"><span data-stu-id="d5b7e-112">There can be one or more role assignments per role.</span></span> <span data-ttu-id="d5b7e-113">Aplica-se às funções internas e personalizadas</span><span class="sxs-lookup"><span data-stu-id="d5b7e-113">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="d5b7e-114">Métodos</span><span class="sxs-lookup"><span data-stu-id="d5b7e-114">Methods</span></span>
|<span data-ttu-id="d5b7e-115">Método</span><span class="sxs-lookup"><span data-stu-id="d5b7e-115">Method</span></span>|<span data-ttu-id="d5b7e-116">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d5b7e-116">Return Type</span></span>|<span data-ttu-id="d5b7e-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5b7e-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d5b7e-118">Listar roleAssignments</span><span class="sxs-lookup"><span data-stu-id="d5b7e-118">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="d5b7e-119">Conjunto [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d5b7e-119">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="d5b7e-120">Listar propriedades e relações de objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d5b7e-120">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="d5b7e-121">Obter roleAssignment</span><span class="sxs-lookup"><span data-stu-id="d5b7e-121">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="d5b7e-122">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="d5b7e-122">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="d5b7e-123">Ler propriedades e relações de objetos de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d5b7e-123">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="d5b7e-124">Create roleAssignment</span><span class="sxs-lookup"><span data-stu-id="d5b7e-124">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="d5b7e-125">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="d5b7e-125">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="d5b7e-126">Criar um novo objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d5b7e-126">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="d5b7e-127">Excluir roleAssignment</span><span class="sxs-lookup"><span data-stu-id="d5b7e-127">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="d5b7e-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d5b7e-128">None</span></span>|<span data-ttu-id="d5b7e-129">Excluir [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d5b7e-129">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="d5b7e-130">Atualizar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="d5b7e-130">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="d5b7e-131">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="d5b7e-131">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="d5b7e-132">Atualizar as propriedades de um objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d5b7e-132">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d5b7e-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5b7e-133">Properties</span></span>
|<span data-ttu-id="d5b7e-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5b7e-134">Property</span></span>|<span data-ttu-id="d5b7e-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5b7e-135">Type</span></span>|<span data-ttu-id="d5b7e-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5b7e-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5b7e-137">id</span><span class="sxs-lookup"><span data-stu-id="d5b7e-137">id</span></span>|<span data-ttu-id="d5b7e-138">String</span><span class="sxs-lookup"><span data-stu-id="d5b7e-138">String</span></span>|<span data-ttu-id="d5b7e-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d5b7e-139">Key of the entity.</span></span> <span data-ttu-id="d5b7e-140">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="d5b7e-140">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="d5b7e-141">displayName</span><span class="sxs-lookup"><span data-stu-id="d5b7e-141">displayName</span></span>|<span data-ttu-id="d5b7e-142">String</span><span class="sxs-lookup"><span data-stu-id="d5b7e-142">String</span></span>|<span data-ttu-id="d5b7e-143">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d5b7e-143">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="d5b7e-144">description</span><span class="sxs-lookup"><span data-stu-id="d5b7e-144">description</span></span>|<span data-ttu-id="d5b7e-145">String</span><span class="sxs-lookup"><span data-stu-id="d5b7e-145">String</span></span>|<span data-ttu-id="d5b7e-146">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d5b7e-146">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="d5b7e-147">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="d5b7e-147">scopeMembers</span></span>|<span data-ttu-id="d5b7e-148">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5b7e-148">String collection</span></span>|<span data-ttu-id="d5b7e-149">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="d5b7e-149">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="d5b7e-150">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d5b7e-150">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="d5b7e-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="d5b7e-151">scopeType</span></span>|[<span data-ttu-id="d5b7e-152">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="d5b7e-152">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="d5b7e-153">Especifica o tipo de escopo de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d5b7e-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="d5b7e-154">O tipo padrão ' ResourceScope ' permite a atribuição de ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="d5b7e-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="d5b7e-155">Para ' mydevices ', ' AllLicensedUsers ' e ' AllDevicesAndLicensedUsers ', a propriedade ResourceScopes deve ser deixada vazia.</span><span class="sxs-lookup"><span data-stu-id="d5b7e-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="d5b7e-156">Os valores possíveis são: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="d5b7e-156">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="d5b7e-157">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="d5b7e-157">resourceScopes</span></span>|<span data-ttu-id="d5b7e-158">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5b7e-158">String collection</span></span>|<span data-ttu-id="d5b7e-159">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="d5b7e-159">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="d5b7e-160">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d5b7e-160">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5b7e-161">Relações</span><span class="sxs-lookup"><span data-stu-id="d5b7e-161">Relationships</span></span>
|<span data-ttu-id="d5b7e-162">Relação</span><span class="sxs-lookup"><span data-stu-id="d5b7e-162">Relationship</span></span>|<span data-ttu-id="d5b7e-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5b7e-163">Type</span></span>|<span data-ttu-id="d5b7e-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5b7e-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5b7e-165">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="d5b7e-165">roleDefinition</span></span>|[<span data-ttu-id="d5b7e-166">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="d5b7e-166">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="d5b7e-167">A definição de função da qual essa atribuição faz parte.</span><span class="sxs-lookup"><span data-stu-id="d5b7e-167">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d5b7e-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5b7e-168">JSON Representation</span></span>
<span data-ttu-id="d5b7e-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5b7e-169">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "scopeMembers": [
    "String"
  ],
  "scopeType": "String",
  "resourceScopes": [
    "String"
  ]
}
```




