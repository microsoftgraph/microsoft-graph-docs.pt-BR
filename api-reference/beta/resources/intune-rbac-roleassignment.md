---
title: Tipo de recurso roleAssignment
description: O recurso de Atribuição de Função. Atribuições de função unem uma definição de função a membros e escopos. Pode haver uma ou mais atribuições de função por função. Aplica-se às funções internas e personalizadas.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 11fc37502fa017494ff884cb70f0006277a42600
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415121"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="2900f-106">Tipo de recurso roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2900f-106">roleAssignment resource type</span></span>

> <span data-ttu-id="2900f-107">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="2900f-107">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2900f-108">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2900f-108">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2900f-109">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="2900f-109">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2900f-110">O recurso de Atribuição de Função.</span><span class="sxs-lookup"><span data-stu-id="2900f-110">The Role Assignment resource.</span></span> <span data-ttu-id="2900f-111">Atribuições de função unem uma definição de função a membros e escopos.</span><span class="sxs-lookup"><span data-stu-id="2900f-111">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="2900f-112">Pode haver uma ou mais atribuições de função por função.</span><span class="sxs-lookup"><span data-stu-id="2900f-112">There can be one or more role assignments per role.</span></span> <span data-ttu-id="2900f-113">Aplica-se às funções internas e personalizadas</span><span class="sxs-lookup"><span data-stu-id="2900f-113">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="2900f-114">Métodos</span><span class="sxs-lookup"><span data-stu-id="2900f-114">Methods</span></span>
|<span data-ttu-id="2900f-115">Método</span><span class="sxs-lookup"><span data-stu-id="2900f-115">Method</span></span>|<span data-ttu-id="2900f-116">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2900f-116">Return Type</span></span>|<span data-ttu-id="2900f-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="2900f-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2900f-118">Listar roleAssignments</span><span class="sxs-lookup"><span data-stu-id="2900f-118">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="2900f-119">Conjunto [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2900f-119">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="2900f-120">Listar propriedades e relações de objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2900f-120">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="2900f-121">Obter roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2900f-121">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="2900f-122">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2900f-122">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="2900f-123">Ler propriedades e relações de objetos de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2900f-123">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="2900f-124">Create roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2900f-124">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="2900f-125">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2900f-125">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="2900f-126">Criar um novo objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2900f-126">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="2900f-127">Excluir roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2900f-127">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="2900f-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2900f-128">None</span></span>|<span data-ttu-id="2900f-129">Excluir [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2900f-129">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="2900f-130">Atualizar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2900f-130">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="2900f-131">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2900f-131">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="2900f-132">Atualizar as propriedades de um objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2900f-132">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2900f-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2900f-133">Properties</span></span>
|<span data-ttu-id="2900f-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2900f-134">Property</span></span>|<span data-ttu-id="2900f-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="2900f-135">Type</span></span>|<span data-ttu-id="2900f-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="2900f-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2900f-137">id</span><span class="sxs-lookup"><span data-stu-id="2900f-137">id</span></span>|<span data-ttu-id="2900f-138">String</span><span class="sxs-lookup"><span data-stu-id="2900f-138">String</span></span>|<span data-ttu-id="2900f-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2900f-139">Key of the entity.</span></span> <span data-ttu-id="2900f-140">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="2900f-140">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="2900f-141">displayName</span><span class="sxs-lookup"><span data-stu-id="2900f-141">displayName</span></span>|<span data-ttu-id="2900f-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2900f-142">String</span></span>|<span data-ttu-id="2900f-143">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="2900f-143">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="2900f-144">descrição</span><span class="sxs-lookup"><span data-stu-id="2900f-144">description</span></span>|<span data-ttu-id="2900f-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2900f-145">String</span></span>|<span data-ttu-id="2900f-146">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="2900f-146">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="2900f-147">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="2900f-147">scopeMembers</span></span>|<span data-ttu-id="2900f-148">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2900f-148">String collection</span></span>|<span data-ttu-id="2900f-149">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="2900f-149">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="2900f-150">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2900f-150">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="2900f-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="2900f-151">scopeType</span></span>|[<span data-ttu-id="2900f-152">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="2900f-152">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="2900f-153">Especifica o tipo de escopo para uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="2900f-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="2900f-154">O tipo de padrão 'ResourceScope' permite que a atribuição de ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="2900f-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="2900f-155">Para 'AllDevices', 'AllLicensedUsers' e 'AllDevicesAndLicensedUsers', a propriedade ResourceScopes deve ser deixada vazia.</span><span class="sxs-lookup"><span data-stu-id="2900f-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="2900f-156">Os valores possíveis são: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="2900f-156">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="2900f-157">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="2900f-157">resourceScopes</span></span>|<span data-ttu-id="2900f-158">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2900f-158">String collection</span></span>|<span data-ttu-id="2900f-159">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="2900f-159">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="2900f-160">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2900f-160">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2900f-161">Relações</span><span class="sxs-lookup"><span data-stu-id="2900f-161">Relationships</span></span>
|<span data-ttu-id="2900f-162">Relação</span><span class="sxs-lookup"><span data-stu-id="2900f-162">Relationship</span></span>|<span data-ttu-id="2900f-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="2900f-163">Type</span></span>|<span data-ttu-id="2900f-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="2900f-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2900f-165">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="2900f-165">roleDefinition</span></span>|[<span data-ttu-id="2900f-166">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="2900f-166">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="2900f-167">A definição de função da qual essa atribuição faz parte.</span><span class="sxs-lookup"><span data-stu-id="2900f-167">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2900f-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2900f-168">JSON Representation</span></span>
<span data-ttu-id="2900f-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2900f-169">Here is a JSON representation of the resource.</span></span>
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




