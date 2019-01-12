---
title: Tipo de recurso roleAssignment
description: O recurso de Atribuição de Função. Atribuições de função unem uma definição de função a membros e escopos. Pode haver uma ou mais atribuições de função por função. Aplica-se às funções internas e personalizadas.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d3f50e028bed17daf9acfe0eaf62776476b1bb61
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927566"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="f3365-106">Tipo de recurso roleAssignment</span><span class="sxs-lookup"><span data-stu-id="f3365-106">roleAssignment resource type</span></span>

> <span data-ttu-id="f3365-107">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f3365-107">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3365-108">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f3365-108">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3365-109">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f3365-109">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3365-110">O recurso de Atribuição de Função.</span><span class="sxs-lookup"><span data-stu-id="f3365-110">The Role Assignment resource.</span></span> <span data-ttu-id="f3365-111">Atribuições de função unem uma definição de função a membros e escopos.</span><span class="sxs-lookup"><span data-stu-id="f3365-111">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="f3365-112">Pode haver uma ou mais atribuições de função por função.</span><span class="sxs-lookup"><span data-stu-id="f3365-112">There can be one or more role assignments per role.</span></span> <span data-ttu-id="f3365-113">Aplica-se às funções internas e personalizadas</span><span class="sxs-lookup"><span data-stu-id="f3365-113">This applies to custom and built-in roles.</span></span>
## <a name="methods"></a><span data-ttu-id="f3365-114">Métodos</span><span class="sxs-lookup"><span data-stu-id="f3365-114">Methods</span></span>
|<span data-ttu-id="f3365-115">Método</span><span class="sxs-lookup"><span data-stu-id="f3365-115">Method</span></span>|<span data-ttu-id="f3365-116">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f3365-116">Return Type</span></span>|<span data-ttu-id="f3365-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3365-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f3365-118">Listar roleAssignments</span><span class="sxs-lookup"><span data-stu-id="f3365-118">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="f3365-119">Conjunto [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f3365-119">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="f3365-120">Listar propriedades e relações de objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f3365-120">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="f3365-121">Obter roleAssignment</span><span class="sxs-lookup"><span data-stu-id="f3365-121">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="f3365-122">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="f3365-122">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="f3365-123">Ler propriedades e relações de objetos de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f3365-123">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="f3365-124">Create roleAssignment</span><span class="sxs-lookup"><span data-stu-id="f3365-124">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="f3365-125">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="f3365-125">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="f3365-126">Criar um novo objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f3365-126">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="f3365-127">Excluir roleAssignment</span><span class="sxs-lookup"><span data-stu-id="f3365-127">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="f3365-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f3365-128">None</span></span>|<span data-ttu-id="f3365-129">Excluir [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f3365-129">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="f3365-130">Atualizar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="f3365-130">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="f3365-131">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="f3365-131">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="f3365-132">Atualizar as propriedades de um objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f3365-132">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f3365-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f3365-133">Properties</span></span>
|<span data-ttu-id="f3365-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3365-134">Property</span></span>|<span data-ttu-id="f3365-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3365-135">Type</span></span>|<span data-ttu-id="f3365-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3365-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3365-137">id</span><span class="sxs-lookup"><span data-stu-id="f3365-137">id</span></span>|<span data-ttu-id="f3365-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3365-138">String</span></span>|<span data-ttu-id="f3365-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f3365-139">Key of the entity.</span></span> <span data-ttu-id="f3365-140">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="f3365-140">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="f3365-141">displayName</span><span class="sxs-lookup"><span data-stu-id="f3365-141">displayName</span></span>|<span data-ttu-id="f3365-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3365-142">String</span></span>|<span data-ttu-id="f3365-143">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f3365-143">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="f3365-144">descrição</span><span class="sxs-lookup"><span data-stu-id="f3365-144">description</span></span>|<span data-ttu-id="f3365-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3365-145">String</span></span>|<span data-ttu-id="f3365-146">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f3365-146">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="f3365-147">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="f3365-147">scopeMembers</span></span>|<span data-ttu-id="f3365-148">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3365-148">String collection</span></span>|<span data-ttu-id="f3365-149">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="f3365-149">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="f3365-150">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f3365-150">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="f3365-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="f3365-151">scopeType</span></span>|[<span data-ttu-id="f3365-152">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="f3365-152">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="f3365-153">Especifica o tipo de escopo para uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f3365-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="f3365-154">O tipo de padrão 'ResourceScope' permite que a atribuição de ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="f3365-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="f3365-155">Para 'AllDevices', 'AllLicensedUsers' e 'AllDevicesAndLicensedUsers', a propriedade ResourceScopes deve ser deixada vazia.</span><span class="sxs-lookup"><span data-stu-id="f3365-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="f3365-156">Os valores possíveis são: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="f3365-156">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="f3365-157">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="f3365-157">resourceScopes</span></span>|<span data-ttu-id="f3365-158">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3365-158">String collection</span></span>|<span data-ttu-id="f3365-159">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="f3365-159">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="f3365-160">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f3365-160">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3365-161">Relações</span><span class="sxs-lookup"><span data-stu-id="f3365-161">Relationships</span></span>
|<span data-ttu-id="f3365-162">Relação</span><span class="sxs-lookup"><span data-stu-id="f3365-162">Relationship</span></span>|<span data-ttu-id="f3365-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3365-163">Type</span></span>|<span data-ttu-id="f3365-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3365-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3365-165">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="f3365-165">roleDefinition</span></span>|[<span data-ttu-id="f3365-166">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="f3365-166">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="f3365-167">A definição de função da qual essa atribuição faz parte.</span><span class="sxs-lookup"><span data-stu-id="f3365-167">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f3365-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f3365-168">JSON Representation</span></span>
<span data-ttu-id="f3365-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f3365-169">Here is a JSON representation of the resource.</span></span>
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





