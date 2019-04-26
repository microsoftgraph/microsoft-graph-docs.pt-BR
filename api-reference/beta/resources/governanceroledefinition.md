---
title: tipo de recurso governanceRoleDefinition
description: Representa as definições de função. Para os recursos do Azure, ele pode representar as funções do Azure RBAC, como proprietário, leitor, colaborador, etc.
localization_priority: Normal
ms.openlocfilehash: 867864892bac9107c44ba9125336429248b6697e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547437"
---
# <a name="governanceroledefinition-resource-type"></a><span data-ttu-id="2adde-104">tipo de recurso governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="2adde-104">governanceRoleDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="2adde-105">Representa as definições de função.</span><span class="sxs-lookup"><span data-stu-id="2adde-105">Represents the role definitions.</span></span> <span data-ttu-id="2adde-106">Para os recursos do Azure, ele pode representar as funções do Azure RBAC, como proprietário, leitor, colaborador, etc.</span><span class="sxs-lookup"><span data-stu-id="2adde-106">For Azure resources, it can represent Azure RBAC roles, such as Owner, Reader, Contributor, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="2adde-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="2adde-107">Methods</span></span>

| <span data-ttu-id="2adde-108">Método</span><span class="sxs-lookup"><span data-stu-id="2adde-108">Method</span></span>          | <span data-ttu-id="2adde-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2adde-109">Return Type</span></span> |<span data-ttu-id="2adde-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2adde-110">Description</span></span>|
|:---------------|:--------|:--------|:----------|
|[<span data-ttu-id="2adde-111">List</span><span class="sxs-lookup"><span data-stu-id="2adde-111">List</span></span>](../api/governanceroledefinition-list.md) | <span data-ttu-id="2adde-112">coleção [governanceRoleDefinition](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2adde-112">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span> |<span data-ttu-id="2adde-113">Lista uma coleção de definições de função em um recurso.</span><span class="sxs-lookup"><span data-stu-id="2adde-113">List a collection of role definitions on a resource.</span></span>|
|[<span data-ttu-id="2adde-114">Get</span><span class="sxs-lookup"><span data-stu-id="2adde-114">Get</span></span>](../api/governanceroledefinition-get.md) | [<span data-ttu-id="2adde-115">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="2adde-115">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md) |<span data-ttu-id="2adde-116">Ler propriedades e relações de uma entidade de definição de função especificado por ID.</span><span class="sxs-lookup"><span data-stu-id="2adde-116">Read properties and relationships of a role definition entity specified by id.</span></span>|
<span data-ttu-id="2adde-117">Não `POST`, `PUT`, `PATCH`, `DELETE` tem suporte no `roleDefinitions` conjunto de entidades por enquanto.</span><span class="sxs-lookup"><span data-stu-id="2adde-117">No `POST`, `PUT`, `PATCH`, `DELETE` is supported on `roleDefinitions` entity set for now.</span></span>
## <a name="properties"></a><span data-ttu-id="2adde-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2adde-118">Properties</span></span>
| <span data-ttu-id="2adde-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2adde-119">Property</span></span>  | <span data-ttu-id="2adde-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="2adde-120">Type</span></span>      |<span data-ttu-id="2adde-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="2adde-121">Description</span></span>|
|:----|:----------|:----------|:----------|
|<span data-ttu-id="2adde-122">id</span><span class="sxs-lookup"><span data-stu-id="2adde-122">id</span></span>         |<span data-ttu-id="2adde-123">String</span><span class="sxs-lookup"><span data-stu-id="2adde-123">String</span></span>     |<span data-ttu-id="2adde-124">A ID da definição de função.</span><span class="sxs-lookup"><span data-stu-id="2adde-124">The id of the role definition.</span></span> |
|<span data-ttu-id="2adde-125">resourceId</span><span class="sxs-lookup"><span data-stu-id="2adde-125">resourceId</span></span> |<span data-ttu-id="2adde-126">String</span><span class="sxs-lookup"><span data-stu-id="2adde-126">String</span></span>     |<span data-ttu-id="2adde-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2adde-127">Required.</span></span> <span data-ttu-id="2adde-128">A ID do recurso associada à definição de função.</span><span class="sxs-lookup"><span data-stu-id="2adde-128">The id of the resource associated with the role definition.</span></span> |
|<span data-ttu-id="2adde-129">externalId</span><span class="sxs-lookup"><span data-stu-id="2adde-129">externalId</span></span>   |<span data-ttu-id="2adde-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2adde-130">String</span></span>     |<span data-ttu-id="2adde-131">A ID externa da definição de função.</span><span class="sxs-lookup"><span data-stu-id="2adde-131">The external id of the role definition.</span></span>|
|<span data-ttu-id="2adde-132">displayName</span><span class="sxs-lookup"><span data-stu-id="2adde-132">displayName</span></span>|<span data-ttu-id="2adde-133">String</span><span class="sxs-lookup"><span data-stu-id="2adde-133">String</span></span>     |<span data-ttu-id="2adde-134">O nome de exibição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="2adde-134">The display name of the role definition.</span></span>|
|<span data-ttu-id="2adde-135">subjectCount</span><span class="sxs-lookup"><span data-stu-id="2adde-135">subjectCount</span></span>|<span data-ttu-id="2adde-136">Int32</span><span class="sxs-lookup"><span data-stu-id="2adde-136">Int32</span></span>     |<span data-ttu-id="2adde-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="2adde-137">Optional.</span></span> <span data-ttu-id="2adde-138">O número de entidades atribuídas à função.</span><span class="sxs-lookup"><span data-stu-id="2adde-138">The number of subjects that are assigned to the role.</span></span> <span data-ttu-id="2adde-139">Ele representa o status do acesso do solicitante ao recurso.</span><span class="sxs-lookup"><span data-stu-id="2adde-139">It represents the status of the requestor's access to the resource.</span></span> <span data-ttu-id="2adde-140">Para obter a propriedade, explictly use `$select=subjectCount` na consulta.</span><span class="sxs-lookup"><span data-stu-id="2adde-140">To get the property, please explictly use `$select=subjectCount` in the query.</span></span>|
|<span data-ttu-id="2adde-141">eligibleAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="2adde-141">eligibleAssignmentCount</span></span>|<span data-ttu-id="2adde-142">Int32</span><span class="sxs-lookup"><span data-stu-id="2adde-142">Int32</span></span>|<span data-ttu-id="2adde-143">Opcional.</span><span class="sxs-lookup"><span data-stu-id="2adde-143">Optional.</span></span> <span data-ttu-id="2adde-144">O número de atribuições de função qualificadas associadas à definição de função.</span><span class="sxs-lookup"><span data-stu-id="2adde-144">The number of eligible role assignments associated with the role definition.</span></span> <span data-ttu-id="2adde-145">Para obter a propriedade, explictly use `$select=eligibleAssignmentCount` na consulta.</span><span class="sxs-lookup"><span data-stu-id="2adde-145">To get the property, please explictly use `$select=eligibleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="2adde-146">activeAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="2adde-146">activeAssignmentCount</span></span>|<span data-ttu-id="2adde-147">Int32</span><span class="sxs-lookup"><span data-stu-id="2adde-147">Int32</span></span>    |<span data-ttu-id="2adde-148">Opcional.</span><span class="sxs-lookup"><span data-stu-id="2adde-148">Optional.</span></span> <span data-ttu-id="2adde-149">O número de atribuições de função ativas associadas à definição de função.</span><span class="sxs-lookup"><span data-stu-id="2adde-149">The number of active role assignments associated with the role definition.</span></span>  <span data-ttu-id="2adde-150">Para obter a propriedade, explictly use `$select=activeAssignmentCount` na consulta.</span><span class="sxs-lookup"><span data-stu-id="2adde-150">To get the property, please explictly use `$select=activeAssignmentCount` in the query.</span></span>|


## <a name="relationships"></a><span data-ttu-id="2adde-151">Relações</span><span class="sxs-lookup"><span data-stu-id="2adde-151">Relationships</span></span>
| <span data-ttu-id="2adde-152">Relação</span><span class="sxs-lookup"><span data-stu-id="2adde-152">Relationship</span></span> | <span data-ttu-id="2adde-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="2adde-153">Type</span></span>   |<span data-ttu-id="2adde-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="2adde-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2adde-155">recurso</span><span class="sxs-lookup"><span data-stu-id="2adde-155">resource</span></span>|[<span data-ttu-id="2adde-156">Entidadegovernanceresource</span><span class="sxs-lookup"><span data-stu-id="2adde-156">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="2adde-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2adde-157">Read-only.</span></span> <span data-ttu-id="2adde-158">O recurso associado para a definição de função.</span><span class="sxs-lookup"><span data-stu-id="2adde-158">The associated resource for the role definition.</span></span>|
|<span data-ttu-id="2adde-159">roleSetting</span><span class="sxs-lookup"><span data-stu-id="2adde-159">roleSetting</span></span>|[<span data-ttu-id="2adde-160">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="2adde-160">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)|<span data-ttu-id="2adde-161">A configuração de função associada para a definição de função.</span><span class="sxs-lookup"><span data-stu-id="2adde-161">The associated role setting for the role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2adde-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2adde-162">JSON representation</span></span>

<span data-ttu-id="2adde-163">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2adde-163">Here is a JSON representation of the resource.</span></span>

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
