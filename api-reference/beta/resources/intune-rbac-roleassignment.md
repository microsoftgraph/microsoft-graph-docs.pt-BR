---
title: Tipo de recurso roleAssignment
description: O recurso de Atribuição de Função. Atribuições de função unem uma definição de função a membros e escopos. Pode haver uma ou mais atribuições de função por função. Aplica-se às funções internas e personalizadas
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c72b6ee403a4a0b06cd1181da584dbb7b4729f8d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967599"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="de8de-106">Tipo de recurso roleAssignment</span><span class="sxs-lookup"><span data-stu-id="de8de-106">roleAssignment resource type</span></span>

> <span data-ttu-id="de8de-107">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="de8de-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de8de-108">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="de8de-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de8de-109">O recurso de Atribuição de Função.</span><span class="sxs-lookup"><span data-stu-id="de8de-109">The Role Assignment resource.</span></span> <span data-ttu-id="de8de-110">Atribuições de função unem uma definição de função a membros e escopos.</span><span class="sxs-lookup"><span data-stu-id="de8de-110">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="de8de-111">Pode haver uma ou mais atribuições de função por função.</span><span class="sxs-lookup"><span data-stu-id="de8de-111">There can be one or more role assignments per role.</span></span> <span data-ttu-id="de8de-112">Aplica-se às funções internas e personalizadas</span><span class="sxs-lookup"><span data-stu-id="de8de-112">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="de8de-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="de8de-113">Methods</span></span>
|<span data-ttu-id="de8de-114">Método</span><span class="sxs-lookup"><span data-stu-id="de8de-114">Method</span></span>|<span data-ttu-id="de8de-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="de8de-115">Return Type</span></span>|<span data-ttu-id="de8de-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="de8de-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="de8de-117">Listar roleAssignments</span><span class="sxs-lookup"><span data-stu-id="de8de-117">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="de8de-118">Conjunto [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="de8de-118">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="de8de-119">Listar propriedades e relações de objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="de8de-119">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="de8de-120">Obter roleAssignment</span><span class="sxs-lookup"><span data-stu-id="de8de-120">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="de8de-121">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="de8de-121">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="de8de-122">Ler propriedades e relações de objetos de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="de8de-122">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="de8de-123">Create roleAssignment</span><span class="sxs-lookup"><span data-stu-id="de8de-123">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="de8de-124">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="de8de-124">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="de8de-125">Criar um novo objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="de8de-125">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="de8de-126">Excluir roleAssignment</span><span class="sxs-lookup"><span data-stu-id="de8de-126">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="de8de-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="de8de-127">None</span></span>|<span data-ttu-id="de8de-128">Excluir [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="de8de-128">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="de8de-129">Atualizar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="de8de-129">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="de8de-130">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="de8de-130">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="de8de-131">Atualizar as propriedades de um objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="de8de-131">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="de8de-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="de8de-132">Properties</span></span>
|<span data-ttu-id="de8de-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de8de-133">Property</span></span>|<span data-ttu-id="de8de-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="de8de-134">Type</span></span>|<span data-ttu-id="de8de-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="de8de-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de8de-136">id</span><span class="sxs-lookup"><span data-stu-id="de8de-136">id</span></span>|<span data-ttu-id="de8de-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de8de-137">String</span></span>|<span data-ttu-id="de8de-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="de8de-138">Key of the entity.</span></span> <span data-ttu-id="de8de-139">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="de8de-139">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="de8de-140">displayName</span><span class="sxs-lookup"><span data-stu-id="de8de-140">displayName</span></span>|<span data-ttu-id="de8de-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de8de-141">String</span></span>|<span data-ttu-id="de8de-142">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="de8de-142">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="de8de-143">descrição</span><span class="sxs-lookup"><span data-stu-id="de8de-143">description</span></span>|<span data-ttu-id="de8de-144">String</span><span class="sxs-lookup"><span data-stu-id="de8de-144">String</span></span>|<span data-ttu-id="de8de-145">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="de8de-145">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="de8de-146">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="de8de-146">scopeMembers</span></span>|<span data-ttu-id="de8de-147">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="de8de-147">String collection</span></span>|<span data-ttu-id="de8de-148">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="de8de-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="de8de-149">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="de8de-149">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="de8de-150">scopeType</span><span class="sxs-lookup"><span data-stu-id="de8de-150">scopeType</span></span>|[<span data-ttu-id="de8de-151">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="de8de-151">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="de8de-152">Especifica o tipo de escopo de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="de8de-152">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="de8de-153">O tipo padrão ' ResourceScope ' permite a atribuição de ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="de8de-153">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="de8de-154">Para ' mydevices ', ' AllLicensedUsers ' e ' AllDevicesAndLicensedUsers ', a propriedade ResourceScopes deve ser deixada vazia.</span><span class="sxs-lookup"><span data-stu-id="de8de-154">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="de8de-155">Os valores possíveis são: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="de8de-155">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="de8de-156">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="de8de-156">resourceScopes</span></span>|<span data-ttu-id="de8de-157">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="de8de-157">String collection</span></span>|<span data-ttu-id="de8de-158">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="de8de-158">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="de8de-159">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="de8de-159">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de8de-160">Relações</span><span class="sxs-lookup"><span data-stu-id="de8de-160">Relationships</span></span>
|<span data-ttu-id="de8de-161">Relação</span><span class="sxs-lookup"><span data-stu-id="de8de-161">Relationship</span></span>|<span data-ttu-id="de8de-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="de8de-162">Type</span></span>|<span data-ttu-id="de8de-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="de8de-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de8de-164">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="de8de-164">roleDefinition</span></span>|[<span data-ttu-id="de8de-165">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="de8de-165">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="de8de-166">A definição de função da qual essa atribuição faz parte.</span><span class="sxs-lookup"><span data-stu-id="de8de-166">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="de8de-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="de8de-167">JSON Representation</span></span>
<span data-ttu-id="de8de-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="de8de-168">Here is a JSON representation of the resource.</span></span>
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





