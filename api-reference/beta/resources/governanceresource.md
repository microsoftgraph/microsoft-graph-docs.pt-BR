---
title: Tipo de recurso governanceResource
description: Representa recursos que podem ser gerenciados pelo PIM (Privileged Identity Management). Para recursos do Azure, pode ser uma assinatura, um grupo de recursos e um recurso, como uma máquina virtual, um banco de dados SQL, etc.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: e0cf42593a35103996217d1ce18bd9938b48a185
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443108"
---
# <a name="governanceresource-resource-type"></a><span data-ttu-id="16b9a-104">Tipo de recurso governanceResource</span><span class="sxs-lookup"><span data-stu-id="16b9a-104">governanceResource resource type</span></span>

<span data-ttu-id="16b9a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16b9a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16b9a-106">Representa recursos que podem ser gerenciados pelo PIM (Privileged Identity Management).</span><span class="sxs-lookup"><span data-stu-id="16b9a-106">Represents resources that could be managed by Privileged Identity Management (PIM).</span></span> <span data-ttu-id="16b9a-107">Para recursos do Azure, pode ser uma assinatura, um grupo de recursos e um recurso, como uma máquina virtual, um banco de dados SQL, etc.</span><span class="sxs-lookup"><span data-stu-id="16b9a-107">For Azure resources, it can be a subscription, a resource group, and a resource such as a virtual machine, a SQL database, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="16b9a-108">Methods</span><span class="sxs-lookup"><span data-stu-id="16b9a-108">Methods</span></span>

| <span data-ttu-id="16b9a-109">Método</span><span class="sxs-lookup"><span data-stu-id="16b9a-109">Method</span></span>          | <span data-ttu-id="16b9a-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="16b9a-110">Return Type</span></span> |<span data-ttu-id="16b9a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="16b9a-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="16b9a-112">List</span><span class="sxs-lookup"><span data-stu-id="16b9a-112">List</span></span>](../api/governanceresource-list.md) | <span data-ttu-id="16b9a-113">[Coleção governanceResource](../resources/governanceresource.md)</span><span class="sxs-lookup"><span data-stu-id="16b9a-113">[governanceResource](../resources/governanceresource.md) collection</span></span>|<span data-ttu-id="16b9a-114">Listar uma coleção de recursos aos que o solicitante tem acesso.</span><span class="sxs-lookup"><span data-stu-id="16b9a-114">List a collection of resources the requestor has access to.</span></span>|
|[<span data-ttu-id="16b9a-115">Get</span><span class="sxs-lookup"><span data-stu-id="16b9a-115">Get</span></span>](../api/governanceresource-get.md) | [<span data-ttu-id="16b9a-116">governanceResource</span><span class="sxs-lookup"><span data-stu-id="16b9a-116">governanceResource</span></span>](../resources/governanceresource.md) |<span data-ttu-id="16b9a-117">Ler propriedades e relações de uma entidade de recurso especificada por id.</span><span class="sxs-lookup"><span data-stu-id="16b9a-117">Read properties and relationships of a resource entity specified by id.</span></span>|
|[<span data-ttu-id="16b9a-118">Registrar</span><span class="sxs-lookup"><span data-stu-id="16b9a-118">Register</span></span>](../api/governanceresource-register.md) | |<span data-ttu-id="16b9a-119">Registre uma assinatura ou grupo de gerenciamento não gerenciada do Azure no serviço PIM.</span><span class="sxs-lookup"><span data-stu-id="16b9a-119">Register an unmanaged Azure subscription or management group to PIM service.</span></span> |

<span data-ttu-id="16b9a-120">Não `POST` , , são `PUT` `PATCH` `DELETE` suportados no conjunto de `roleDefinitions` entidades por enquanto.</span><span class="sxs-lookup"><span data-stu-id="16b9a-120">No `POST`, `PUT`, `PATCH`, `DELETE` are supported on `roleDefinitions` entity set for now.</span></span>

## <a name="properties"></a><span data-ttu-id="16b9a-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="16b9a-121">Properties</span></span>
| <span data-ttu-id="16b9a-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16b9a-122">Property</span></span>          |<span data-ttu-id="16b9a-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="16b9a-123">Type</span></span>         |<span data-ttu-id="16b9a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="16b9a-124">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="16b9a-125">id</span><span class="sxs-lookup"><span data-stu-id="16b9a-125">id</span></span>                 |<span data-ttu-id="16b9a-126">String</span><span class="sxs-lookup"><span data-stu-id="16b9a-126">String</span></span>     |<span data-ttu-id="16b9a-127">A id do recurso.</span><span class="sxs-lookup"><span data-stu-id="16b9a-127">The id of the resource.</span></span> <span data-ttu-id="16b9a-128">Está no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="16b9a-128">It is in GUID format.</span></span>|
|<span data-ttu-id="16b9a-129">externalId</span><span class="sxs-lookup"><span data-stu-id="16b9a-129">externalId</span></span>           |<span data-ttu-id="16b9a-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16b9a-130">String</span></span>   |<span data-ttu-id="16b9a-131">A id externa do recurso, representando sua id original no sistema externo.</span><span class="sxs-lookup"><span data-stu-id="16b9a-131">The external id of the resource, representing its original id in the external system.</span></span> <span data-ttu-id="16b9a-132">Por exemplo, a ID externa de um recurso de assinatura pode ser "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac".</span><span class="sxs-lookup"><span data-stu-id="16b9a-132">For example, a subscription resource's external id can be "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac".</span></span> |
|<span data-ttu-id="16b9a-133">type</span><span class="sxs-lookup"><span data-stu-id="16b9a-133">type</span></span>               |<span data-ttu-id="16b9a-134">String</span><span class="sxs-lookup"><span data-stu-id="16b9a-134">String</span></span>     |<span data-ttu-id="16b9a-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16b9a-135">Required.</span></span> <span data-ttu-id="16b9a-136">Tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="16b9a-136">Resource type.</span></span> <span data-ttu-id="16b9a-137">Por exemplo, para recursos do Azure, o tipo pode ser "Subscription", "ResourceGroup", "Microsoft.Sql/server", etc.</span><span class="sxs-lookup"><span data-stu-id="16b9a-137">For example, for Azure resources, the type could be "Subscription", "ResourceGroup", "Microsoft.Sql/server", etc.</span></span>|
|<span data-ttu-id="16b9a-138">displayName</span><span class="sxs-lookup"><span data-stu-id="16b9a-138">displayName</span></span>        |<span data-ttu-id="16b9a-139">String</span><span class="sxs-lookup"><span data-stu-id="16b9a-139">String</span></span>     |<span data-ttu-id="16b9a-140">O nome de exibição do recurso.</span><span class="sxs-lookup"><span data-stu-id="16b9a-140">The display name of the resource.</span></span>|
|<span data-ttu-id="16b9a-141">status</span><span class="sxs-lookup"><span data-stu-id="16b9a-141">status</span></span>             |<span data-ttu-id="16b9a-142">String</span><span class="sxs-lookup"><span data-stu-id="16b9a-142">String</span></span>     |<span data-ttu-id="16b9a-143">O status de um determinado recurso.</span><span class="sxs-lookup"><span data-stu-id="16b9a-143">The status of a given resource.</span></span> <span data-ttu-id="16b9a-144">Por exemplo, ele pode representar se o recurso está bloqueado ou não (valores: `Active` / `Locked` ).</span><span class="sxs-lookup"><span data-stu-id="16b9a-144">For example, it could represent whether the resource is locked or not (values: `Active`/`Locked`).</span></span> <span data-ttu-id="16b9a-145">Observação: essa propriedade pode ser estendida no futuro para dar suporte a mais cenários.</span><span class="sxs-lookup"><span data-stu-id="16b9a-145">Note: This property may be extended in the future to support more scenarios.</span></span>|
|<span data-ttu-id="16b9a-146">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="16b9a-146">registeredDateTime</span></span>|<span data-ttu-id="16b9a-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16b9a-147">DateTimeOffset</span></span>      |<span data-ttu-id="16b9a-148">Representa a data em que o recurso é registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="16b9a-148">Represents the date time when the resource is registered in PIM.</span></span>|
|<span data-ttu-id="16b9a-149">registeredRoot</span><span class="sxs-lookup"><span data-stu-id="16b9a-149">registeredRoot</span></span>|<span data-ttu-id="16b9a-150">String</span><span class="sxs-lookup"><span data-stu-id="16b9a-150">String</span></span>      |<span data-ttu-id="16b9a-151">O externalId do escopo raiz do recurso que está registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="16b9a-151">The externalId of the resource's root scope that is registered in PIM.</span></span> <span data-ttu-id="16b9a-152">O escopo raiz pode ser o pai, o vôrent ou recursos ancestrais superiores.</span><span class="sxs-lookup"><span data-stu-id="16b9a-152">The root scope can be the parent, grandparent, or higher ancestor resources.</span></span>|
|<span data-ttu-id="16b9a-153">roleAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="16b9a-153">roleAssignmentCount</span></span>|<span data-ttu-id="16b9a-154">Int32</span><span class="sxs-lookup"><span data-stu-id="16b9a-154">Int32</span></span>      |<span data-ttu-id="16b9a-155">Opcional.</span><span class="sxs-lookup"><span data-stu-id="16b9a-155">Optional.</span></span> <span data-ttu-id="16b9a-156">O número de atribuições de função para o recurso determinado.</span><span class="sxs-lookup"><span data-stu-id="16b9a-156">The number of role assignments for the given resource.</span></span> <span data-ttu-id="16b9a-157">Para obter a propriedade, use explictly `$select=roleAssignmentCount` na consulta.</span><span class="sxs-lookup"><span data-stu-id="16b9a-157">To get the property, please explictly use `$select=roleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="16b9a-158">roleDefinitionCount</span><span class="sxs-lookup"><span data-stu-id="16b9a-158">roleDefinitionCount</span></span>|<span data-ttu-id="16b9a-159">Int32</span><span class="sxs-lookup"><span data-stu-id="16b9a-159">Int32</span></span>      |<span data-ttu-id="16b9a-160">Opcional.</span><span class="sxs-lookup"><span data-stu-id="16b9a-160">Optional.</span></span> <span data-ttu-id="16b9a-161">O número de definições de função para o determinado recurso.</span><span class="sxs-lookup"><span data-stu-id="16b9a-161">The number of role definitions for the given resource.</span></span> <span data-ttu-id="16b9a-162">Para obter a propriedade, use explictly `$select=roleDefinitionCount` na consulta.</span><span class="sxs-lookup"><span data-stu-id="16b9a-162">To get the property, please explictly use `$select=roleDefinitionCount` in the query.</span></span>|
|<span data-ttu-id="16b9a-163">permissões</span><span class="sxs-lookup"><span data-stu-id="16b9a-163">permissions</span></span>|[<span data-ttu-id="16b9a-164">governancePermission</span><span class="sxs-lookup"><span data-stu-id="16b9a-164">governancePermission</span></span>](../resources/governancepermission.md)      |<span data-ttu-id="16b9a-165">Opcional.</span><span class="sxs-lookup"><span data-stu-id="16b9a-165">Optional.</span></span> <span data-ttu-id="16b9a-166">Ele representa o status do acesso do solicitante ao recurso. Para obter a propriedade, use explictly `$select=permissions` na consulta.</span><span class="sxs-lookup"><span data-stu-id="16b9a-166">It represents the status of the requestor's access to the resource.To get the property, please explictly use `$select=permissions` in the query.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16b9a-167">Relações</span><span class="sxs-lookup"><span data-stu-id="16b9a-167">Relationships</span></span>
| <span data-ttu-id="16b9a-168">Relação</span><span class="sxs-lookup"><span data-stu-id="16b9a-168">Relationship</span></span>   | <span data-ttu-id="16b9a-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="16b9a-169">Type</span></span>                                         |<span data-ttu-id="16b9a-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="16b9a-170">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="16b9a-171">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="16b9a-171">roleAssignments</span></span> |<span data-ttu-id="16b9a-172">[Coleção governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="16b9a-172">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="16b9a-173">A coleção de atribuições de função para o recurso.</span><span class="sxs-lookup"><span data-stu-id="16b9a-173">The collection of role assignments for the resource.</span></span>|
|<span data-ttu-id="16b9a-174">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="16b9a-174">roleDefinitions</span></span> |<span data-ttu-id="16b9a-175">[Coleção governanceRoleDefinition](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="16b9a-175">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="16b9a-176">A coleção de definições de função para o recurso.</span><span class="sxs-lookup"><span data-stu-id="16b9a-176">The collection of role defintions for the resource.</span></span>|
|<span data-ttu-id="16b9a-177">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="16b9a-177">roleAssignmentRequests</span></span> |<span data-ttu-id="16b9a-178">[Coleção governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="16b9a-178">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="16b9a-179">A coleção de solicitações de atribuição de função para o recurso.</span><span class="sxs-lookup"><span data-stu-id="16b9a-179">The collection of role assignment requests for the resource.</span></span>|
|<span data-ttu-id="16b9a-180">roleSettings</span><span class="sxs-lookup"><span data-stu-id="16b9a-180">roleSettings</span></span> |<span data-ttu-id="16b9a-181">[Coleção governanceRoleSetting](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="16b9a-181">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="16b9a-182">A coleção de configurações de função do recurso.</span><span class="sxs-lookup"><span data-stu-id="16b9a-182">The collection of role settings for the resource.</span></span>|
|<span data-ttu-id="16b9a-183">primário</span><span class="sxs-lookup"><span data-stu-id="16b9a-183">parent</span></span>          |[<span data-ttu-id="16b9a-184">governanceResource</span><span class="sxs-lookup"><span data-stu-id="16b9a-184">governanceResource</span></span>](../resources/governanceresource.md)           |<span data-ttu-id="16b9a-185">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="16b9a-185">Read-only.</span></span> <span data-ttu-id="16b9a-186">O recurso pai.</span><span class="sxs-lookup"><span data-stu-id="16b9a-186">The parent resource.</span></span> <span data-ttu-id="16b9a-187">para `pimforazurerbac` cenário, ele pode representar a assinatura à que o recurso pertence.</span><span class="sxs-lookup"><span data-stu-id="16b9a-187">for `pimforazurerbac` scenario, it can represent the subscription the resource belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="16b9a-188">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="16b9a-188">JSON representation</span></span>

<span data-ttu-id="16b9a-189">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="16b9a-189">The following is a JSON representation of the resource.</span></span>

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


