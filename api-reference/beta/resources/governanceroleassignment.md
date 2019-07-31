---
title: tipo de recurso governanceRoleAssignment
description: Representa a atribuição de um usuário ou grupo a uma função.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 518fbe18fcd09b1b4cc9730c6b7f0112adabfeae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971876"
---
# <a name="governanceroleassignment-resource-type"></a><span data-ttu-id="50f8a-103">tipo de recurso governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="50f8a-103">governanceRoleAssignment resource type</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50f8a-104">Representa a atribuição de um usuário ou grupo a uma função.</span><span class="sxs-lookup"><span data-stu-id="50f8a-104">Represents the assignment of a user or group to a role.</span></span>

<span data-ttu-id="50f8a-105">O gerenciamento de identidade privilegiada (PIM) oferece suporte a dois tipos de atribuições:</span><span class="sxs-lookup"><span data-stu-id="50f8a-105">Privileged Identity Management (PIM) supports two types of assignments:</span></span>

1. <span data-ttu-id="50f8a-106">Atribuição ativa – representa o acesso direto/ativado aos recursos.</span><span class="sxs-lookup"><span data-stu-id="50f8a-106">Active assignment - Represents the direct/activated access to resources.</span></span>
2. <span data-ttu-id="50f8a-107">Atribuição qualificada – representa um estágio intermediário de acesso privilegiado a recursos, entre sem acesso e acesso direto.</span><span class="sxs-lookup"><span data-stu-id="50f8a-107">Eligible assignment - Represents an intermediate stage of privileged access to resources, between no access and direct access.</span></span> <span data-ttu-id="50f8a-108">Os administradores podem atribuir usuários/grupos `eligible assignment` com antecedência e sempre que o acesso for necessário, `activation` quando `eligible assignment` for necessário, para obter o acesso instantâneo ao recurso por várias horas.</span><span class="sxs-lookup"><span data-stu-id="50f8a-108">Administrators can assign users/groups to `eligible assignment` in advance, and whenever the access is needed, `activation` on the `eligible assignment` is needed to gain the instant access to the resource for several hours.</span></span> <span data-ttu-id="50f8a-109">Após a ativação, `active assignment` um será criado para os membros de usuários/grupos para indicar o status ativado.</span><span class="sxs-lookup"><span data-stu-id="50f8a-109">After activation, an `active assignment` will be created for the users/group members to indicate the activated status.</span></span>

## <a name="methods"></a><span data-ttu-id="50f8a-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="50f8a-110">Methods</span></span>

| <span data-ttu-id="50f8a-111">Método</span><span class="sxs-lookup"><span data-stu-id="50f8a-111">Method</span></span>          | <span data-ttu-id="50f8a-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="50f8a-112">Return Type</span></span> |<span data-ttu-id="50f8a-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="50f8a-113">Description</span></span>|
|:------------|:--------|:--------|
|[<span data-ttu-id="50f8a-114">Get</span><span class="sxs-lookup"><span data-stu-id="50f8a-114">Get</span></span>](../api/governanceroleassignment-get.md) |  [<span data-ttu-id="50f8a-115">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="50f8a-115">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md) |<span data-ttu-id="50f8a-116">Leia as propriedades e as relações de uma entidade de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="50f8a-116">Read properties and relationships of a role assignment entity.</span></span>|
|[<span data-ttu-id="50f8a-117">List</span><span class="sxs-lookup"><span data-stu-id="50f8a-117">List</span></span>](../api/governanceroleassignment-list.md) | <span data-ttu-id="50f8a-118">coleção [governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="50f8a-118">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="50f8a-119">Lista uma coleção de atribuições de função em um recurso.</span><span class="sxs-lookup"><span data-stu-id="50f8a-119">List a collection of role assignments on a resource.</span></span> |
|[<span data-ttu-id="50f8a-120">Export</span><span class="sxs-lookup"><span data-stu-id="50f8a-120">Export</span></span>](../api/governanceroleassignment-export.md) | <span data-ttu-id="50f8a-121">octeto-Stream</span><span class="sxs-lookup"><span data-stu-id="50f8a-121">octet-stream</span></span> |<span data-ttu-id="50f8a-122">Baixe uma coleção de atribuições de função em um recurso e salve `.csv` como um arquivo.</span><span class="sxs-lookup"><span data-stu-id="50f8a-122">Download a collection of role assignments on a resource and save as a `.csv` file.</span></span>|

<span data-ttu-id="50f8a-123">`POST` `DELETE` Nenhuma operação é suportada no conjunto de `roleAssignments` `PUT` `PATCH`entidades.</span><span class="sxs-lookup"><span data-stu-id="50f8a-123">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `roleAssignments` entity set.</span></span> <span data-ttu-id="50f8a-124">Qualquer operação de criação, atualização e exclusão no `governanceRoleAssignment` é feita por `governanceRoleAssignmentRequest`.</span><span class="sxs-lookup"><span data-stu-id="50f8a-124">Any create, update, and delete operations on `governanceRoleAssignment` are done by `governanceRoleAssignmentRequest`.</span></span>

## <a name="properties"></a><span data-ttu-id="50f8a-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50f8a-125">Properties</span></span>
| <span data-ttu-id="50f8a-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50f8a-126">Property</span></span>  | <span data-ttu-id="50f8a-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="50f8a-127">Type</span></span>      |<span data-ttu-id="50f8a-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="50f8a-128">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="50f8a-129">id</span><span class="sxs-lookup"><span data-stu-id="50f8a-129">id</span></span>         |<span data-ttu-id="50f8a-130">String</span><span class="sxs-lookup"><span data-stu-id="50f8a-130">String</span></span>     |<span data-ttu-id="50f8a-131">A ID da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="50f8a-131">The ID of the role assignment.</span></span> <span data-ttu-id="50f8a-132">Está no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="50f8a-132">It is in GUID format.</span></span>|
|<span data-ttu-id="50f8a-133">resourceId</span><span class="sxs-lookup"><span data-stu-id="50f8a-133">resourceId</span></span> |<span data-ttu-id="50f8a-134">String</span><span class="sxs-lookup"><span data-stu-id="50f8a-134">String</span></span>     |<span data-ttu-id="50f8a-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50f8a-135">Required.</span></span> <span data-ttu-id="50f8a-136">A identificação do recurso ao qual a atribuição de função está associada.</span><span class="sxs-lookup"><span data-stu-id="50f8a-136">The ID of the resource which the role assignment is associated with.</span></span> |
|<span data-ttu-id="50f8a-137">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="50f8a-137">roleDefinitionId</span></span>|<span data-ttu-id="50f8a-138">String</span><span class="sxs-lookup"><span data-stu-id="50f8a-138">String</span></span>|<span data-ttu-id="50f8a-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50f8a-139">Required.</span></span> <span data-ttu-id="50f8a-140">A ID da definição de função à qual a atribuição de função está associada.</span><span class="sxs-lookup"><span data-stu-id="50f8a-140">The ID of the role definition which the role assignment is associated with.</span></span> |
|<span data-ttu-id="50f8a-141">SubjectID</span><span class="sxs-lookup"><span data-stu-id="50f8a-141">subjectId</span></span>|<span data-ttu-id="50f8a-142">String</span><span class="sxs-lookup"><span data-stu-id="50f8a-142">String</span></span>       |<span data-ttu-id="50f8a-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50f8a-143">Required.</span></span> <span data-ttu-id="50f8a-144">A ID da entidade à qual a atribuição de função está associada.</span><span class="sxs-lookup"><span data-stu-id="50f8a-144">The ID of the subject which the role assignment is associated with.</span></span> |
|<span data-ttu-id="50f8a-145">linkedEligibleRoleAssignmentId</span><span class="sxs-lookup"><span data-stu-id="50f8a-145">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="50f8a-146">String</span><span class="sxs-lookup"><span data-stu-id="50f8a-146">String</span></span>|<span data-ttu-id="50f8a-147">Se este é um `active assignment` e criado devido à ativação em um `eligible assignment`, ele representa o ID dele `eligible assignment`; Caso contrário, o valor `null`será.</span><span class="sxs-lookup"><span data-stu-id="50f8a-147">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the ID of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |
|<span data-ttu-id="50f8a-148">externalId</span><span class="sxs-lookup"><span data-stu-id="50f8a-148">externalId</span></span>   |<span data-ttu-id="50f8a-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50f8a-149">String</span></span>     |<span data-ttu-id="50f8a-150">A ID externa o recurso usado para identificar a atribuição de função no provedor.</span><span class="sxs-lookup"><span data-stu-id="50f8a-150">The external ID the resource that is used to identify the role assignment in the provider.</span></span>|
|<span data-ttu-id="50f8a-151">startDateTime</span><span class="sxs-lookup"><span data-stu-id="50f8a-151">startDateTime</span></span>|<span data-ttu-id="50f8a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50f8a-152">DateTimeOffset</span></span>|<span data-ttu-id="50f8a-153">A hora de início da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="50f8a-153">The start time of the role assignment.</span></span> <span data-ttu-id="50f8a-154">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="50f8a-154">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="50f8a-155">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="50f8a-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="50f8a-156">endDateTime</span><span class="sxs-lookup"><span data-stu-id="50f8a-156">endDateTime</span></span>|<span data-ttu-id="50f8a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50f8a-157">DateTimeOffset</span></span>|<span data-ttu-id="50f8a-158">Para uma atribuição de função não permanente, esse é o momento em que a atribuição de função será expirada.</span><span class="sxs-lookup"><span data-stu-id="50f8a-158">For a non-permanent role assignment, this is the time when the role assignment will be expired.</span></span> <span data-ttu-id="50f8a-159">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="50f8a-159">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="50f8a-160">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="50f8a-160">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="50f8a-161">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="50f8a-161">assignmentState</span></span>|<span data-ttu-id="50f8a-162">String</span><span class="sxs-lookup"><span data-stu-id="50f8a-162">String</span></span>  |<span data-ttu-id="50f8a-163">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="50f8a-163">The state of the assignment.</span></span> <span data-ttu-id="50f8a-164">O valor pode ser</span><span class="sxs-lookup"><span data-stu-id="50f8a-164">The value can be</span></span> <ul><li> <span data-ttu-id="50f8a-165">`Eligible`para atribuição qualificada</span><span class="sxs-lookup"><span data-stu-id="50f8a-165">`Eligible` for eligible assignment</span></span></li><li> <span data-ttu-id="50f8a-166">`Active`– Se ele for atribuído `Active` diretamente por administradores ou ativado em uma atribuição qualificada pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="50f8a-166">`Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span></li></ul>|
|<span data-ttu-id="50f8a-167">memberType</span><span class="sxs-lookup"><span data-stu-id="50f8a-167">memberType</span></span>|<span data-ttu-id="50f8a-168">String</span><span class="sxs-lookup"><span data-stu-id="50f8a-168">String</span></span>      |<span data-ttu-id="50f8a-169">O tipo do membro.</span><span class="sxs-lookup"><span data-stu-id="50f8a-169">The type of member.</span></span> <span data-ttu-id="50f8a-170">O valor pode ser:</span><span class="sxs-lookup"><span data-stu-id="50f8a-170">The value can be:</span></span> <ul><li><span data-ttu-id="50f8a-171">`Inherited`-a atribuição de função é herdada de um escopo de recurso pai</span><span class="sxs-lookup"><span data-stu-id="50f8a-171">`Inherited` - the role assignment is inherited from a parent resource scope</span></span></li><li><span data-ttu-id="50f8a-172">`Group`– a atribuição de função não é herdada, mas vem da Associação de uma atribuição de grupo</span><span class="sxs-lookup"><span data-stu-id="50f8a-172">`Group`- the role assignment is not inherited, but comes from the membership of a group assignment</span></span></li><li><span data-ttu-id="50f8a-173">`User`– a atribuição de função não é herdada nem de uma atribuição de grupo.</span><span class="sxs-lookup"><span data-stu-id="50f8a-173">`User` - the role assignment is neither inherited nor from a group assignment.</span></span></li></ul>|


## <a name="relationships"></a><span data-ttu-id="50f8a-174">Relações</span><span class="sxs-lookup"><span data-stu-id="50f8a-174">Relationships</span></span>
| <span data-ttu-id="50f8a-175">Relação</span><span class="sxs-lookup"><span data-stu-id="50f8a-175">Relationship</span></span> | <span data-ttu-id="50f8a-176">Tipo</span><span class="sxs-lookup"><span data-stu-id="50f8a-176">Type</span></span>   |<span data-ttu-id="50f8a-177">Descrição</span><span class="sxs-lookup"><span data-stu-id="50f8a-177">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50f8a-178">recurso</span><span class="sxs-lookup"><span data-stu-id="50f8a-178">resource</span></span>|[<span data-ttu-id="50f8a-179">Entidadegovernanceresource</span><span class="sxs-lookup"><span data-stu-id="50f8a-179">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="50f8a-180">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50f8a-180">Read-only.</span></span> <span data-ttu-id="50f8a-181">O recurso associado à atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="50f8a-181">The resource associated with the role assignment.</span></span> |
|<span data-ttu-id="50f8a-182">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="50f8a-182">roleDefinition</span></span>|[<span data-ttu-id="50f8a-183">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="50f8a-183">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="50f8a-184">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50f8a-184">Read-only.</span></span> <span data-ttu-id="50f8a-185">A definição de função associada à atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="50f8a-185">The role definition associated with the role assignment.</span></span> |
|<span data-ttu-id="50f8a-186">subject</span><span class="sxs-lookup"><span data-stu-id="50f8a-186">subject</span></span>|[<span data-ttu-id="50f8a-187">governanceSubject</span><span class="sxs-lookup"><span data-stu-id="50f8a-187">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="50f8a-188">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50f8a-188">Read-only.</span></span> <span data-ttu-id="50f8a-189">O assunto associado à atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="50f8a-189">The subject associated with the role assignment.</span></span> |
|<span data-ttu-id="50f8a-190">linkedEligibleRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="50f8a-190">linkedEligibleRoleAssignment</span></span>|[<span data-ttu-id="50f8a-191">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="50f8a-191">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md)|<span data-ttu-id="50f8a-192">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50f8a-192">Read-only.</span></span> <span data-ttu-id="50f8a-193">Se este é um `active assignment` e criado devido à ativação em um `eligible assignment`, ele representa o objeto desse `eligible assignment`; Caso contrário, o valor `null`será.</span><span class="sxs-lookup"><span data-stu-id="50f8a-193">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the object of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="50f8a-194">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50f8a-194">JSON representation</span></span>

<span data-ttu-id="50f8a-195">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="50f8a-195">Here is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleAssignment"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "subjectId": "String",
  "linkedEligibleRoleAssignmentId": "String",
  "externalId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "assignmentState": "String",
  "memberType": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
