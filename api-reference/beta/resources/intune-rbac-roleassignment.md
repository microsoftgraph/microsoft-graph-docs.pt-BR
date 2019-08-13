---
title: Tipo de recurso roleAssignment
description: O recurso de Atribuição de Função. Atribuições de função unem uma definição de função a membros e escopos. Pode haver uma ou mais atribuições de função por função. Aplica-se às funções internas e personalizadas
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9f9a76366ca97464b4180a693e85d8d68d7358a8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369252"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="9cf23-106">Tipo de recurso roleAssignment</span><span class="sxs-lookup"><span data-stu-id="9cf23-106">roleAssignment resource type</span></span>

> <span data-ttu-id="9cf23-107">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9cf23-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9cf23-108">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9cf23-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cf23-109">O recurso de Atribuição de Função.</span><span class="sxs-lookup"><span data-stu-id="9cf23-109">The Role Assignment resource.</span></span> <span data-ttu-id="9cf23-110">Atribuições de função unem uma definição de função a membros e escopos.</span><span class="sxs-lookup"><span data-stu-id="9cf23-110">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="9cf23-111">Pode haver uma ou mais atribuições de função por função.</span><span class="sxs-lookup"><span data-stu-id="9cf23-111">There can be one or more role assignments per role.</span></span> <span data-ttu-id="9cf23-112">Aplica-se às funções internas e personalizadas</span><span class="sxs-lookup"><span data-stu-id="9cf23-112">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="9cf23-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="9cf23-113">Methods</span></span>
|<span data-ttu-id="9cf23-114">Método</span><span class="sxs-lookup"><span data-stu-id="9cf23-114">Method</span></span>|<span data-ttu-id="9cf23-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9cf23-115">Return Type</span></span>|<span data-ttu-id="9cf23-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cf23-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9cf23-117">Listar roleAssignments</span><span class="sxs-lookup"><span data-stu-id="9cf23-117">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="9cf23-118">Conjunto [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9cf23-118">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="9cf23-119">Listar propriedades e relações de objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9cf23-119">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="9cf23-120">Obter roleAssignment</span><span class="sxs-lookup"><span data-stu-id="9cf23-120">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="9cf23-121">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="9cf23-121">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="9cf23-122">Ler propriedades e relações de objetos de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9cf23-122">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="9cf23-123">Create roleAssignment</span><span class="sxs-lookup"><span data-stu-id="9cf23-123">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="9cf23-124">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="9cf23-124">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="9cf23-125">Criar um novo objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9cf23-125">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="9cf23-126">Excluir roleAssignment</span><span class="sxs-lookup"><span data-stu-id="9cf23-126">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="9cf23-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9cf23-127">None</span></span>|<span data-ttu-id="9cf23-128">Excluir [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9cf23-128">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="9cf23-129">Atualizar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="9cf23-129">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="9cf23-130">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="9cf23-130">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="9cf23-131">Atualizar as propriedades de um objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9cf23-131">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9cf23-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9cf23-132">Properties</span></span>
|<span data-ttu-id="9cf23-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9cf23-133">Property</span></span>|<span data-ttu-id="9cf23-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="9cf23-134">Type</span></span>|<span data-ttu-id="9cf23-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cf23-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cf23-136">id</span><span class="sxs-lookup"><span data-stu-id="9cf23-136">id</span></span>|<span data-ttu-id="9cf23-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9cf23-137">String</span></span>|<span data-ttu-id="9cf23-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9cf23-138">Key of the entity.</span></span> <span data-ttu-id="9cf23-139">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="9cf23-139">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="9cf23-140">displayName</span><span class="sxs-lookup"><span data-stu-id="9cf23-140">displayName</span></span>|<span data-ttu-id="9cf23-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9cf23-141">String</span></span>|<span data-ttu-id="9cf23-142">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="9cf23-142">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="9cf23-143">descrição</span><span class="sxs-lookup"><span data-stu-id="9cf23-143">description</span></span>|<span data-ttu-id="9cf23-144">String</span><span class="sxs-lookup"><span data-stu-id="9cf23-144">String</span></span>|<span data-ttu-id="9cf23-145">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="9cf23-145">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="9cf23-146">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="9cf23-146">scopeMembers</span></span>|<span data-ttu-id="9cf23-147">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9cf23-147">String collection</span></span>|<span data-ttu-id="9cf23-148">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="9cf23-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="9cf23-149">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9cf23-149">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="9cf23-150">scopeType</span><span class="sxs-lookup"><span data-stu-id="9cf23-150">scopeType</span></span>|[<span data-ttu-id="9cf23-151">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="9cf23-151">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="9cf23-152">Especifica o tipo de escopo de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="9cf23-152">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="9cf23-153">O tipo padrão ' ResourceScope ' permite a atribuição de ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="9cf23-153">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="9cf23-154">Para ' mydevices ', ' AllLicensedUsers ' e ' AllDevicesAndLicensedUsers ', a propriedade ResourceScopes deve ser deixada vazia.</span><span class="sxs-lookup"><span data-stu-id="9cf23-154">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="9cf23-155">Os valores possíveis são: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="9cf23-155">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="9cf23-156">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="9cf23-156">resourceScopes</span></span>|<span data-ttu-id="9cf23-157">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9cf23-157">String collection</span></span>|<span data-ttu-id="9cf23-158">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="9cf23-158">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="9cf23-159">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9cf23-159">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9cf23-160">Relações</span><span class="sxs-lookup"><span data-stu-id="9cf23-160">Relationships</span></span>
|<span data-ttu-id="9cf23-161">Relação</span><span class="sxs-lookup"><span data-stu-id="9cf23-161">Relationship</span></span>|<span data-ttu-id="9cf23-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="9cf23-162">Type</span></span>|<span data-ttu-id="9cf23-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cf23-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cf23-164">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="9cf23-164">roleDefinition</span></span>|[<span data-ttu-id="9cf23-165">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="9cf23-165">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="9cf23-166">A definição de função da qual essa atribuição faz parte.</span><span class="sxs-lookup"><span data-stu-id="9cf23-166">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9cf23-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9cf23-167">JSON Representation</span></span>
<span data-ttu-id="9cf23-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9cf23-168">Here is a JSON representation of the resource.</span></span>
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



