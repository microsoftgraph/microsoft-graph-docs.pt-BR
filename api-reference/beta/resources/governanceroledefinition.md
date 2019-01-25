---
title: tipo de recurso de governanceRoleDefinition
description: Representa as definições de função. Para obter recursos Azure, ela pode representar funções de RBAC do Azure, proprietário, leitor, colaborador, etc.
localization_priority: Normal
ms.openlocfilehash: 867864892bac9107c44ba9125336429248b6697e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528638"
---
# <a name="governanceroledefinition-resource-type"></a><span data-ttu-id="14d58-104">tipo de recurso de governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="14d58-104">governanceRoleDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="14d58-105">Representa as definições de função.</span><span class="sxs-lookup"><span data-stu-id="14d58-105">Represents the role definitions.</span></span> <span data-ttu-id="14d58-106">Para obter recursos Azure, ela pode representar funções de RBAC do Azure, proprietário, leitor, colaborador, etc.</span><span class="sxs-lookup"><span data-stu-id="14d58-106">For Azure resources, it can represent Azure RBAC roles, such as Owner, Reader, Contributor, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="14d58-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="14d58-107">Methods</span></span>

| <span data-ttu-id="14d58-108">Método</span><span class="sxs-lookup"><span data-stu-id="14d58-108">Method</span></span>          | <span data-ttu-id="14d58-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="14d58-109">Return Type</span></span> |<span data-ttu-id="14d58-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="14d58-110">Description</span></span>|
|:---------------|:--------|:--------|:----------|
|[<span data-ttu-id="14d58-111">List</span><span class="sxs-lookup"><span data-stu-id="14d58-111">List</span></span>](../api/governanceroledefinition-list.md) | <span data-ttu-id="14d58-112">coleção [governanceRoleDefinition](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="14d58-112">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span> |<span data-ttu-id="14d58-113">Uma coleção de definições de função em um recurso de lista.</span><span class="sxs-lookup"><span data-stu-id="14d58-113">List a collection of role definitions on a resource.</span></span>|
|[<span data-ttu-id="14d58-114">Get</span><span class="sxs-lookup"><span data-stu-id="14d58-114">Get</span></span>](../api/governanceroledefinition-get.md) | [<span data-ttu-id="14d58-115">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="14d58-115">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md) |<span data-ttu-id="14d58-116">Leia as propriedades e os relacionamentos de uma entidade de definição de função especificado pelo id.</span><span class="sxs-lookup"><span data-stu-id="14d58-116">Read properties and relationships of a role definition entity specified by id.</span></span>|
<span data-ttu-id="14d58-117">Não `POST`, `PUT`, `PATCH`, `DELETE` tem suporte nos `roleDefinitions` conjunto de entidade para agora.</span><span class="sxs-lookup"><span data-stu-id="14d58-117">No `POST`, `PUT`, `PATCH`, `DELETE` is supported on `roleDefinitions` entity set for now.</span></span>
## <a name="properties"></a><span data-ttu-id="14d58-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="14d58-118">Properties</span></span>
| <span data-ttu-id="14d58-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14d58-119">Property</span></span>  | <span data-ttu-id="14d58-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="14d58-120">Type</span></span>      |<span data-ttu-id="14d58-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="14d58-121">Description</span></span>|
|:----|:----------|:----------|:----------|
|<span data-ttu-id="14d58-122">id</span><span class="sxs-lookup"><span data-stu-id="14d58-122">id</span></span>         |<span data-ttu-id="14d58-123">String</span><span class="sxs-lookup"><span data-stu-id="14d58-123">String</span></span>     |<span data-ttu-id="14d58-124">A id da definição de função.</span><span class="sxs-lookup"><span data-stu-id="14d58-124">The id of the role definition.</span></span> |
|<span data-ttu-id="14d58-125">resourceId</span><span class="sxs-lookup"><span data-stu-id="14d58-125">resourceId</span></span> |<span data-ttu-id="14d58-126">String</span><span class="sxs-lookup"><span data-stu-id="14d58-126">String</span></span>     |<span data-ttu-id="14d58-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14d58-127">Required.</span></span> <span data-ttu-id="14d58-128">A identificação do recurso associado à definição de função.</span><span class="sxs-lookup"><span data-stu-id="14d58-128">The id of the resource associated with the role definition.</span></span> |
|<span data-ttu-id="14d58-129">externalId</span><span class="sxs-lookup"><span data-stu-id="14d58-129">externalId</span></span>   |<span data-ttu-id="14d58-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14d58-130">String</span></span>     |<span data-ttu-id="14d58-131">A id externa da definição de função.</span><span class="sxs-lookup"><span data-stu-id="14d58-131">The external id of the role definition.</span></span>|
|<span data-ttu-id="14d58-132">displayName</span><span class="sxs-lookup"><span data-stu-id="14d58-132">displayName</span></span>|<span data-ttu-id="14d58-133">String</span><span class="sxs-lookup"><span data-stu-id="14d58-133">String</span></span>     |<span data-ttu-id="14d58-134">O nome de exibição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="14d58-134">The display name of the role definition.</span></span>|
|<span data-ttu-id="14d58-135">subjectCount</span><span class="sxs-lookup"><span data-stu-id="14d58-135">subjectCount</span></span>|<span data-ttu-id="14d58-136">Int32</span><span class="sxs-lookup"><span data-stu-id="14d58-136">Int32</span></span>     |<span data-ttu-id="14d58-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="14d58-137">Optional.</span></span> <span data-ttu-id="14d58-138">O número de assuntos que são atribuídas à função.</span><span class="sxs-lookup"><span data-stu-id="14d58-138">The number of subjects that are assigned to the role.</span></span> <span data-ttu-id="14d58-139">Representa o status de acesso do solicitador para o recurso.</span><span class="sxs-lookup"><span data-stu-id="14d58-139">It represents the status of the requestor's access to the resource.</span></span> <span data-ttu-id="14d58-140">Para obter a propriedade, faça uso explicitamente `$select=subjectCount` na consulta.</span><span class="sxs-lookup"><span data-stu-id="14d58-140">To get the property, please explictly use `$select=subjectCount` in the query.</span></span>|
|<span data-ttu-id="14d58-141">eligibleAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="14d58-141">eligibleAssignmentCount</span></span>|<span data-ttu-id="14d58-142">Int32</span><span class="sxs-lookup"><span data-stu-id="14d58-142">Int32</span></span>|<span data-ttu-id="14d58-143">Opcional.</span><span class="sxs-lookup"><span data-stu-id="14d58-143">Optional.</span></span> <span data-ttu-id="14d58-144">O número de atribuições de função elegíveis associado à definição de função.</span><span class="sxs-lookup"><span data-stu-id="14d58-144">The number of eligible role assignments associated with the role definition.</span></span> <span data-ttu-id="14d58-145">Para obter a propriedade, faça uso explicitamente `$select=eligibleAssignmentCount` na consulta.</span><span class="sxs-lookup"><span data-stu-id="14d58-145">To get the property, please explictly use `$select=eligibleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="14d58-146">activeAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="14d58-146">activeAssignmentCount</span></span>|<span data-ttu-id="14d58-147">Int32</span><span class="sxs-lookup"><span data-stu-id="14d58-147">Int32</span></span>    |<span data-ttu-id="14d58-148">Opcional.</span><span class="sxs-lookup"><span data-stu-id="14d58-148">Optional.</span></span> <span data-ttu-id="14d58-149">O número de atribuições de função ativa associado à definição de função.</span><span class="sxs-lookup"><span data-stu-id="14d58-149">The number of active role assignments associated with the role definition.</span></span>  <span data-ttu-id="14d58-150">Para obter a propriedade, faça uso explicitamente `$select=activeAssignmentCount` na consulta.</span><span class="sxs-lookup"><span data-stu-id="14d58-150">To get the property, please explictly use `$select=activeAssignmentCount` in the query.</span></span>|


## <a name="relationships"></a><span data-ttu-id="14d58-151">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="14d58-151">Relationships</span></span>
| <span data-ttu-id="14d58-152">Relação</span><span class="sxs-lookup"><span data-stu-id="14d58-152">Relationship</span></span> | <span data-ttu-id="14d58-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="14d58-153">Type</span></span>   |<span data-ttu-id="14d58-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="14d58-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14d58-155">recurso</span><span class="sxs-lookup"><span data-stu-id="14d58-155">resource</span></span>|[<span data-ttu-id="14d58-156">governanceResource</span><span class="sxs-lookup"><span data-stu-id="14d58-156">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="14d58-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="14d58-157">Read-only.</span></span> <span data-ttu-id="14d58-158">O recurso associado para a definição de função.</span><span class="sxs-lookup"><span data-stu-id="14d58-158">The associated resource for the role definition.</span></span>|
|<span data-ttu-id="14d58-159">roleSetting</span><span class="sxs-lookup"><span data-stu-id="14d58-159">roleSetting</span></span>|[<span data-ttu-id="14d58-160">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="14d58-160">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)|<span data-ttu-id="14d58-161">A configuração da função associada para a definição de função.</span><span class="sxs-lookup"><span data-stu-id="14d58-161">The associated role setting for the role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="14d58-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="14d58-162">JSON representation</span></span>

<span data-ttu-id="14d58-163">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="14d58-163">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceroledefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
