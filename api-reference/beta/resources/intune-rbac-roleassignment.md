---
title: Tipo de recurso roleAssignment
description: O recurso de Atribuição de Função. Atribuições de função unem uma definição de função a membros e escopos. Pode haver uma ou mais atribuições de função por função. Aplica-se às funções internas e personalizadas
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 65a37c749380ce62da56f27aa335e89aa43b6e2e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527544"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="00258-106">Tipo de recurso roleAssignment</span><span class="sxs-lookup"><span data-stu-id="00258-106">roleAssignment resource type</span></span>

<span data-ttu-id="00258-107">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="00258-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00258-108">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="00258-108">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00258-109">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="00258-109">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00258-110">O recurso de Atribuição de Função.</span><span class="sxs-lookup"><span data-stu-id="00258-110">The Role Assignment resource.</span></span> <span data-ttu-id="00258-111">Atribuições de função unem uma definição de função a membros e escopos.</span><span class="sxs-lookup"><span data-stu-id="00258-111">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="00258-112">Pode haver uma ou mais atribuições de função por função.</span><span class="sxs-lookup"><span data-stu-id="00258-112">There can be one or more role assignments per role.</span></span> <span data-ttu-id="00258-113">Aplica-se às funções internas e personalizadas</span><span class="sxs-lookup"><span data-stu-id="00258-113">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="00258-114">Métodos</span><span class="sxs-lookup"><span data-stu-id="00258-114">Methods</span></span>
|<span data-ttu-id="00258-115">Método</span><span class="sxs-lookup"><span data-stu-id="00258-115">Method</span></span>|<span data-ttu-id="00258-116">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="00258-116">Return Type</span></span>|<span data-ttu-id="00258-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="00258-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="00258-118">Listar roleAssignments</span><span class="sxs-lookup"><span data-stu-id="00258-118">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="00258-119">Conjunto [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="00258-119">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="00258-120">Listar propriedades e relações de objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="00258-120">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="00258-121">Obter roleAssignment</span><span class="sxs-lookup"><span data-stu-id="00258-121">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="00258-122">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="00258-122">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="00258-123">Ler propriedades e relações de objetos de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="00258-123">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="00258-124">Create roleAssignment</span><span class="sxs-lookup"><span data-stu-id="00258-124">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="00258-125">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="00258-125">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="00258-126">Criar um novo objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="00258-126">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="00258-127">Excluir roleAssignment</span><span class="sxs-lookup"><span data-stu-id="00258-127">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="00258-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="00258-128">None</span></span>|<span data-ttu-id="00258-129">Excluir [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="00258-129">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="00258-130">Atualizar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="00258-130">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="00258-131">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="00258-131">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="00258-132">Atualizar as propriedades de um objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="00258-132">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="00258-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="00258-133">Properties</span></span>
|<span data-ttu-id="00258-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00258-134">Property</span></span>|<span data-ttu-id="00258-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="00258-135">Type</span></span>|<span data-ttu-id="00258-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="00258-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00258-137">id</span><span class="sxs-lookup"><span data-stu-id="00258-137">id</span></span>|<span data-ttu-id="00258-138">String</span><span class="sxs-lookup"><span data-stu-id="00258-138">String</span></span>|<span data-ttu-id="00258-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="00258-139">Key of the entity.</span></span> <span data-ttu-id="00258-140">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="00258-140">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="00258-141">displayName</span><span class="sxs-lookup"><span data-stu-id="00258-141">displayName</span></span>|<span data-ttu-id="00258-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00258-142">String</span></span>|<span data-ttu-id="00258-143">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="00258-143">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="00258-144">description</span><span class="sxs-lookup"><span data-stu-id="00258-144">description</span></span>|<span data-ttu-id="00258-145">String</span><span class="sxs-lookup"><span data-stu-id="00258-145">String</span></span>|<span data-ttu-id="00258-146">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="00258-146">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="00258-147">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="00258-147">scopeMembers</span></span>|<span data-ttu-id="00258-148">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="00258-148">String collection</span></span>|<span data-ttu-id="00258-149">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="00258-149">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="00258-150">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="00258-150">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="00258-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="00258-151">scopeType</span></span>|[<span data-ttu-id="00258-152">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="00258-152">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="00258-153">Especifica o tipo de escopo de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="00258-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="00258-154">O tipo padrão ' ResourceScope ' permite a atribuição de ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="00258-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="00258-155">Para ' mydevices ', ' AllLicensedUsers ' e ' AllDevicesAndLicensedUsers ', a propriedade ResourceScopes deve ser deixada vazia.</span><span class="sxs-lookup"><span data-stu-id="00258-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="00258-156">Os valores possíveis são: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="00258-156">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="00258-157">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="00258-157">resourceScopes</span></span>|<span data-ttu-id="00258-158">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="00258-158">String collection</span></span>|<span data-ttu-id="00258-159">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="00258-159">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="00258-160">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="00258-160">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00258-161">Relações</span><span class="sxs-lookup"><span data-stu-id="00258-161">Relationships</span></span>
|<span data-ttu-id="00258-162">Relação</span><span class="sxs-lookup"><span data-stu-id="00258-162">Relationship</span></span>|<span data-ttu-id="00258-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="00258-163">Type</span></span>|<span data-ttu-id="00258-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="00258-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00258-165">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="00258-165">roleDefinition</span></span>|[<span data-ttu-id="00258-166">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="00258-166">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="00258-167">A definição de função da qual essa atribuição faz parte.</span><span class="sxs-lookup"><span data-stu-id="00258-167">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00258-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="00258-168">JSON Representation</span></span>
<span data-ttu-id="00258-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="00258-169">Here is a JSON representation of the resource.</span></span>
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



