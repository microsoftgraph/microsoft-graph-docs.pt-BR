---
title: Tipo de recurso governanceRoleAssignmentRequest
description: Representa a solicitação de operações de atribuição de função em Gerenciamento de Identidade Privada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: e96a0009c6108a77383fe770a6351d7b64efd6f7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961276"
---
# <a name="governanceroleassignmentrequest-resource-type"></a><span data-ttu-id="171c8-103">Tipo de recurso governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="171c8-103">governanceRoleAssignmentRequest resource type</span></span>

<span data-ttu-id="171c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="171c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="171c8-105">Representa a solicitação de operações de atribuição de função em Gerenciamento de Identidade Privilegd.</span><span class="sxs-lookup"><span data-stu-id="171c8-105">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="171c8-106">`governanceRoleAssignmentRequest` é uma entidade modelada por tíquete usada para gerenciar o ciclo de vida das atribuições de função.</span><span class="sxs-lookup"><span data-stu-id="171c8-106">`governanceRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="171c8-107">Ele representa a intenção/decisão dos usuários e administradores e também oferece a flexibilidade para habilitar a implementação de esquemas recorrentes, portais de aprovação e assim por diante, em comparação com a exposição direta , e operações `POST` `PUT` em `DELETE` `governanceRoleAssignment` .</span><span class="sxs-lookup"><span data-stu-id="171c8-107">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST`, `PUT`, and `DELETE` operations on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="171c8-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="171c8-108">Methods</span></span>

| <span data-ttu-id="171c8-109">Método</span><span class="sxs-lookup"><span data-stu-id="171c8-109">Method</span></span>          |<span data-ttu-id="171c8-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="171c8-110">Return Type</span></span>  |<span data-ttu-id="171c8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="171c8-111">Description</span></span>|
|:------------|:--------|:--------|
|[<span data-ttu-id="171c8-112">Get</span><span class="sxs-lookup"><span data-stu-id="171c8-112">Get</span></span>](../api/governanceroleassignmentrequest-get.md) | [<span data-ttu-id="171c8-113">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="171c8-113">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="171c8-114">Obter uma solicitação de atribuição de função especificada pela ID.</span><span class="sxs-lookup"><span data-stu-id="171c8-114">Get a role assignment request specified by ID.</span></span>  
|[<span data-ttu-id="171c8-115">Lista</span><span class="sxs-lookup"><span data-stu-id="171c8-115">List</span></span>](../api/governanceroleassignmentrequest-list.md) | <span data-ttu-id="171c8-116">[Coleção governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="171c8-116">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="171c8-117">Obter solicitações de atribuição de função em um recurso.</span><span class="sxs-lookup"><span data-stu-id="171c8-117">Get role assignment requests on a resource.</span></span>|
|[<span data-ttu-id="171c8-118">Create</span><span class="sxs-lookup"><span data-stu-id="171c8-118">Create</span></span>](../api/governanceroleassignmentrequest-post.md)|  [<span data-ttu-id="171c8-119">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="171c8-119">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="171c8-120">Crie uma solicitação para gerenciar o ciclo de vida da atribuição de função existente ou nova.</span><span class="sxs-lookup"><span data-stu-id="171c8-120">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="171c8-121">Cancel</span><span class="sxs-lookup"><span data-stu-id="171c8-121">Cancel</span></span>](../api/governanceroleassignmentrequest-cancel.md)|  |<span data-ttu-id="171c8-122">Cancele uma solicitação de atribuição de função pendente.</span><span class="sxs-lookup"><span data-stu-id="171c8-122">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="171c8-123">Atualização</span><span class="sxs-lookup"><span data-stu-id="171c8-123">Update</span></span>](../api/governanceroleassignmentrequest-update.md)| [<span data-ttu-id="171c8-124">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="171c8-124">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="171c8-125">Os administradores atualizam as decisões sobre solicitações se as solicitações estão em status de `PendingAdminDecision` .</span><span class="sxs-lookup"><span data-stu-id="171c8-125">Administrators update the decisions on requests if the requests are in status of `PendingAdminDecision`.</span></span>|

## <a name="properties"></a><span data-ttu-id="171c8-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="171c8-126">Properties</span></span>
| <span data-ttu-id="171c8-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="171c8-127">Property</span></span>                  | <span data-ttu-id="171c8-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="171c8-128">Type</span></span>          |<span data-ttu-id="171c8-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="171c8-129">Description</span></span>|
|:--------------------------|:--------------|:----------|
|<span data-ttu-id="171c8-130">id</span><span class="sxs-lookup"><span data-stu-id="171c8-130">id</span></span>                         |<span data-ttu-id="171c8-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="171c8-131">String</span></span>         |<span data-ttu-id="171c8-132">A id da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="171c8-132">The id of the role assignment request.</span></span>|
|<span data-ttu-id="171c8-133">resourceId</span><span class="sxs-lookup"><span data-stu-id="171c8-133">resourceId</span></span>                 |<span data-ttu-id="171c8-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="171c8-134">String</span></span>         |<span data-ttu-id="171c8-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="171c8-135">Required.</span></span> <span data-ttu-id="171c8-136">A id do recurso ao qual a solicitação de atribuição de função está associada.</span><span class="sxs-lookup"><span data-stu-id="171c8-136">The id of the resource which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="171c8-137">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="171c8-137">roleDefinitionId</span></span>           |<span data-ttu-id="171c8-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="171c8-138">String</span></span>         |<span data-ttu-id="171c8-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="171c8-139">Required.</span></span> <span data-ttu-id="171c8-140">A id da definição de função à qual a solicitação de atribuição de função está associada.</span><span class="sxs-lookup"><span data-stu-id="171c8-140">The id of the role definition which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="171c8-141">subjectId</span><span class="sxs-lookup"><span data-stu-id="171c8-141">subjectId</span></span>                  |<span data-ttu-id="171c8-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="171c8-142">String</span></span>         |<span data-ttu-id="171c8-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="171c8-143">Required.</span></span> <span data-ttu-id="171c8-144">A id do assunto ao qual a solicitação de atribuição de função está associada.</span><span class="sxs-lookup"><span data-stu-id="171c8-144">The id of the subject which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="171c8-145">tipo</span><span class="sxs-lookup"><span data-stu-id="171c8-145">type</span></span>                       |<span data-ttu-id="171c8-146">String</span><span class="sxs-lookup"><span data-stu-id="171c8-146">String</span></span>        |<span data-ttu-id="171c8-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="171c8-147">Required.</span></span> <span data-ttu-id="171c8-148">Representando o tipo da operação na atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="171c8-148">Representing the type of the operation on the role assignment.</span></span> <span data-ttu-id="171c8-149">Os valores possíveis são: `AdminAdd` , , , , , , , , `UserAdd` , `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `AdminExtend` `UserRenew` `AdminRenew` .</span><span class="sxs-lookup"><span data-stu-id="171c8-149">The possible values are: `AdminAdd` , `UserAdd` , `AdminUpdate` , `AdminRemove` , `UserRemove` , `UserExtend` , `AdminExtend` , `UserRenew` , `AdminRenew`.</span></span>|
|<span data-ttu-id="171c8-150">assignmentState</span><span class="sxs-lookup"><span data-stu-id="171c8-150">assignmentState</span></span>|<span data-ttu-id="171c8-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="171c8-151">String</span></span>  |<span data-ttu-id="171c8-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="171c8-152">Required.</span></span> <span data-ttu-id="171c8-153">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="171c8-153">The state of the assignment.</span></span> <span data-ttu-id="171c8-154">Os valores possíveis são: (para atribuição qualificada), (se for atribuída diretamente), (por administradores ou ativada em uma atribuição qualificada `Eligible`  `Active` pelos `Active` usuários).</span><span class="sxs-lookup"><span data-stu-id="171c8-154">The possible values are: `Eligible` (for eligible assignment),  `Active` (if it is directly assigned), `Active` (by administrators, or activated on an eligible assignment by the users).</span></span>|
|<span data-ttu-id="171c8-155">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="171c8-155">requestedDateTime</span></span>          |<span data-ttu-id="171c8-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="171c8-156">DateTimeOffset</span></span> |<span data-ttu-id="171c8-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="171c8-157">Read-only.</span></span> <span data-ttu-id="171c8-158">A solicitação cria tempo.</span><span class="sxs-lookup"><span data-stu-id="171c8-158">The request create time.</span></span> <span data-ttu-id="171c8-159">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="171c8-159">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="171c8-160">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="171c8-160">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="171c8-161">Cronograma</span><span class="sxs-lookup"><span data-stu-id="171c8-161">schedule</span></span>                   |[<span data-ttu-id="171c8-162">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="171c8-162">governanceSchedule</span></span>](governanceschedule.md)|<span data-ttu-id="171c8-163">O objeto schedule da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="171c8-163">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="171c8-164">motivo</span><span class="sxs-lookup"><span data-stu-id="171c8-164">reason</span></span>                     |<span data-ttu-id="171c8-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="171c8-165">String</span></span>         |<span data-ttu-id="171c8-166">Uma mensagem fornecida por usuários e administradores ao criar a solicitação sobre por que ela é necessária.</span><span class="sxs-lookup"><span data-stu-id="171c8-166">A message provided by users and administrators when create the request about why it is needed.</span></span>|
|<span data-ttu-id="171c8-167">status</span><span class="sxs-lookup"><span data-stu-id="171c8-167">status</span></span>                     |[<span data-ttu-id="171c8-168">governanceRoleAssignmentRequestStatus</span><span class="sxs-lookup"><span data-stu-id="171c8-168">governanceRoleAssignmentRequestStatus</span></span>](governanceroleassignmentrequeststatus.md)         |<span data-ttu-id="171c8-169">O status da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="171c8-169">The status of the role assignment request.</span></span>|
|<span data-ttu-id="171c8-170">linkedEligibleRoleAssignmentId</span><span class="sxs-lookup"><span data-stu-id="171c8-170">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="171c8-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="171c8-171">String</span></span>        |<span data-ttu-id="171c8-172">Se for uma solicitação de ativação de função, ela representará a id do `eligible assignment` referido; Caso contrário, o valor será `null` .</span><span class="sxs-lookup"><span data-stu-id="171c8-172">If this is a request for role activation, it represents the id of the `eligible assignment` being referred; Otherwise, the value is `null`.</span></span> |

|<span data-ttu-id="171c8-173">Member</span><span class="sxs-lookup"><span data-stu-id="171c8-173">Member</span></span>|<span data-ttu-id="171c8-174">Descrição</span><span class="sxs-lookup"><span data-stu-id="171c8-174">Description</span></span>|
|:---|:---|
|<span data-ttu-id="171c8-175">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="171c8-175">AdminAdd</span></span>|<span data-ttu-id="171c8-176">Os administradores atribuem usuários/grupos a funções.</span><span class="sxs-lookup"><span data-stu-id="171c8-176">Administrators assign users/groups to roles.</span></span>|
|<span data-ttu-id="171c8-177">UserAdd</span><span class="sxs-lookup"><span data-stu-id="171c8-177">UserAdd</span></span>|<span data-ttu-id="171c8-178">Os usuários ativam atribuições qualificadas.</span><span class="sxs-lookup"><span data-stu-id="171c8-178">Users activate eligible assignments.</span></span>|
|<span data-ttu-id="171c8-179">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="171c8-179">AdminUpdate</span></span>|<span data-ttu-id="171c8-180">Os administradores alteram as atribuições de função existentes.</span><span class="sxs-lookup"><span data-stu-id="171c8-180">Administrators change existing role assignments.</span></span>|
|<span data-ttu-id="171c8-181">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="171c8-181">AdminRemove</span></span>|<span data-ttu-id="171c8-182">Os administradores removem usuários/grupos de funções.</span><span class="sxs-lookup"><span data-stu-id="171c8-182">Administrators remove users/groups from roles.</span></span>|
|<span data-ttu-id="171c8-183">UserRemove</span><span class="sxs-lookup"><span data-stu-id="171c8-183">UserRemove</span></span>|<span data-ttu-id="171c8-184">Os usuários desativam as atribuições ativas.</span><span class="sxs-lookup"><span data-stu-id="171c8-184">Users deactivate active assignments.</span></span>|
|<span data-ttu-id="171c8-185">UserExtend</span><span class="sxs-lookup"><span data-stu-id="171c8-185">UserExtend</span></span>|<span data-ttu-id="171c8-186">Os usuários solicitam estender suas atribuições de expiração.</span><span class="sxs-lookup"><span data-stu-id="171c8-186">Users request to extend their expiring assignments.</span></span>|
|<span data-ttu-id="171c8-187">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="171c8-187">AdminExtend</span></span>|<span data-ttu-id="171c8-188">Os administradores estendem atribuições expiradas.</span><span class="sxs-lookup"><span data-stu-id="171c8-188">Administrators extend expiring assignments.</span></span>|
|<span data-ttu-id="171c8-189">UserRenew</span><span class="sxs-lookup"><span data-stu-id="171c8-189">UserRenew</span></span>|<span data-ttu-id="171c8-190">Os usuários solicitam renovar suas atribuições expiradas.</span><span class="sxs-lookup"><span data-stu-id="171c8-190">Users request to renew their expired assignments.</span></span>|
|<span data-ttu-id="171c8-191">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="171c8-191">AdminRenew</span></span>|<span data-ttu-id="171c8-192">Os administradores estendem atribuições expiradas.</span><span class="sxs-lookup"><span data-stu-id="171c8-192">Administrators extend expiring assignments.</span></span>|



## <a name="relationships"></a><span data-ttu-id="171c8-193">Relações</span><span class="sxs-lookup"><span data-stu-id="171c8-193">Relationships</span></span>
| <span data-ttu-id="171c8-194">Relação</span><span class="sxs-lookup"><span data-stu-id="171c8-194">Relationship</span></span> | <span data-ttu-id="171c8-195">Tipo</span><span class="sxs-lookup"><span data-stu-id="171c8-195">Type</span></span>                                |<span data-ttu-id="171c8-196">Descrição</span><span class="sxs-lookup"><span data-stu-id="171c8-196">Description</span></span>|
|:-------------|:----------------------------------|:----------|
|<span data-ttu-id="171c8-197">recurso</span><span class="sxs-lookup"><span data-stu-id="171c8-197">resource</span></span>      |[<span data-ttu-id="171c8-198">governanceResource</span><span class="sxs-lookup"><span data-stu-id="171c8-198">governanceResource</span></span>](../resources/governanceresource.md)            |<span data-ttu-id="171c8-199">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="171c8-199">Read-only.</span></span> <span data-ttu-id="171c8-200">O recurso que a solicitação visa.</span><span class="sxs-lookup"><span data-stu-id="171c8-200">The resource that the request aims to.</span></span> |
|<span data-ttu-id="171c8-201">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="171c8-201">roleDefinition</span></span>|[<span data-ttu-id="171c8-202">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="171c8-202">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="171c8-203">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="171c8-203">Read-only.</span></span> <span data-ttu-id="171c8-204">A definição de função que a solicitação visa.</span><span class="sxs-lookup"><span data-stu-id="171c8-204">The role definition that the request aims to.</span></span> |
|<span data-ttu-id="171c8-205">assunto</span><span class="sxs-lookup"><span data-stu-id="171c8-205">subject</span></span>       |[<span data-ttu-id="171c8-206">governanceSubject</span><span class="sxs-lookup"><span data-stu-id="171c8-206">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="171c8-207">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="171c8-207">Read-only.</span></span> <span data-ttu-id="171c8-208">A entidade de usuário/grupo.</span><span class="sxs-lookup"><span data-stu-id="171c8-208">The user/group principal.</span></span>|

### <a name="json-representation"></a><span data-ttu-id="171c8-209">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="171c8-209">JSON representation</span></span>

<span data-ttu-id="171c8-210">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="171c8-210">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "subjectId": "String",
  "type": "String",
  "assignmentState": "String",
  "reason": "String",
  "requestedDateTime": "String (timestamp)",
  "schedule": {"@odata.type": "microsoft.graph.governanceSchedule"},
  "status": {"@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus"},
  "linkedEligibleRoleAssignmentId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


