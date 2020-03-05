---
title: tipo de recurso Entidadegovernanceresource
description: Representa os recursos que podem ser gerenciados pelo gerenciamento de identidade privilegiado (PIM). Para recursos do Azure, pode ser uma assinatura, um grupo de recursos e um recurso como uma máquina virtual, um banco de dados SQL, etc.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 28af0f6ca55881bd0f0848cda27cfe56bd1d5eb5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497612"
---
# <a name="governanceresource-resource-type"></a><span data-ttu-id="77ec3-104">tipo de recurso Entidadegovernanceresource</span><span class="sxs-lookup"><span data-stu-id="77ec3-104">governanceResource resource type</span></span>

<span data-ttu-id="77ec3-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="77ec3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77ec3-106">Representa os recursos que podem ser gerenciados pelo gerenciamento de identidade privilegiado (PIM).</span><span class="sxs-lookup"><span data-stu-id="77ec3-106">Represents resources that could be managed by Privileged Identity Management (PIM).</span></span> <span data-ttu-id="77ec3-107">Para recursos do Azure, pode ser uma assinatura, um grupo de recursos e um recurso como uma máquina virtual, um banco de dados SQL, etc.</span><span class="sxs-lookup"><span data-stu-id="77ec3-107">For Azure resources, it can be a subscription, a resource group, and a resource such as a virtual machine, a SQL database, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="77ec3-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="77ec3-108">Methods</span></span>

| <span data-ttu-id="77ec3-109">Método</span><span class="sxs-lookup"><span data-stu-id="77ec3-109">Method</span></span>          | <span data-ttu-id="77ec3-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="77ec3-110">Return Type</span></span> |<span data-ttu-id="77ec3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="77ec3-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="77ec3-112">List</span><span class="sxs-lookup"><span data-stu-id="77ec3-112">List</span></span>](../api/governanceresource-list.md) | <span data-ttu-id="77ec3-113">coleção [entidadegovernanceresource](../resources/governanceresource.md)</span><span class="sxs-lookup"><span data-stu-id="77ec3-113">[governanceResource](../resources/governanceresource.md) collection</span></span>|<span data-ttu-id="77ec3-114">Lista uma coleção de recursos aos quais o solicitante tem acesso.</span><span class="sxs-lookup"><span data-stu-id="77ec3-114">List a collection of resources the requestor has access to.</span></span>|
|[<span data-ttu-id="77ec3-115">Get</span><span class="sxs-lookup"><span data-stu-id="77ec3-115">Get</span></span>](../api/governanceresource-get.md) | [<span data-ttu-id="77ec3-116">governanceResource</span><span class="sxs-lookup"><span data-stu-id="77ec3-116">governanceResource</span></span>](../resources/governanceresource.md) |<span data-ttu-id="77ec3-117">Leia as propriedades e as relações de uma entidade de recurso especificada por ID.</span><span class="sxs-lookup"><span data-stu-id="77ec3-117">Read properties and relationships of a resource entity specified by id.</span></span>|
|[<span data-ttu-id="77ec3-118">Registrar</span><span class="sxs-lookup"><span data-stu-id="77ec3-118">Register</span></span>](../api/governanceresource-register.md) | |<span data-ttu-id="77ec3-119">Registre uma assinatura do Azure ou um grupo de gerenciamento não gerenciados no serviço PIM.</span><span class="sxs-lookup"><span data-stu-id="77ec3-119">Register an unmanaged Azure subscription or management group to PIM service.</span></span> |

<span data-ttu-id="77ec3-120">Não `POST`, `PUT`, `PATCH`, `DELETE` há suporte no `roleDefinitions` conjunto de entidades por enquanto.</span><span class="sxs-lookup"><span data-stu-id="77ec3-120">No `POST`, `PUT`, `PATCH`, `DELETE` are supported on `roleDefinitions` entity set for now.</span></span>

## <a name="properties"></a><span data-ttu-id="77ec3-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="77ec3-121">Properties</span></span>
| <span data-ttu-id="77ec3-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77ec3-122">Property</span></span>          |<span data-ttu-id="77ec3-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="77ec3-123">Type</span></span>         |<span data-ttu-id="77ec3-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="77ec3-124">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="77ec3-125">id</span><span class="sxs-lookup"><span data-stu-id="77ec3-125">id</span></span>                 |<span data-ttu-id="77ec3-126">String</span><span class="sxs-lookup"><span data-stu-id="77ec3-126">String</span></span>     |<span data-ttu-id="77ec3-127">A ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="77ec3-127">The id of the resource.</span></span> <span data-ttu-id="77ec3-128">Está no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="77ec3-128">It is in GUID format.</span></span>|
|<span data-ttu-id="77ec3-129">externalId</span><span class="sxs-lookup"><span data-stu-id="77ec3-129">externalId</span></span>           |<span data-ttu-id="77ec3-130">String</span><span class="sxs-lookup"><span data-stu-id="77ec3-130">String</span></span>   |<span data-ttu-id="77ec3-131">A ID externa do recurso, que representa sua ID original no sistema externo.</span><span class="sxs-lookup"><span data-stu-id="77ec3-131">The external id of the resource, representing its original id in the external system.</span></span> <span data-ttu-id="77ec3-132">Por exemplo, a ID externa de um recurso de assinatura pode ser "/subscriptions/c14ae696-5e0c-4E5D-88cc-bef6637737ac".</span><span class="sxs-lookup"><span data-stu-id="77ec3-132">For example, a subscription resource's external id can be "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac".</span></span> |
|<span data-ttu-id="77ec3-133">type</span><span class="sxs-lookup"><span data-stu-id="77ec3-133">type</span></span>               |<span data-ttu-id="77ec3-134">String</span><span class="sxs-lookup"><span data-stu-id="77ec3-134">String</span></span>     |<span data-ttu-id="77ec3-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77ec3-135">Required.</span></span> <span data-ttu-id="77ec3-136">Tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="77ec3-136">Resource type.</span></span> <span data-ttu-id="77ec3-137">Por exemplo, para recursos do Azure, o tipo poderia ser "Subscription", "resourcer", "Microsoft. SQL/Server", etc.</span><span class="sxs-lookup"><span data-stu-id="77ec3-137">For example, for Azure resources, the type could be "Subscription", "ResourceGroup", "Microsoft.Sql/server", etc.</span></span>|
|<span data-ttu-id="77ec3-138">displayName</span><span class="sxs-lookup"><span data-stu-id="77ec3-138">displayName</span></span>        |<span data-ttu-id="77ec3-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77ec3-139">String</span></span>     |<span data-ttu-id="77ec3-140">O nome de exibição do recurso.</span><span class="sxs-lookup"><span data-stu-id="77ec3-140">The display name of the resource.</span></span>|
|<span data-ttu-id="77ec3-141">status</span><span class="sxs-lookup"><span data-stu-id="77ec3-141">status</span></span>             |<span data-ttu-id="77ec3-142">String</span><span class="sxs-lookup"><span data-stu-id="77ec3-142">String</span></span>     |<span data-ttu-id="77ec3-143">O status de um determinado recurso.</span><span class="sxs-lookup"><span data-stu-id="77ec3-143">The status of a given resource.</span></span> <span data-ttu-id="77ec3-144">Por exemplo, ele pode representar se o recurso está bloqueado ou não (valores: `Active` / `Locked`).</span><span class="sxs-lookup"><span data-stu-id="77ec3-144">For example, it could represent whether the resource is locked or not (values: `Active`/`Locked`).</span></span> <span data-ttu-id="77ec3-145">Observação: essa propriedade pode ser estendida no futuro para dar suporte a mais cenários.</span><span class="sxs-lookup"><span data-stu-id="77ec3-145">Note: This property may be extended in the future to support more scenarios.</span></span>|
|<span data-ttu-id="77ec3-146">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="77ec3-146">registeredDateTime</span></span>|<span data-ttu-id="77ec3-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77ec3-147">DateTimeOffset</span></span>      |<span data-ttu-id="77ec3-148">Representa a data e hora em que o recurso é registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="77ec3-148">Represents the date time when the resource is registered in PIM.</span></span>|
|<span data-ttu-id="77ec3-149">registeredRoot</span><span class="sxs-lookup"><span data-stu-id="77ec3-149">registeredRoot</span></span>|<span data-ttu-id="77ec3-150">String</span><span class="sxs-lookup"><span data-stu-id="77ec3-150">String</span></span>      |<span data-ttu-id="77ec3-151">ExternalId do escopo raiz do recurso que é registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="77ec3-151">The externalId of the resource's root scope that is registered in PIM.</span></span> <span data-ttu-id="77ec3-152">O escopo raiz pode ser os recursos pai, avô ou ancestral superior.</span><span class="sxs-lookup"><span data-stu-id="77ec3-152">The root scope can be the parent, grandparent, or higher ancestor resources.</span></span>|
|<span data-ttu-id="77ec3-153">roleAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="77ec3-153">roleAssignmentCount</span></span>|<span data-ttu-id="77ec3-154">Int32</span><span class="sxs-lookup"><span data-stu-id="77ec3-154">Int32</span></span>      |<span data-ttu-id="77ec3-155">Opcional.</span><span class="sxs-lookup"><span data-stu-id="77ec3-155">Optional.</span></span> <span data-ttu-id="77ec3-156">O número de atribuições de função para determinado recurso.</span><span class="sxs-lookup"><span data-stu-id="77ec3-156">The number of role assignments for the given resource.</span></span> <span data-ttu-id="77ec3-157">Para obter a propriedade, explictly use `$select=roleAssignmentCount` na consulta.</span><span class="sxs-lookup"><span data-stu-id="77ec3-157">To get the property, please explictly use `$select=roleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="77ec3-158">roleDefinitionCount</span><span class="sxs-lookup"><span data-stu-id="77ec3-158">roleDefinitionCount</span></span>|<span data-ttu-id="77ec3-159">Int32</span><span class="sxs-lookup"><span data-stu-id="77ec3-159">Int32</span></span>      |<span data-ttu-id="77ec3-160">Opcional.</span><span class="sxs-lookup"><span data-stu-id="77ec3-160">Optional.</span></span> <span data-ttu-id="77ec3-161">O número de definições de função para o recurso especificado.</span><span class="sxs-lookup"><span data-stu-id="77ec3-161">The number of role definitions for the given resource.</span></span> <span data-ttu-id="77ec3-162">Para obter a propriedade, explictly use `$select=roleDefinitionCount` na consulta.</span><span class="sxs-lookup"><span data-stu-id="77ec3-162">To get the property, please explictly use `$select=roleDefinitionCount` in the query.</span></span>|
|<span data-ttu-id="77ec3-163">permissões</span><span class="sxs-lookup"><span data-stu-id="77ec3-163">permissions</span></span>|[<span data-ttu-id="77ec3-164">governancePermission</span><span class="sxs-lookup"><span data-stu-id="77ec3-164">governancePermission</span></span>](../resources/governancepermission.md)      |<span data-ttu-id="77ec3-165">Opcional.</span><span class="sxs-lookup"><span data-stu-id="77ec3-165">Optional.</span></span> <span data-ttu-id="77ec3-166">Ele representa o status do acesso do solicitante ao recurso. Para obter a propriedade, explictly use `$select=permissions` na consulta.</span><span class="sxs-lookup"><span data-stu-id="77ec3-166">It represents the status of the requestor's access to the resource.To get the property, please explictly use `$select=permissions` in the query.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77ec3-167">Relações</span><span class="sxs-lookup"><span data-stu-id="77ec3-167">Relationships</span></span>
| <span data-ttu-id="77ec3-168">Relação</span><span class="sxs-lookup"><span data-stu-id="77ec3-168">Relationship</span></span>   | <span data-ttu-id="77ec3-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="77ec3-169">Type</span></span>                                         |<span data-ttu-id="77ec3-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="77ec3-170">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="77ec3-171">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="77ec3-171">roleAssignments</span></span> |<span data-ttu-id="77ec3-172">coleção [governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="77ec3-172">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="77ec3-173">A coleção de atribuições de função para o recurso.</span><span class="sxs-lookup"><span data-stu-id="77ec3-173">The collection of role assignments for the resource.</span></span>|
|<span data-ttu-id="77ec3-174">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="77ec3-174">roleDefinitions</span></span> |<span data-ttu-id="77ec3-175">coleção [governanceRoleDefinition](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="77ec3-175">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="77ec3-176">O conjunto de defintions de função para o recurso.</span><span class="sxs-lookup"><span data-stu-id="77ec3-176">The collection of role defintions for the resource.</span></span>|
|<span data-ttu-id="77ec3-177">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="77ec3-177">roleAssignmentRequests</span></span> |<span data-ttu-id="77ec3-178">coleção [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="77ec3-178">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="77ec3-179">A coleção de solicitações de atribuição de função para o recurso.</span><span class="sxs-lookup"><span data-stu-id="77ec3-179">The collection of role assignment requests for the resource.</span></span>|
|<span data-ttu-id="77ec3-180">roleSettings</span><span class="sxs-lookup"><span data-stu-id="77ec3-180">roleSettings</span></span> |<span data-ttu-id="77ec3-181">coleção [governanceRoleSetting](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="77ec3-181">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="77ec3-182">O conjunto de configurações de função para o recurso.</span><span class="sxs-lookup"><span data-stu-id="77ec3-182">The collection of role settings for the resource.</span></span>|
|<span data-ttu-id="77ec3-183">primário</span><span class="sxs-lookup"><span data-stu-id="77ec3-183">parent</span></span>          |[<span data-ttu-id="77ec3-184">governanceResource</span><span class="sxs-lookup"><span data-stu-id="77ec3-184">governanceResource</span></span>](../resources/governanceresource.md)           |<span data-ttu-id="77ec3-185">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="77ec3-185">Read-only.</span></span> <span data-ttu-id="77ec3-186">O recurso pai.</span><span class="sxs-lookup"><span data-stu-id="77ec3-186">The parent resource.</span></span> <span data-ttu-id="77ec3-187">para `pimforazurerbac` o cenário, ele pode representar a assinatura à qual o recurso pertence.</span><span class="sxs-lookup"><span data-stu-id="77ec3-187">for `pimforazurerbac` scenario, it can represent the subscription the resource belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="77ec3-188">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="77ec3-188">JSON representation</span></span>

<span data-ttu-id="77ec3-189">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="77ec3-189">The following is a JSON representation of the resource.</span></span>

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
