---
title: Tipo de recurso governanceRoleAssignment
description: Representa a atribuição de um usuário ou grupo a uma função.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 6d9e1b56a503ffdf1bde6bde6a583b78f8a34851
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722304"
---
# <a name="governanceroleassignment-resource-type"></a><span data-ttu-id="66137-103">Tipo de recurso governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="66137-103">governanceRoleAssignment resource type</span></span>

<span data-ttu-id="66137-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="66137-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="66137-105">Representa a atribuição de um usuário ou grupo a uma função.</span><span class="sxs-lookup"><span data-stu-id="66137-105">Represents the assignment of a user or group to a role.</span></span>

<span data-ttu-id="66137-106">O PIM (Privileged Identity Management) dá suporte a dois tipos de atribuições:</span><span class="sxs-lookup"><span data-stu-id="66137-106">Privileged Identity Management (PIM) supports two types of assignments:</span></span>

1. <span data-ttu-id="66137-107">Atribuição ativa - Representa o acesso direto/ativado aos recursos.</span><span class="sxs-lookup"><span data-stu-id="66137-107">Active assignment - Represents the direct/activated access to resources.</span></span>
2. <span data-ttu-id="66137-108">Atribuição qualificada - representa um estágio intermediário de acesso privilegiado a recursos, entre nenhum acesso e acesso direto.</span><span class="sxs-lookup"><span data-stu-id="66137-108">Eligible assignment - Represents an intermediate stage of privileged access to resources, between no access and direct access.</span></span> <span data-ttu-id="66137-109">Os administradores podem atribuir usuários/grupos com antecedência e, sempre que o acesso for necessário, o acesso é necessário para obter o acesso instantâneo ao recurso `eligible assignment` `activation` por várias `eligible assignment` horas.</span><span class="sxs-lookup"><span data-stu-id="66137-109">Administrators can assign users/groups to `eligible assignment` in advance, and whenever the access is needed, `activation` on the `eligible assignment` is needed to gain the instant access to the resource for several hours.</span></span> <span data-ttu-id="66137-110">Após a ativação, `active assignment` um será criado para os usuários/membros do grupo indicarem o status ativado.</span><span class="sxs-lookup"><span data-stu-id="66137-110">After activation, an `active assignment` will be created for the users/group members to indicate the activated status.</span></span>

## <a name="methods"></a><span data-ttu-id="66137-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="66137-111">Methods</span></span>

| <span data-ttu-id="66137-112">Método</span><span class="sxs-lookup"><span data-stu-id="66137-112">Method</span></span>          | <span data-ttu-id="66137-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="66137-113">Return Type</span></span> |<span data-ttu-id="66137-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="66137-114">Description</span></span>|
|:------------|:--------|:--------|
|[<span data-ttu-id="66137-115">Get</span><span class="sxs-lookup"><span data-stu-id="66137-115">Get</span></span>](../api/governanceroleassignment-get.md) |  [<span data-ttu-id="66137-116">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="66137-116">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md) |<span data-ttu-id="66137-117">Ler propriedades e relações de uma entidade de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="66137-117">Read properties and relationships of a role assignment entity.</span></span>|
|[<span data-ttu-id="66137-118">List</span><span class="sxs-lookup"><span data-stu-id="66137-118">List</span></span>](../api/governanceroleassignment-list.md) | <span data-ttu-id="66137-119">[Coleção governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="66137-119">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="66137-120">Listar uma coleção de atribuições de função em um recurso.</span><span class="sxs-lookup"><span data-stu-id="66137-120">List a collection of role assignments on a resource.</span></span> |
|[<span data-ttu-id="66137-121">Export</span><span class="sxs-lookup"><span data-stu-id="66137-121">Export</span></span>](../api/governanceroleassignment-export.md) | <span data-ttu-id="66137-122">octet-stream</span><span class="sxs-lookup"><span data-stu-id="66137-122">octet-stream</span></span> |<span data-ttu-id="66137-123">Baixe uma coleção de atribuições de função em um recurso e salve como um `.csv` arquivo.</span><span class="sxs-lookup"><span data-stu-id="66137-123">Download a collection of role assignments on a resource and save as a `.csv` file.</span></span>|

<span data-ttu-id="66137-124">Não `POST` , , ou as operações são `PUT` `PATCH` `DELETE` suportadas no conjunto de `roleAssignments` entidades.</span><span class="sxs-lookup"><span data-stu-id="66137-124">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `roleAssignments` entity set.</span></span> <span data-ttu-id="66137-125">Todas as operações de criação, atualização e exclusão são `governanceRoleAssignment` feitas por `governanceRoleAssignmentRequest` .</span><span class="sxs-lookup"><span data-stu-id="66137-125">Any create, update, and delete operations on `governanceRoleAssignment` are done by `governanceRoleAssignmentRequest`.</span></span>

## <a name="properties"></a><span data-ttu-id="66137-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66137-126">Properties</span></span>
| <span data-ttu-id="66137-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66137-127">Property</span></span>  | <span data-ttu-id="66137-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="66137-128">Type</span></span>      |<span data-ttu-id="66137-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="66137-129">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="66137-130">id</span><span class="sxs-lookup"><span data-stu-id="66137-130">id</span></span>         |<span data-ttu-id="66137-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66137-131">String</span></span>     |<span data-ttu-id="66137-132">A ID da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="66137-132">The ID of the role assignment.</span></span> <span data-ttu-id="66137-133">Está no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="66137-133">It is in GUID format.</span></span>|
|<span data-ttu-id="66137-134">resourceId</span><span class="sxs-lookup"><span data-stu-id="66137-134">resourceId</span></span> |<span data-ttu-id="66137-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66137-135">String</span></span>     |<span data-ttu-id="66137-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66137-136">Required.</span></span> <span data-ttu-id="66137-137">A ID do recurso ao qual a atribuição de função está associada.</span><span class="sxs-lookup"><span data-stu-id="66137-137">The ID of the resource which the role assignment is associated with.</span></span> |
|<span data-ttu-id="66137-138">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="66137-138">roleDefinitionId</span></span>|<span data-ttu-id="66137-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66137-139">String</span></span>|<span data-ttu-id="66137-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66137-140">Required.</span></span> <span data-ttu-id="66137-141">A ID da definição de função à qual a atribuição de função está associada.</span><span class="sxs-lookup"><span data-stu-id="66137-141">The ID of the role definition which the role assignment is associated with.</span></span> |
|<span data-ttu-id="66137-142">subjectId</span><span class="sxs-lookup"><span data-stu-id="66137-142">subjectId</span></span>|<span data-ttu-id="66137-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66137-143">String</span></span>       |<span data-ttu-id="66137-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66137-144">Required.</span></span> <span data-ttu-id="66137-145">A ID do assunto ao qual a atribuição de função está associada.</span><span class="sxs-lookup"><span data-stu-id="66137-145">The ID of the subject which the role assignment is associated with.</span></span> |
|<span data-ttu-id="66137-146">linkedEligibleRoleAssignmentId</span><span class="sxs-lookup"><span data-stu-id="66137-146">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="66137-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66137-147">String</span></span>|<span data-ttu-id="66137-148">Se for um e criado devido à `active assignment` ativação em `eligible assignment` um , ele representará a ID `eligible assignment` disso; Caso contrário, o valor será `null` .</span><span class="sxs-lookup"><span data-stu-id="66137-148">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the ID of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |
|<span data-ttu-id="66137-149">externalId</span><span class="sxs-lookup"><span data-stu-id="66137-149">externalId</span></span>   |<span data-ttu-id="66137-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66137-150">String</span></span>     |<span data-ttu-id="66137-151">A ID externa do recurso usado para identificar a atribuição de função no provedor.</span><span class="sxs-lookup"><span data-stu-id="66137-151">The external ID the resource that is used to identify the role assignment in the provider.</span></span>|
|<span data-ttu-id="66137-152">startDateTime</span><span class="sxs-lookup"><span data-stu-id="66137-152">startDateTime</span></span>|<span data-ttu-id="66137-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66137-153">DateTimeOffset</span></span>|<span data-ttu-id="66137-154">A hora de início da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="66137-154">The start time of the role assignment.</span></span> <span data-ttu-id="66137-155">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="66137-155">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="66137-156">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="66137-156">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="66137-157">endDateTime</span><span class="sxs-lookup"><span data-stu-id="66137-157">endDateTime</span></span>|<span data-ttu-id="66137-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66137-158">DateTimeOffset</span></span>|<span data-ttu-id="66137-159">Para uma atribuição de função não permanente, este é o momento em que a atribuição de função será expirada.</span><span class="sxs-lookup"><span data-stu-id="66137-159">For a non-permanent role assignment, this is the time when the role assignment will be expired.</span></span> <span data-ttu-id="66137-160">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="66137-160">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="66137-161">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="66137-161">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="66137-162">assignmentState</span><span class="sxs-lookup"><span data-stu-id="66137-162">assignmentState</span></span>|<span data-ttu-id="66137-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66137-163">String</span></span>  |<span data-ttu-id="66137-164">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="66137-164">The state of the assignment.</span></span> <span data-ttu-id="66137-165">O valor pode ser</span><span class="sxs-lookup"><span data-stu-id="66137-165">The value can be</span></span> <ul><li> <span data-ttu-id="66137-166">`Eligible` para atribuição qualificada</span><span class="sxs-lookup"><span data-stu-id="66137-166">`Eligible` for eligible assignment</span></span></li><li> <span data-ttu-id="66137-167">`Active` - se ele for atribuído diretamente pelos administradores ou ativado em uma `Active` atribuição qualificada pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="66137-167">`Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span></li></ul>|
|<span data-ttu-id="66137-168">memberType</span><span class="sxs-lookup"><span data-stu-id="66137-168">memberType</span></span>|<span data-ttu-id="66137-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66137-169">String</span></span>      |<span data-ttu-id="66137-170">O tipo de membro.</span><span class="sxs-lookup"><span data-stu-id="66137-170">The type of member.</span></span> <span data-ttu-id="66137-171">O valor pode ser:</span><span class="sxs-lookup"><span data-stu-id="66137-171">The value can be:</span></span> <ul><li><span data-ttu-id="66137-172">`Inherited` - a atribuição de função é herdada de um escopo de recurso pai</span><span class="sxs-lookup"><span data-stu-id="66137-172">`Inherited` - the role assignment is inherited from a parent resource scope</span></span></li><li><span data-ttu-id="66137-173">`Group`- a atribuição de função não é herdada, mas vem da associação de uma atribuição de grupo</span><span class="sxs-lookup"><span data-stu-id="66137-173">`Group`- the role assignment is not inherited, but comes from the membership of a group assignment</span></span></li><li><span data-ttu-id="66137-174">`User` - a atribuição de função não é herdada nem de uma atribuição de grupo.</span><span class="sxs-lookup"><span data-stu-id="66137-174">`User` - the role assignment is neither inherited nor from a group assignment.</span></span></li></ul>|


## <a name="relationships"></a><span data-ttu-id="66137-175">Relações</span><span class="sxs-lookup"><span data-stu-id="66137-175">Relationships</span></span>
| <span data-ttu-id="66137-176">Relação</span><span class="sxs-lookup"><span data-stu-id="66137-176">Relationship</span></span> | <span data-ttu-id="66137-177">Tipo</span><span class="sxs-lookup"><span data-stu-id="66137-177">Type</span></span>   |<span data-ttu-id="66137-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="66137-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66137-179">recurso</span><span class="sxs-lookup"><span data-stu-id="66137-179">resource</span></span>|[<span data-ttu-id="66137-180">governanceResource</span><span class="sxs-lookup"><span data-stu-id="66137-180">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="66137-181">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66137-181">Read-only.</span></span> <span data-ttu-id="66137-182">O recurso associado à atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="66137-182">The resource associated with the role assignment.</span></span> |
|<span data-ttu-id="66137-183">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="66137-183">roleDefinition</span></span>|[<span data-ttu-id="66137-184">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="66137-184">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="66137-185">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66137-185">Read-only.</span></span> <span data-ttu-id="66137-186">A definição de função associada à atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="66137-186">The role definition associated with the role assignment.</span></span> |
|<span data-ttu-id="66137-187">assunto</span><span class="sxs-lookup"><span data-stu-id="66137-187">subject</span></span>|[<span data-ttu-id="66137-188">governanceSubject</span><span class="sxs-lookup"><span data-stu-id="66137-188">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="66137-189">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66137-189">Read-only.</span></span> <span data-ttu-id="66137-190">O assunto associado à atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="66137-190">The subject associated with the role assignment.</span></span> |
|<span data-ttu-id="66137-191">linkedEligibleRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="66137-191">linkedEligibleRoleAssignment</span></span>|[<span data-ttu-id="66137-192">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="66137-192">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md)|<span data-ttu-id="66137-193">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66137-193">Read-only.</span></span> <span data-ttu-id="66137-194">Se for um `active assignment` e criado devido à ativação em um , ele `eligible assignment` representará o objeto disso `eligible assignment` ; Caso contrário, o valor será `null` .</span><span class="sxs-lookup"><span data-stu-id="66137-194">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the object of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="66137-195">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66137-195">JSON representation</span></span>

<span data-ttu-id="66137-196">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="66137-196">Here is a JSON representation of the resource.</span></span>


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


