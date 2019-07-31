---
title: tipo de recurso Entidadegovernanceresource
description: Representa os recursos que podem ser gerenciados pelo gerenciamento de identidade privilegiado (PIM). Para recursos do Azure, pode ser uma assinatura, um grupo de recursos e um recurso como uma máquina virtual, um banco de dados SQL, etc.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: a0429de2cacc816eaf1a603a29a08897650da6e2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971918"
---
# <a name="governanceresource-resource-type"></a><span data-ttu-id="566eb-104">tipo de recurso Entidadegovernanceresource</span><span class="sxs-lookup"><span data-stu-id="566eb-104">governanceResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="566eb-105">Representa os recursos que podem ser gerenciados pelo gerenciamento de identidade privilegiado (PIM).</span><span class="sxs-lookup"><span data-stu-id="566eb-105">Represents resources that could be managed by Privileged Identity Management (PIM).</span></span> <span data-ttu-id="566eb-106">Para recursos do Azure, pode ser uma assinatura, um grupo de recursos e um recurso como uma máquina virtual, um banco de dados SQL, etc.</span><span class="sxs-lookup"><span data-stu-id="566eb-106">For Azure resources, it can be a subscription, a resource group, and a resource such as a virtual machine, a SQL database, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="566eb-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="566eb-107">Methods</span></span>

| <span data-ttu-id="566eb-108">Método</span><span class="sxs-lookup"><span data-stu-id="566eb-108">Method</span></span>          | <span data-ttu-id="566eb-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="566eb-109">Return Type</span></span> |<span data-ttu-id="566eb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="566eb-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="566eb-111">List</span><span class="sxs-lookup"><span data-stu-id="566eb-111">List</span></span>](../api/governanceresource-list.md) | <span data-ttu-id="566eb-112">coleção [entidadegovernanceresource](../resources/governanceresource.md)</span><span class="sxs-lookup"><span data-stu-id="566eb-112">[governanceResource](../resources/governanceresource.md) collection</span></span>|<span data-ttu-id="566eb-113">Lista uma coleção de recursos aos quais o solicitante tem acesso.</span><span class="sxs-lookup"><span data-stu-id="566eb-113">List a collection of resources the requestor has access to.</span></span>|
|[<span data-ttu-id="566eb-114">Get</span><span class="sxs-lookup"><span data-stu-id="566eb-114">Get</span></span>](../api/governanceresource-get.md) | [<span data-ttu-id="566eb-115">Entidadegovernanceresource</span><span class="sxs-lookup"><span data-stu-id="566eb-115">governanceResource</span></span>](../resources/governanceresource.md) |<span data-ttu-id="566eb-116">Leia as propriedades e as relações de uma entidade de recurso especificada por ID.</span><span class="sxs-lookup"><span data-stu-id="566eb-116">Read properties and relationships of a resource entity specified by id.</span></span>|
|[<span data-ttu-id="566eb-117">Registrar</span><span class="sxs-lookup"><span data-stu-id="566eb-117">Register</span></span>](../api/governanceresource-register.md) | |<span data-ttu-id="566eb-118">Registre uma assinatura do Azure ou um grupo de gerenciamento não gerenciados no serviço PIM.</span><span class="sxs-lookup"><span data-stu-id="566eb-118">Register an unmanaged Azure subscription or management group to PIM service.</span></span> |

<span data-ttu-id="566eb-119">Não `POST`, `PUT`, `PATCH`, `DELETE` há suporte no `roleDefinitions` conjunto de entidades por enquanto.</span><span class="sxs-lookup"><span data-stu-id="566eb-119">No `POST`, `PUT`, `PATCH`, `DELETE` are supported on `roleDefinitions` entity set for now.</span></span>

## <a name="properties"></a><span data-ttu-id="566eb-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="566eb-120">Properties</span></span>
| <span data-ttu-id="566eb-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="566eb-121">Property</span></span>          |<span data-ttu-id="566eb-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="566eb-122">Type</span></span>         |<span data-ttu-id="566eb-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="566eb-123">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="566eb-124">id</span><span class="sxs-lookup"><span data-stu-id="566eb-124">id</span></span>                 |<span data-ttu-id="566eb-125">String</span><span class="sxs-lookup"><span data-stu-id="566eb-125">String</span></span>     |<span data-ttu-id="566eb-126">A ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="566eb-126">The id of the resource.</span></span> <span data-ttu-id="566eb-127">Está no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="566eb-127">It is in GUID format.</span></span>|
|<span data-ttu-id="566eb-128">externalId</span><span class="sxs-lookup"><span data-stu-id="566eb-128">externalId</span></span>           |<span data-ttu-id="566eb-129">String</span><span class="sxs-lookup"><span data-stu-id="566eb-129">String</span></span>   |<span data-ttu-id="566eb-130">A ID externa do recurso, que representa sua ID original no sistema externo.</span><span class="sxs-lookup"><span data-stu-id="566eb-130">The external id of the resource, representing its original id in the external system.</span></span> <span data-ttu-id="566eb-131">Por exemplo, a ID externa de um recurso de assinatura pode ser "/subscriptions/c14ae696-5e0c-4E5D-88cc-bef6637737ac".</span><span class="sxs-lookup"><span data-stu-id="566eb-131">For example, a subscription resource's external id can be "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac".</span></span> |
|<span data-ttu-id="566eb-132">type</span><span class="sxs-lookup"><span data-stu-id="566eb-132">type</span></span>               |<span data-ttu-id="566eb-133">String</span><span class="sxs-lookup"><span data-stu-id="566eb-133">String</span></span>     |<span data-ttu-id="566eb-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="566eb-134">Required.</span></span> <span data-ttu-id="566eb-135">Tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="566eb-135">Resource type.</span></span> <span data-ttu-id="566eb-136">Por exemplo, para recursos do Azure, o tipo poderia ser "Subscription", "resourcer", "Microsoft. SQL/Server", etc.</span><span class="sxs-lookup"><span data-stu-id="566eb-136">For example, for Azure resources, the type could be "Subscription", "ResourceGroup", "Microsoft.Sql/server", etc.</span></span>|
|<span data-ttu-id="566eb-137">displayName</span><span class="sxs-lookup"><span data-stu-id="566eb-137">displayName</span></span>        |<span data-ttu-id="566eb-138">String</span><span class="sxs-lookup"><span data-stu-id="566eb-138">String</span></span>     |<span data-ttu-id="566eb-139">O nome de exibição do recurso.</span><span class="sxs-lookup"><span data-stu-id="566eb-139">The display name of the resource.</span></span>|
|<span data-ttu-id="566eb-140">status</span><span class="sxs-lookup"><span data-stu-id="566eb-140">status</span></span>             |<span data-ttu-id="566eb-141">String</span><span class="sxs-lookup"><span data-stu-id="566eb-141">String</span></span>     |<span data-ttu-id="566eb-142">O status de um determinado recurso.</span><span class="sxs-lookup"><span data-stu-id="566eb-142">The status of a given resource.</span></span> <span data-ttu-id="566eb-143">Por exemplo, ele pode representar se o recurso está bloqueado ou não (valores: `Active` / `Locked`).</span><span class="sxs-lookup"><span data-stu-id="566eb-143">For example, it could represent whether the resource is locked or not (values: `Active`/`Locked`).</span></span> <span data-ttu-id="566eb-144">Observação: essa propriedade pode ser estendida no futuro para dar suporte a mais cenários.</span><span class="sxs-lookup"><span data-stu-id="566eb-144">Note: This property may be extended in the future to support more scenarios.</span></span>|
|<span data-ttu-id="566eb-145">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="566eb-145">registeredDateTime</span></span>|<span data-ttu-id="566eb-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="566eb-146">DateTimeOffset</span></span>      |<span data-ttu-id="566eb-147">Representa a data e hora em que o recurso é registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="566eb-147">Represents the date time when the resource is registered in PIM.</span></span>|
|<span data-ttu-id="566eb-148">registeredRoot</span><span class="sxs-lookup"><span data-stu-id="566eb-148">registeredRoot</span></span>|<span data-ttu-id="566eb-149">String</span><span class="sxs-lookup"><span data-stu-id="566eb-149">String</span></span>      |<span data-ttu-id="566eb-150">ExternalId do escopo raiz do recurso que é registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="566eb-150">The externalId of the resource's root scope that is registered in PIM.</span></span> <span data-ttu-id="566eb-151">O escopo raiz pode ser os recursos pai, avô ou ancestral superior.</span><span class="sxs-lookup"><span data-stu-id="566eb-151">The root scope can be the parent, grandparent, or higher ancestor resources.</span></span>|
|<span data-ttu-id="566eb-152">roleAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="566eb-152">roleAssignmentCount</span></span>|<span data-ttu-id="566eb-153">Int32</span><span class="sxs-lookup"><span data-stu-id="566eb-153">Int32</span></span>      |<span data-ttu-id="566eb-154">Opcional.</span><span class="sxs-lookup"><span data-stu-id="566eb-154">Optional.</span></span> <span data-ttu-id="566eb-155">O número de atribuições de função para determinado recurso.</span><span class="sxs-lookup"><span data-stu-id="566eb-155">The number of role assignments for the given resource.</span></span> <span data-ttu-id="566eb-156">Para obter a propriedade, explictly use `$select=roleAssignmentCount` na consulta.</span><span class="sxs-lookup"><span data-stu-id="566eb-156">To get the property, please explictly use `$select=roleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="566eb-157">roleDefinitionCount</span><span class="sxs-lookup"><span data-stu-id="566eb-157">roleDefinitionCount</span></span>|<span data-ttu-id="566eb-158">Int32</span><span class="sxs-lookup"><span data-stu-id="566eb-158">Int32</span></span>      |<span data-ttu-id="566eb-159">Opcional.</span><span class="sxs-lookup"><span data-stu-id="566eb-159">Optional.</span></span> <span data-ttu-id="566eb-160">O número de definições de função para o recurso especificado.</span><span class="sxs-lookup"><span data-stu-id="566eb-160">The number of role definitions for the given resource.</span></span> <span data-ttu-id="566eb-161">Para obter a propriedade, explictly use `$select=roleDefinitionCount` na consulta.</span><span class="sxs-lookup"><span data-stu-id="566eb-161">To get the property, please explictly use `$select=roleDefinitionCount` in the query.</span></span>|
|<span data-ttu-id="566eb-162">permissões</span><span class="sxs-lookup"><span data-stu-id="566eb-162">permissions</span></span>|[<span data-ttu-id="566eb-163">governancePermission</span><span class="sxs-lookup"><span data-stu-id="566eb-163">governancePermission</span></span>](../resources/governancepermission.md)      |<span data-ttu-id="566eb-164">Opcional.</span><span class="sxs-lookup"><span data-stu-id="566eb-164">Optional.</span></span> <span data-ttu-id="566eb-165">Ele representa o status do acesso do solicitante ao recurso. Para obter a propriedade, explictly use `$select=permissions` na consulta.</span><span class="sxs-lookup"><span data-stu-id="566eb-165">It represents the status of the requestor's access to the resource.To get the property, please explictly use `$select=permissions` in the query.</span></span>|

## <a name="relationships"></a><span data-ttu-id="566eb-166">Relações</span><span class="sxs-lookup"><span data-stu-id="566eb-166">Relationships</span></span>
| <span data-ttu-id="566eb-167">Relação</span><span class="sxs-lookup"><span data-stu-id="566eb-167">Relationship</span></span>   | <span data-ttu-id="566eb-168">Tipo</span><span class="sxs-lookup"><span data-stu-id="566eb-168">Type</span></span>                                         |<span data-ttu-id="566eb-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="566eb-169">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="566eb-170">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="566eb-170">roleAssignments</span></span> |<span data-ttu-id="566eb-171">coleção [governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="566eb-171">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="566eb-172">A coleção de atribuições de função para o recurso.</span><span class="sxs-lookup"><span data-stu-id="566eb-172">The collection of role assignments for the resource.</span></span>|
|<span data-ttu-id="566eb-173">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="566eb-173">roleDefinitions</span></span> |<span data-ttu-id="566eb-174">coleção [governanceRoleDefinition](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="566eb-174">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="566eb-175">O conjunto de defintions de função para o recurso.</span><span class="sxs-lookup"><span data-stu-id="566eb-175">The collection of role defintions for the resource.</span></span>|
|<span data-ttu-id="566eb-176">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="566eb-176">roleAssignmentRequests</span></span> |<span data-ttu-id="566eb-177">coleção [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="566eb-177">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="566eb-178">A coleção de solicitações de atribuição de função para o recurso.</span><span class="sxs-lookup"><span data-stu-id="566eb-178">The collection of role assignment requests for the resource.</span></span>|
|<span data-ttu-id="566eb-179">roleSettings</span><span class="sxs-lookup"><span data-stu-id="566eb-179">roleSettings</span></span> |<span data-ttu-id="566eb-180">coleção [governanceRoleSetting](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="566eb-180">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="566eb-181">O conjunto de configurações de função para o recurso.</span><span class="sxs-lookup"><span data-stu-id="566eb-181">The collection of role settings for the resource.</span></span>|
|<span data-ttu-id="566eb-182">primário</span><span class="sxs-lookup"><span data-stu-id="566eb-182">parent</span></span>          |[<span data-ttu-id="566eb-183">Entidadegovernanceresource</span><span class="sxs-lookup"><span data-stu-id="566eb-183">governanceResource</span></span>](../resources/governanceresource.md)           |<span data-ttu-id="566eb-184">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="566eb-184">Read-only.</span></span> <span data-ttu-id="566eb-185">O recurso pai.</span><span class="sxs-lookup"><span data-stu-id="566eb-185">The parent resource.</span></span> <span data-ttu-id="566eb-186">para `pimforazurerbac` o cenário, ele pode representar a assinatura à qual o recurso pertence.</span><span class="sxs-lookup"><span data-stu-id="566eb-186">for `pimforazurerbac` scenario, it can represent the subscription the resource belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="566eb-187">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="566eb-187">JSON representation</span></span>

<span data-ttu-id="566eb-188">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="566eb-188">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceResource"
}-->
```json
{
  "id": "String (identifier)",
  "externalId": "String",
  "type": "String",
  "displayName": "String",
  "status": "String",
  "registeredDateTime": "String (timestamp)",
  "registeredRoot": "String",
  "roleAssignmentCount": 12356,
  "roleDefinitionCount": 12356,
  "permissions": {
    "@odata.type": "microsoft.graph.governancePermission"
  }
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
