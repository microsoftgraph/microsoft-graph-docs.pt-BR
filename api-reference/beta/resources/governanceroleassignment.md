---
title: tipo de recurso governanceRoleAssignment
description: Representa a atribuição de um usuário ou grupo a uma função.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 96bb2179798049946026872e7c4ce4f4d82f155f
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219239"
---
# <a name="governanceroleassignment-resource-type"></a><span data-ttu-id="f2eca-103">tipo de recurso governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="f2eca-103">governanceRoleAssignment resource type</span></span>

<span data-ttu-id="f2eca-104">Namespace: Microsoft. Graph[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="f2eca-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="f2eca-105">Representa a atribuição de um usuário ou grupo a uma função.</span><span class="sxs-lookup"><span data-stu-id="f2eca-105">Represents the assignment of a user or group to a role.</span></span>

<span data-ttu-id="f2eca-106">O gerenciamento de identidade privilegiada (PIM) oferece suporte a dois tipos de atribuições:</span><span class="sxs-lookup"><span data-stu-id="f2eca-106">Privileged Identity Management (PIM) supports two types of assignments:</span></span>

1. <span data-ttu-id="f2eca-107">Atribuição ativa – representa o acesso direto/ativado aos recursos.</span><span class="sxs-lookup"><span data-stu-id="f2eca-107">Active assignment - Represents the direct/activated access to resources.</span></span>
2. <span data-ttu-id="f2eca-108">Atribuição qualificada – representa um estágio intermediário de acesso privilegiado a recursos, entre sem acesso e acesso direto.</span><span class="sxs-lookup"><span data-stu-id="f2eca-108">Eligible assignment - Represents an intermediate stage of privileged access to resources, between no access and direct access.</span></span> <span data-ttu-id="f2eca-109">Os administradores podem atribuir usuários/grupos `eligible assignment` com antecedência e sempre que o acesso for necessário, `activation` quando `eligible assignment` for necessário, para obter o acesso instantâneo ao recurso por várias horas.</span><span class="sxs-lookup"><span data-stu-id="f2eca-109">Administrators can assign users/groups to `eligible assignment` in advance, and whenever the access is needed, `activation` on the `eligible assignment` is needed to gain the instant access to the resource for several hours.</span></span> <span data-ttu-id="f2eca-110">Após a ativação, `active assignment` um será criado para os membros de usuários/grupos para indicar o status ativado.</span><span class="sxs-lookup"><span data-stu-id="f2eca-110">After activation, an `active assignment` will be created for the users/group members to indicate the activated status.</span></span>

## <a name="methods"></a><span data-ttu-id="f2eca-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="f2eca-111">Methods</span></span>

| <span data-ttu-id="f2eca-112">Método</span><span class="sxs-lookup"><span data-stu-id="f2eca-112">Method</span></span>          | <span data-ttu-id="f2eca-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f2eca-113">Return Type</span></span> |<span data-ttu-id="f2eca-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2eca-114">Description</span></span>|
|:------------|:--------|:--------|
|[<span data-ttu-id="f2eca-115">Get</span><span class="sxs-lookup"><span data-stu-id="f2eca-115">Get</span></span>](../api/governanceroleassignment-get.md) |  [<span data-ttu-id="f2eca-116">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="f2eca-116">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md) |<span data-ttu-id="f2eca-117">Leia as propriedades e as relações de uma entidade de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f2eca-117">Read properties and relationships of a role assignment entity.</span></span>|
|[<span data-ttu-id="f2eca-118">List</span><span class="sxs-lookup"><span data-stu-id="f2eca-118">List</span></span>](../api/governanceroleassignment-list.md) | <span data-ttu-id="f2eca-119">coleção [governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f2eca-119">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="f2eca-120">Lista uma coleção de atribuições de função em um recurso.</span><span class="sxs-lookup"><span data-stu-id="f2eca-120">List a collection of role assignments on a resource.</span></span> |
|[<span data-ttu-id="f2eca-121">Export</span><span class="sxs-lookup"><span data-stu-id="f2eca-121">Export</span></span>](../api/governanceroleassignment-export.md) | <span data-ttu-id="f2eca-122">octeto-Stream</span><span class="sxs-lookup"><span data-stu-id="f2eca-122">octet-stream</span></span> |<span data-ttu-id="f2eca-123">Baixe uma coleção de atribuições de função em um recurso e salve `.csv` como um arquivo.</span><span class="sxs-lookup"><span data-stu-id="f2eca-123">Download a collection of role assignments on a resource and save as a `.csv` file.</span></span>|

<span data-ttu-id="f2eca-124">`POST` `DELETE` Nenhuma operação é suportada no conjunto de `roleAssignments` `PUT` `PATCH`entidades.</span><span class="sxs-lookup"><span data-stu-id="f2eca-124">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `roleAssignments` entity set.</span></span> <span data-ttu-id="f2eca-125">Qualquer operação de criação, atualização e exclusão no `governanceRoleAssignment` é feita por `governanceRoleAssignmentRequest`.</span><span class="sxs-lookup"><span data-stu-id="f2eca-125">Any create, update, and delete operations on `governanceRoleAssignment` are done by `governanceRoleAssignmentRequest`.</span></span>

## <a name="properties"></a><span data-ttu-id="f2eca-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f2eca-126">Properties</span></span>
| <span data-ttu-id="f2eca-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2eca-127">Property</span></span>  | <span data-ttu-id="f2eca-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2eca-128">Type</span></span>      |<span data-ttu-id="f2eca-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2eca-129">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="f2eca-130">id</span><span class="sxs-lookup"><span data-stu-id="f2eca-130">id</span></span>         |<span data-ttu-id="f2eca-131">String</span><span class="sxs-lookup"><span data-stu-id="f2eca-131">String</span></span>     |<span data-ttu-id="f2eca-132">A ID da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f2eca-132">The ID of the role assignment.</span></span> <span data-ttu-id="f2eca-133">Está no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="f2eca-133">It is in GUID format.</span></span>|
|<span data-ttu-id="f2eca-134">resourceId</span><span class="sxs-lookup"><span data-stu-id="f2eca-134">resourceId</span></span> |<span data-ttu-id="f2eca-135">String</span><span class="sxs-lookup"><span data-stu-id="f2eca-135">String</span></span>     |<span data-ttu-id="f2eca-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2eca-136">Required.</span></span> <span data-ttu-id="f2eca-137">A identificação do recurso ao qual a atribuição de função está associada.</span><span class="sxs-lookup"><span data-stu-id="f2eca-137">The ID of the resource which the role assignment is associated with.</span></span> |
|<span data-ttu-id="f2eca-138">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="f2eca-138">roleDefinitionId</span></span>|<span data-ttu-id="f2eca-139">String</span><span class="sxs-lookup"><span data-stu-id="f2eca-139">String</span></span>|<span data-ttu-id="f2eca-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2eca-140">Required.</span></span> <span data-ttu-id="f2eca-141">A ID da definição de função à qual a atribuição de função está associada.</span><span class="sxs-lookup"><span data-stu-id="f2eca-141">The ID of the role definition which the role assignment is associated with.</span></span> |
|<span data-ttu-id="f2eca-142">SubjectID</span><span class="sxs-lookup"><span data-stu-id="f2eca-142">subjectId</span></span>|<span data-ttu-id="f2eca-143">String</span><span class="sxs-lookup"><span data-stu-id="f2eca-143">String</span></span>       |<span data-ttu-id="f2eca-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2eca-144">Required.</span></span> <span data-ttu-id="f2eca-145">A ID da entidade à qual a atribuição de função está associada.</span><span class="sxs-lookup"><span data-stu-id="f2eca-145">The ID of the subject which the role assignment is associated with.</span></span> |
|<span data-ttu-id="f2eca-146">linkedEligibleRoleAssignmentId</span><span class="sxs-lookup"><span data-stu-id="f2eca-146">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="f2eca-147">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="f2eca-147">String</span></span>|<span data-ttu-id="f2eca-148">Se este é um `active assignment` e criado devido à ativação em um `eligible assignment`, ele representa o ID dele `eligible assignment`; Caso contrário, o valor `null`será.</span><span class="sxs-lookup"><span data-stu-id="f2eca-148">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the ID of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |
|<span data-ttu-id="f2eca-149">externalId</span><span class="sxs-lookup"><span data-stu-id="f2eca-149">externalId</span></span>   |<span data-ttu-id="f2eca-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2eca-150">String</span></span>     |<span data-ttu-id="f2eca-151">A ID externa o recurso usado para identificar a atribuição de função no provedor.</span><span class="sxs-lookup"><span data-stu-id="f2eca-151">The external ID the resource that is used to identify the role assignment in the provider.</span></span>|
|<span data-ttu-id="f2eca-152">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f2eca-152">startDateTime</span></span>|<span data-ttu-id="f2eca-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2eca-153">DateTimeOffset</span></span>|<span data-ttu-id="f2eca-154">A hora de início da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f2eca-154">The start time of the role assignment.</span></span> <span data-ttu-id="f2eca-155">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f2eca-155">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f2eca-156">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f2eca-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f2eca-157">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f2eca-157">endDateTime</span></span>|<span data-ttu-id="f2eca-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2eca-158">DateTimeOffset</span></span>|<span data-ttu-id="f2eca-159">Para uma atribuição de função não permanente, esse é o momento em que a atribuição de função será expirada.</span><span class="sxs-lookup"><span data-stu-id="f2eca-159">For a non-permanent role assignment, this is the time when the role assignment will be expired.</span></span> <span data-ttu-id="f2eca-160">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f2eca-160">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f2eca-161">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f2eca-161">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f2eca-162">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="f2eca-162">assignmentState</span></span>|<span data-ttu-id="f2eca-163">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="f2eca-163">String</span></span>  |<span data-ttu-id="f2eca-164">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="f2eca-164">The state of the assignment.</span></span> <span data-ttu-id="f2eca-165">O valor pode ser</span><span class="sxs-lookup"><span data-stu-id="f2eca-165">The value can be</span></span> <ul><li> <span data-ttu-id="f2eca-166">`Eligible`para atribuição qualificada</span><span class="sxs-lookup"><span data-stu-id="f2eca-166">`Eligible` for eligible assignment</span></span></li><li> <span data-ttu-id="f2eca-167">`Active`– Se ele for atribuído `Active` diretamente por administradores ou ativado em uma atribuição qualificada pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="f2eca-167">`Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span></li></ul>|
|<span data-ttu-id="f2eca-168">memberType</span><span class="sxs-lookup"><span data-stu-id="f2eca-168">memberType</span></span>|<span data-ttu-id="f2eca-169">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="f2eca-169">String</span></span>      |<span data-ttu-id="f2eca-170">O tipo do membro.</span><span class="sxs-lookup"><span data-stu-id="f2eca-170">The type of member.</span></span> <span data-ttu-id="f2eca-171">O valor pode ser:</span><span class="sxs-lookup"><span data-stu-id="f2eca-171">The value can be:</span></span> <ul><li><span data-ttu-id="f2eca-172">`Inherited`-a atribuição de função é herdada de um escopo de recurso pai</span><span class="sxs-lookup"><span data-stu-id="f2eca-172">`Inherited` - the role assignment is inherited from a parent resource scope</span></span></li><li><span data-ttu-id="f2eca-173">`Group`– a atribuição de função não é herdada, mas vem da Associação de uma atribuição de grupo</span><span class="sxs-lookup"><span data-stu-id="f2eca-173">`Group`- the role assignment is not inherited, but comes from the membership of a group assignment</span></span></li><li><span data-ttu-id="f2eca-174">`User`– a atribuição de função não é herdada nem de uma atribuição de grupo.</span><span class="sxs-lookup"><span data-stu-id="f2eca-174">`User` - the role assignment is neither inherited nor from a group assignment.</span></span></li></ul>|


## <a name="relationships"></a><span data-ttu-id="f2eca-175">Relações</span><span class="sxs-lookup"><span data-stu-id="f2eca-175">Relationships</span></span>
| <span data-ttu-id="f2eca-176">Relação</span><span class="sxs-lookup"><span data-stu-id="f2eca-176">Relationship</span></span> | <span data-ttu-id="f2eca-177">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2eca-177">Type</span></span>   |<span data-ttu-id="f2eca-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2eca-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2eca-179">recurso</span><span class="sxs-lookup"><span data-stu-id="f2eca-179">resource</span></span>|[<span data-ttu-id="f2eca-180">governanceResource</span><span class="sxs-lookup"><span data-stu-id="f2eca-180">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="f2eca-181">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2eca-181">Read-only.</span></span> <span data-ttu-id="f2eca-182">O recurso associado à atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f2eca-182">The resource associated with the role assignment.</span></span> |
|<span data-ttu-id="f2eca-183">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="f2eca-183">roleDefinition</span></span>|[<span data-ttu-id="f2eca-184">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="f2eca-184">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="f2eca-185">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2eca-185">Read-only.</span></span> <span data-ttu-id="f2eca-186">A definição de função associada à atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f2eca-186">The role definition associated with the role assignment.</span></span> |
|<span data-ttu-id="f2eca-187">assunto</span><span class="sxs-lookup"><span data-stu-id="f2eca-187">subject</span></span>|[<span data-ttu-id="f2eca-188">governanceSubject</span><span class="sxs-lookup"><span data-stu-id="f2eca-188">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="f2eca-189">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2eca-189">Read-only.</span></span> <span data-ttu-id="f2eca-190">O assunto associado à atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f2eca-190">The subject associated with the role assignment.</span></span> |
|<span data-ttu-id="f2eca-191">linkedEligibleRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="f2eca-191">linkedEligibleRoleAssignment</span></span>|[<span data-ttu-id="f2eca-192">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="f2eca-192">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md)|<span data-ttu-id="f2eca-193">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2eca-193">Read-only.</span></span> <span data-ttu-id="f2eca-194">Se este é um `active assignment` e criado devido à ativação em um `eligible assignment`, ele representa o objeto desse `eligible assignment`; Caso contrário, o valor `null`será.</span><span class="sxs-lookup"><span data-stu-id="f2eca-194">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the object of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f2eca-195">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f2eca-195">JSON representation</span></span>

<span data-ttu-id="f2eca-196">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f2eca-196">Here is a JSON representation of the resource.</span></span>


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
