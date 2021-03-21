---
title: Tipo de recurso governanceRoleAssignment
description: Representa a atribuição de um usuário ou grupo a uma função.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 532ea3c1d8fe5b1bc1128994c96c493774e9b19b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964559"
---
# <a name="governanceroleassignment-resource-type"></a><span data-ttu-id="81df1-103">Tipo de recurso governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="81df1-103">governanceRoleAssignment resource type</span></span>

<span data-ttu-id="81df1-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="81df1-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="81df1-105">Representa a atribuição de um usuário ou grupo a uma função.</span><span class="sxs-lookup"><span data-stu-id="81df1-105">Represents the assignment of a user or group to a role.</span></span>

<span data-ttu-id="81df1-106">O PIM (Privileged Identity Management) dá suporte a dois tipos de atribuições:</span><span class="sxs-lookup"><span data-stu-id="81df1-106">Privileged Identity Management (PIM) supports two types of assignments:</span></span>

1. <span data-ttu-id="81df1-107">Atribuição ativa - Representa o acesso direto/ativado aos recursos.</span><span class="sxs-lookup"><span data-stu-id="81df1-107">Active assignment - Represents the direct/activated access to resources.</span></span>
2. <span data-ttu-id="81df1-108">Atribuição qualificada - representa um estágio intermediário de acesso privilegiado a recursos, entre nenhum acesso e acesso direto.</span><span class="sxs-lookup"><span data-stu-id="81df1-108">Eligible assignment - Represents an intermediate stage of privileged access to resources, between no access and direct access.</span></span> <span data-ttu-id="81df1-109">Os administradores podem atribuir usuários/grupos com antecedência e, sempre que o acesso for necessário, o acesso é necessário para obter o acesso instantâneo ao recurso `eligible assignment` `activation` por várias `eligible assignment` horas.</span><span class="sxs-lookup"><span data-stu-id="81df1-109">Administrators can assign users/groups to `eligible assignment` in advance, and whenever the access is needed, `activation` on the `eligible assignment` is needed to gain the instant access to the resource for several hours.</span></span> <span data-ttu-id="81df1-110">Após a ativação, `active assignment` um será criado para os usuários/membros do grupo indicarem o status ativado.</span><span class="sxs-lookup"><span data-stu-id="81df1-110">After activation, an `active assignment` will be created for the users/group members to indicate the activated status.</span></span>

## <a name="methods"></a><span data-ttu-id="81df1-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="81df1-111">Methods</span></span>

| <span data-ttu-id="81df1-112">Método</span><span class="sxs-lookup"><span data-stu-id="81df1-112">Method</span></span>          | <span data-ttu-id="81df1-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="81df1-113">Return Type</span></span> |<span data-ttu-id="81df1-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="81df1-114">Description</span></span>|
|:------------|:--------|:--------|
|[<span data-ttu-id="81df1-115">Get</span><span class="sxs-lookup"><span data-stu-id="81df1-115">Get</span></span>](../api/governanceroleassignment-get.md) |  [<span data-ttu-id="81df1-116">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="81df1-116">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md) |<span data-ttu-id="81df1-117">Ler propriedades e relações de uma entidade de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="81df1-117">Read properties and relationships of a role assignment entity.</span></span>|
|[<span data-ttu-id="81df1-118">Lista</span><span class="sxs-lookup"><span data-stu-id="81df1-118">List</span></span>](../api/governanceroleassignment-list.md) | <span data-ttu-id="81df1-119">[Coleção governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="81df1-119">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="81df1-120">Listar uma coleção de atribuições de função em um recurso.</span><span class="sxs-lookup"><span data-stu-id="81df1-120">List a collection of role assignments on a resource.</span></span> |
|[<span data-ttu-id="81df1-121">Export</span><span class="sxs-lookup"><span data-stu-id="81df1-121">Export</span></span>](../api/governanceroleassignment-export.md) | <span data-ttu-id="81df1-122">octet-stream</span><span class="sxs-lookup"><span data-stu-id="81df1-122">octet-stream</span></span> |<span data-ttu-id="81df1-123">Baixe uma coleção de atribuições de função em um recurso e salve como um `.csv` arquivo.</span><span class="sxs-lookup"><span data-stu-id="81df1-123">Download a collection of role assignments on a resource and save as a `.csv` file.</span></span>|

<span data-ttu-id="81df1-124">Não `POST` , , ou as operações são `PUT` `PATCH` `DELETE` suportadas no conjunto de `roleAssignments` entidades.</span><span class="sxs-lookup"><span data-stu-id="81df1-124">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `roleAssignments` entity set.</span></span> <span data-ttu-id="81df1-125">Todas as operações de criação, atualização e exclusão são `governanceRoleAssignment` feitas por `governanceRoleAssignmentRequest` .</span><span class="sxs-lookup"><span data-stu-id="81df1-125">Any create, update, and delete operations on `governanceRoleAssignment` are done by `governanceRoleAssignmentRequest`.</span></span>

## <a name="properties"></a><span data-ttu-id="81df1-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81df1-126">Properties</span></span>
| <span data-ttu-id="81df1-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81df1-127">Property</span></span>  | <span data-ttu-id="81df1-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="81df1-128">Type</span></span>      |<span data-ttu-id="81df1-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="81df1-129">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="81df1-130">id</span><span class="sxs-lookup"><span data-stu-id="81df1-130">id</span></span>         |<span data-ttu-id="81df1-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81df1-131">String</span></span>     |<span data-ttu-id="81df1-132">A ID da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="81df1-132">The ID of the role assignment.</span></span> <span data-ttu-id="81df1-133">Está no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="81df1-133">It is in GUID format.</span></span>|
|<span data-ttu-id="81df1-134">resourceId</span><span class="sxs-lookup"><span data-stu-id="81df1-134">resourceId</span></span> |<span data-ttu-id="81df1-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81df1-135">String</span></span>     |<span data-ttu-id="81df1-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81df1-136">Required.</span></span> <span data-ttu-id="81df1-137">A ID do recurso ao qual a atribuição de função está associada.</span><span class="sxs-lookup"><span data-stu-id="81df1-137">The ID of the resource which the role assignment is associated with.</span></span> |
|<span data-ttu-id="81df1-138">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="81df1-138">roleDefinitionId</span></span>|<span data-ttu-id="81df1-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81df1-139">String</span></span>|<span data-ttu-id="81df1-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81df1-140">Required.</span></span> <span data-ttu-id="81df1-141">A ID da definição de função à qual a atribuição de função está associada.</span><span class="sxs-lookup"><span data-stu-id="81df1-141">The ID of the role definition which the role assignment is associated with.</span></span> |
|<span data-ttu-id="81df1-142">subjectId</span><span class="sxs-lookup"><span data-stu-id="81df1-142">subjectId</span></span>|<span data-ttu-id="81df1-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81df1-143">String</span></span>       |<span data-ttu-id="81df1-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81df1-144">Required.</span></span> <span data-ttu-id="81df1-145">A ID do assunto ao qual a atribuição de função está associada.</span><span class="sxs-lookup"><span data-stu-id="81df1-145">The ID of the subject which the role assignment is associated with.</span></span> |
|<span data-ttu-id="81df1-146">linkedEligibleRoleAssignmentId</span><span class="sxs-lookup"><span data-stu-id="81df1-146">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="81df1-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81df1-147">String</span></span>|<span data-ttu-id="81df1-148">Se for um e criado devido à `active assignment` ativação em `eligible assignment` um , ele representará a ID `eligible assignment` disso; Caso contrário, o valor será `null` .</span><span class="sxs-lookup"><span data-stu-id="81df1-148">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the ID of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |
|<span data-ttu-id="81df1-149">externalId</span><span class="sxs-lookup"><span data-stu-id="81df1-149">externalId</span></span>   |<span data-ttu-id="81df1-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81df1-150">String</span></span>     |<span data-ttu-id="81df1-151">A ID externa do recurso usado para identificar a atribuição de função no provedor.</span><span class="sxs-lookup"><span data-stu-id="81df1-151">The external ID the resource that is used to identify the role assignment in the provider.</span></span>|
|<span data-ttu-id="81df1-152">startDateTime</span><span class="sxs-lookup"><span data-stu-id="81df1-152">startDateTime</span></span>|<span data-ttu-id="81df1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81df1-153">DateTimeOffset</span></span>|<span data-ttu-id="81df1-154">A hora de início da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="81df1-154">The start time of the role assignment.</span></span> <span data-ttu-id="81df1-155">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="81df1-155">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="81df1-156">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="81df1-156">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="81df1-157">endDateTime</span><span class="sxs-lookup"><span data-stu-id="81df1-157">endDateTime</span></span>|<span data-ttu-id="81df1-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81df1-158">DateTimeOffset</span></span>|<span data-ttu-id="81df1-159">Para uma atribuição de função não permanente, este é o momento em que a atribuição de função será expirada.</span><span class="sxs-lookup"><span data-stu-id="81df1-159">For a non-permanent role assignment, this is the time when the role assignment will be expired.</span></span> <span data-ttu-id="81df1-160">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="81df1-160">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="81df1-161">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="81df1-161">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="81df1-162">assignmentState</span><span class="sxs-lookup"><span data-stu-id="81df1-162">assignmentState</span></span>|<span data-ttu-id="81df1-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81df1-163">String</span></span>  |<span data-ttu-id="81df1-164">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="81df1-164">The state of the assignment.</span></span> <span data-ttu-id="81df1-165">O valor pode ser para atribuição qualificada ou se ele for atribuído diretamente pelos administradores ou ativado em uma atribuição qualificada `Eligible` `Active` pelos `Active` usuários.</span><span class="sxs-lookup"><span data-stu-id="81df1-165">The value can be `Eligible` for eligible assignment or `Active` if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="81df1-166">memberType</span><span class="sxs-lookup"><span data-stu-id="81df1-166">memberType</span></span>|<span data-ttu-id="81df1-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81df1-167">String</span></span>      |<span data-ttu-id="81df1-168">O tipo de membro.</span><span class="sxs-lookup"><span data-stu-id="81df1-168">The type of member.</span></span> <span data-ttu-id="81df1-169">O valor pode ser: (se a atribuição de função for herdada de um escopo de recurso pai), (se a atribuição de função não for herdada, mas vier da associação de uma atribuição de grupo) ou (se a atribuição de função não for herdada nem de uma atribuição de `Inherited` `Group` `User` grupo).</span><span class="sxs-lookup"><span data-stu-id="81df1-169">The value can be: `Inherited` (if the role assignment is inherited from a parent resource scope), `Group` (if the role assignment is not inherited, but comes from the membership of a group assignment), or `User` (if the role assignment is neither inherited nor from a group assignment).</span></span>|


## <a name="relationships"></a><span data-ttu-id="81df1-170">Relações</span><span class="sxs-lookup"><span data-stu-id="81df1-170">Relationships</span></span>
| <span data-ttu-id="81df1-171">Relação</span><span class="sxs-lookup"><span data-stu-id="81df1-171">Relationship</span></span> | <span data-ttu-id="81df1-172">Tipo</span><span class="sxs-lookup"><span data-stu-id="81df1-172">Type</span></span>   |<span data-ttu-id="81df1-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="81df1-173">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81df1-174">recurso</span><span class="sxs-lookup"><span data-stu-id="81df1-174">resource</span></span>|[<span data-ttu-id="81df1-175">governanceResource</span><span class="sxs-lookup"><span data-stu-id="81df1-175">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="81df1-176">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="81df1-176">Read-only.</span></span> <span data-ttu-id="81df1-177">O recurso associado à atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="81df1-177">The resource associated with the role assignment.</span></span> |
|<span data-ttu-id="81df1-178">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="81df1-178">roleDefinition</span></span>|[<span data-ttu-id="81df1-179">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="81df1-179">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="81df1-180">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="81df1-180">Read-only.</span></span> <span data-ttu-id="81df1-181">A definição de função associada à atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="81df1-181">The role definition associated with the role assignment.</span></span> |
|<span data-ttu-id="81df1-182">assunto</span><span class="sxs-lookup"><span data-stu-id="81df1-182">subject</span></span>|[<span data-ttu-id="81df1-183">governanceSubject</span><span class="sxs-lookup"><span data-stu-id="81df1-183">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="81df1-184">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="81df1-184">Read-only.</span></span> <span data-ttu-id="81df1-185">O assunto associado à atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="81df1-185">The subject associated with the role assignment.</span></span> |
|<span data-ttu-id="81df1-186">linkedEligibleRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="81df1-186">linkedEligibleRoleAssignment</span></span>|[<span data-ttu-id="81df1-187">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="81df1-187">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md)|<span data-ttu-id="81df1-188">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="81df1-188">Read-only.</span></span> <span data-ttu-id="81df1-189">Se for um `active assignment` e criado devido à ativação em um , ele `eligible assignment` representará o objeto disso `eligible assignment` ; Caso contrário, o valor será `null` .</span><span class="sxs-lookup"><span data-stu-id="81df1-189">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the object of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="81df1-190">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81df1-190">JSON representation</span></span>

<span data-ttu-id="81df1-191">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81df1-191">Here is a JSON representation of the resource.</span></span>


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


