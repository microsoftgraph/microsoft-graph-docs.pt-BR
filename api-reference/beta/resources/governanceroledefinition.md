---
title: tipo de recurso de governanceRoleDefinition
description: Representa as definições de função. Para obter recursos Azure, ela pode representar funções de RBAC do Azure, proprietário, leitor, colaborador, etc.
ms.openlocfilehash: 057d74276b41abad47eb60ce48a99f1160c401ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034777"
---
# <a name="governanceroledefinition-resource-type"></a><span data-ttu-id="16cd8-104">tipo de recurso de governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="16cd8-104">governanceRoleDefinition resource type</span></span>

> <span data-ttu-id="16cd8-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="16cd8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16cd8-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="16cd8-106">Use of these APIs in production applications is not supported.</span></span> 


<span data-ttu-id="16cd8-107">Representa as definições de função.</span><span class="sxs-lookup"><span data-stu-id="16cd8-107">Represents the role definitions.</span></span> <span data-ttu-id="16cd8-108">Para obter recursos Azure, ela pode representar funções de RBAC do Azure, proprietário, leitor, colaborador, etc.</span><span class="sxs-lookup"><span data-stu-id="16cd8-108">For Azure resources, it can represent Azure RBAC roles, such as Owner, Reader, Contributor, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="16cd8-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="16cd8-109">Methods</span></span>

| <span data-ttu-id="16cd8-110">Método</span><span class="sxs-lookup"><span data-stu-id="16cd8-110">Method</span></span>          | <span data-ttu-id="16cd8-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="16cd8-111">Return Type</span></span> |<span data-ttu-id="16cd8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="16cd8-112">Description</span></span>|
|:---------------|:--------|:--------|:----------|
|[<span data-ttu-id="16cd8-113">List</span><span class="sxs-lookup"><span data-stu-id="16cd8-113">List</span></span>](../api/governanceroledefinition-list.md) | <span data-ttu-id="16cd8-114">coleção [governanceRoleDefinition](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="16cd8-114">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span> |<span data-ttu-id="16cd8-115">Uma coleção de definições de função em um recurso de lista.</span><span class="sxs-lookup"><span data-stu-id="16cd8-115">List a collection of role definitions on a resource.</span></span>|
|[<span data-ttu-id="16cd8-116">Get</span><span class="sxs-lookup"><span data-stu-id="16cd8-116">Get</span></span>](../api/governanceroledefinition-get.md) | [<span data-ttu-id="16cd8-117">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="16cd8-117">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md) |<span data-ttu-id="16cd8-118">Leia as propriedades e os relacionamentos de uma entidade de definição de função especificado pelo id.</span><span class="sxs-lookup"><span data-stu-id="16cd8-118">Read properties and relationships of a role definition entity specified by id.</span></span>|
<span data-ttu-id="16cd8-119">Não `POST`, `PUT`, `PATCH`, `DELETE` tem suporte nos `roleDefinitions` conjunto de entidade para agora.</span><span class="sxs-lookup"><span data-stu-id="16cd8-119">No `POST`, `PUT`, `PATCH`, `DELETE` is supported on `roleDefinitions` entity set for now.</span></span>
## <a name="properties"></a><span data-ttu-id="16cd8-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="16cd8-120">Properties</span></span>
| <span data-ttu-id="16cd8-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16cd8-121">Property</span></span>  | <span data-ttu-id="16cd8-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="16cd8-122">Type</span></span>      |<span data-ttu-id="16cd8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="16cd8-123">Description</span></span>|
|:----|:----------|:----------|:----------|
|<span data-ttu-id="16cd8-124">id</span><span class="sxs-lookup"><span data-stu-id="16cd8-124">id</span></span>         |<span data-ttu-id="16cd8-125">String</span><span class="sxs-lookup"><span data-stu-id="16cd8-125">String</span></span>     |<span data-ttu-id="16cd8-126">A id da definição de função.</span><span class="sxs-lookup"><span data-stu-id="16cd8-126">The id of the role definition.</span></span> |
|<span data-ttu-id="16cd8-127">resourceId</span><span class="sxs-lookup"><span data-stu-id="16cd8-127">resourceId</span></span> |<span data-ttu-id="16cd8-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16cd8-128">String</span></span>     |<span data-ttu-id="16cd8-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16cd8-129">Required.</span></span> <span data-ttu-id="16cd8-130">A identificação do recurso associado à definição de função.</span><span class="sxs-lookup"><span data-stu-id="16cd8-130">The id of the resource associated with the role definition.</span></span> |
|<span data-ttu-id="16cd8-131">externalId</span><span class="sxs-lookup"><span data-stu-id="16cd8-131">externalId</span></span>   |<span data-ttu-id="16cd8-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16cd8-132">String</span></span>     |<span data-ttu-id="16cd8-133">A id externa da definição de função.</span><span class="sxs-lookup"><span data-stu-id="16cd8-133">The external id of the role definition.</span></span>|
|<span data-ttu-id="16cd8-134">displayName</span><span class="sxs-lookup"><span data-stu-id="16cd8-134">displayName</span></span>|<span data-ttu-id="16cd8-135">String</span><span class="sxs-lookup"><span data-stu-id="16cd8-135">String</span></span>     |<span data-ttu-id="16cd8-136">O nome de exibição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="16cd8-136">The display name of the role definition.</span></span>|
|<span data-ttu-id="16cd8-137">subjectCount</span><span class="sxs-lookup"><span data-stu-id="16cd8-137">subjectCount</span></span>|<span data-ttu-id="16cd8-138">Int32</span><span class="sxs-lookup"><span data-stu-id="16cd8-138">Int32</span></span>     |<span data-ttu-id="16cd8-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="16cd8-139">Optional.</span></span> <span data-ttu-id="16cd8-140">O número de assuntos que são atribuídas à função.</span><span class="sxs-lookup"><span data-stu-id="16cd8-140">The number of subjects that are assigned to the role.</span></span> <span data-ttu-id="16cd8-141">Representa o status de acesso do solicitador para o recurso.</span><span class="sxs-lookup"><span data-stu-id="16cd8-141">It represents the status of the requestor's access to the resource.</span></span> <span data-ttu-id="16cd8-142">Para obter a propriedade, faça uso explicitamente `$select=subjectCount` na consulta.</span><span class="sxs-lookup"><span data-stu-id="16cd8-142">To get the property, please explictly use `$select=subjectCount` in the query.</span></span>|
|<span data-ttu-id="16cd8-143">eligibleAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="16cd8-143">eligibleAssignmentCount</span></span>|<span data-ttu-id="16cd8-144">Int32</span><span class="sxs-lookup"><span data-stu-id="16cd8-144">Int32</span></span>|<span data-ttu-id="16cd8-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="16cd8-145">Optional.</span></span> <span data-ttu-id="16cd8-146">O número de atribuições de função elegíveis associado à definição de função.</span><span class="sxs-lookup"><span data-stu-id="16cd8-146">The number of eligible role assignments associated with the role definition.</span></span> <span data-ttu-id="16cd8-147">Para obter a propriedade, faça uso explicitamente `$select=eligibleAssignmentCount` na consulta.</span><span class="sxs-lookup"><span data-stu-id="16cd8-147">To get the property, please explictly use `$select=eligibleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="16cd8-148">activeAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="16cd8-148">activeAssignmentCount</span></span>|<span data-ttu-id="16cd8-149">Int32</span><span class="sxs-lookup"><span data-stu-id="16cd8-149">Int32</span></span>    |<span data-ttu-id="16cd8-150">Opcional.</span><span class="sxs-lookup"><span data-stu-id="16cd8-150">Optional.</span></span> <span data-ttu-id="16cd8-151">O número de atribuições de função ativa associado à definição de função.</span><span class="sxs-lookup"><span data-stu-id="16cd8-151">The number of active role assignments associated with the role definition.</span></span>  <span data-ttu-id="16cd8-152">Para obter a propriedade, faça uso explicitamente `$select=activeAssignmentCount` na consulta.</span><span class="sxs-lookup"><span data-stu-id="16cd8-152">To get the property, please explictly use `$select=activeAssignmentCount` in the query.</span></span>|


## <a name="relationships"></a><span data-ttu-id="16cd8-153">Relações</span><span class="sxs-lookup"><span data-stu-id="16cd8-153">Relationships</span></span>
| <span data-ttu-id="16cd8-154">Relação</span><span class="sxs-lookup"><span data-stu-id="16cd8-154">Relationship</span></span> | <span data-ttu-id="16cd8-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="16cd8-155">Type</span></span>   |<span data-ttu-id="16cd8-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="16cd8-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16cd8-157">recurso</span><span class="sxs-lookup"><span data-stu-id="16cd8-157">resource</span></span>|[<span data-ttu-id="16cd8-158">governanceResource</span><span class="sxs-lookup"><span data-stu-id="16cd8-158">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="16cd8-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="16cd8-159">Read-only.</span></span> <span data-ttu-id="16cd8-160">O recurso associado para a definição de função.</span><span class="sxs-lookup"><span data-stu-id="16cd8-160">The associated resource for the role definition.</span></span>|
|<span data-ttu-id="16cd8-161">roleSetting</span><span class="sxs-lookup"><span data-stu-id="16cd8-161">roleSetting</span></span>|[<span data-ttu-id="16cd8-162">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="16cd8-162">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)|<span data-ttu-id="16cd8-163">A configuração da função associada para a definição de função.</span><span class="sxs-lookup"><span data-stu-id="16cd8-163">The associated role setting for the role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="16cd8-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="16cd8-164">JSON representation</span></span>

<span data-ttu-id="16cd8-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="16cd8-165">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "externalId": "String",
  "displayName": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->