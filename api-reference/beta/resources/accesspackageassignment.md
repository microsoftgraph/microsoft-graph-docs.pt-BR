---
title: tipo de recurso accessPackageAssignment
description: Uma atribuição de pacote do Access é uma atribuição de um pacote do Access a um assunto específico, por um período de tempo.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fd85461a4429801aad5145256c711278789c95ed
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000704"
---
# <a name="accesspackageassignment-resource-type"></a><span data-ttu-id="72b00-103">tipo de recurso accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="72b00-103">accessPackageAssignment resource type</span></span>

<span data-ttu-id="72b00-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72b00-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72b00-105">No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma atribuição de pacote de acesso é uma atribuição de um pacote do Access a um assunto específico, por um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="72b00-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment is an assignment of an access package to a particular subject, for a period of time.</span></span>  <span data-ttu-id="72b00-106">Por exemplo, uma atribuição de pacote de acesso pode indicar que o usuário Alice recebeu acesso por meio do pacote de acesso vendas no período de janeiro de 2019 a 2019 de julho.</span><span class="sxs-lookup"><span data-stu-id="72b00-106">For example, an access package assignment can state that user Alice has been assigned access via the access package Sales for the period January 2019 through July 2019.</span></span>

## <a name="methods"></a><span data-ttu-id="72b00-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="72b00-107">Methods</span></span>

| <span data-ttu-id="72b00-108">Método</span><span class="sxs-lookup"><span data-stu-id="72b00-108">Method</span></span>       | <span data-ttu-id="72b00-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="72b00-109">Return Type</span></span> | <span data-ttu-id="72b00-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="72b00-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="72b00-111">Listar accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="72b00-111">List accessPackageAssignments</span></span>](../api/accesspackageassignment-list.md) | <span data-ttu-id="72b00-112">coleção [accessPackageAssignment](accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="72b00-112">[accessPackageAssignment](accesspackageassignment.md) collection</span></span> | <span data-ttu-id="72b00-113">Recupere uma lista de objetos **accesspackageassignment** .</span><span class="sxs-lookup"><span data-stu-id="72b00-113">Retrieve a list of **accesspackageassignment** objects.</span></span> |

><span data-ttu-id="72b00-114">**Observação:** Você não pode usar um método para criar ou remover uma atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="72b00-114">**Note:** You can't use a method to create or remove an access package assignment.</span></span> <span data-ttu-id="72b00-115">Em vez disso, um cliente que deseja solicitar uma atribuição de pacote do Access para um usuário ou remover uma atribuição de pacote de acesso de um usuário, pode [criar um accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).</span><span class="sxs-lookup"><span data-stu-id="72b00-115">Instead, a client that wants to request an access package assignment for a user, or remove an access package assignment from a user, can [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).</span></span>

## <a name="properties"></a><span data-ttu-id="72b00-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="72b00-116">Properties</span></span>

| <span data-ttu-id="72b00-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="72b00-117">Property</span></span>     | <span data-ttu-id="72b00-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="72b00-118">Type</span></span>        | <span data-ttu-id="72b00-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="72b00-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="72b00-120">accessPackageId</span><span class="sxs-lookup"><span data-stu-id="72b00-120">accessPackageId</span></span>|<span data-ttu-id="72b00-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72b00-121">String</span></span>|<span data-ttu-id="72b00-122">O identificador do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="72b00-122">The identifier of the access package.</span></span> <span data-ttu-id="72b00-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b00-123">Read-only.</span></span>|
|<span data-ttu-id="72b00-124">assignmentPolicyId</span><span class="sxs-lookup"><span data-stu-id="72b00-124">assignmentPolicyId</span></span>|<span data-ttu-id="72b00-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72b00-125">String</span></span>|<span data-ttu-id="72b00-126">O identificador da política de atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="72b00-126">The identifier of the access package assignment policy.</span></span> <span data-ttu-id="72b00-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b00-127">Read-only.</span></span>|
|<span data-ttu-id="72b00-128">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="72b00-128">assignmentState</span></span>|<span data-ttu-id="72b00-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72b00-129">String</span></span>|<span data-ttu-id="72b00-130">O estado da atribuição do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="72b00-130">The state of the access package assignment.</span></span> <span data-ttu-id="72b00-131">Os valores possíveis são `Delivering` , `Delivered` , ou `Expired` .</span><span class="sxs-lookup"><span data-stu-id="72b00-131">Possible values are `Delivering`, `Delivered`, or `Expired`.</span></span> <span data-ttu-id="72b00-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b00-132">Read-only.</span></span>|
|<span data-ttu-id="72b00-133">assignmentStatus</span><span class="sxs-lookup"><span data-stu-id="72b00-133">assignmentStatus</span></span>|<span data-ttu-id="72b00-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72b00-134">String</span></span>|<span data-ttu-id="72b00-135">Mais informações sobre o ciclo de vida da atribuição.</span><span class="sxs-lookup"><span data-stu-id="72b00-135">More information about the assignment lifecycle.</span></span>  <span data-ttu-id="72b00-136">Os valores possíveis incluem `Delivering` ,, `Delivered` `NearExpiry1DayNotificationTriggered` ou `ExpiredNotificationTriggered` .</span><span class="sxs-lookup"><span data-stu-id="72b00-136">Possible values include `Delivering`, `Delivered`, `NearExpiry1DayNotificationTriggered`, or `ExpiredNotificationTriggered`.</span></span>  <span data-ttu-id="72b00-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b00-137">Read-only.</span></span>|
|<span data-ttu-id="72b00-138">catalogID</span><span class="sxs-lookup"><span data-stu-id="72b00-138">catalogId</span></span>|<span data-ttu-id="72b00-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72b00-139">String</span></span>|<span data-ttu-id="72b00-140">O identificador do catálogo que contém o pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="72b00-140">The identifier of the catalog containing the access package.</span></span> <span data-ttu-id="72b00-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b00-141">Read-only.</span></span>|
|<span data-ttu-id="72b00-142">expiredDateTime</span><span class="sxs-lookup"><span data-stu-id="72b00-142">expiredDateTime</span></span>|<span data-ttu-id="72b00-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72b00-143">DateTimeOffset</span></span>|<span data-ttu-id="72b00-p108">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="72b00-p108">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="72b00-146">id</span><span class="sxs-lookup"><span data-stu-id="72b00-146">id</span></span>|<span data-ttu-id="72b00-147">String</span><span class="sxs-lookup"><span data-stu-id="72b00-147">String</span></span>| <span data-ttu-id="72b00-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b00-148">Read-only.</span></span>|
|<span data-ttu-id="72b00-149">Extended</span><span class="sxs-lookup"><span data-stu-id="72b00-149">isExtended</span></span>|<span data-ttu-id="72b00-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="72b00-150">Boolean</span></span>|<span data-ttu-id="72b00-151">Indica se a atribuição de pacote de acesso é estendida.</span><span class="sxs-lookup"><span data-stu-id="72b00-151">Indicates whether the access package assignment is extended.</span></span> <span data-ttu-id="72b00-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b00-152">Read-only.</span></span>|
|<span data-ttu-id="72b00-153">targetId</span><span class="sxs-lookup"><span data-stu-id="72b00-153">targetId</span></span>|<span data-ttu-id="72b00-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72b00-154">String</span></span>| <span data-ttu-id="72b00-155">A ID do assunto com a atribuição.</span><span class="sxs-lookup"><span data-stu-id="72b00-155">The ID of the subject with the assignment.</span></span> <span data-ttu-id="72b00-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b00-156">Read-only.</span></span>|
|<span data-ttu-id="72b00-157">Cronograma</span><span class="sxs-lookup"><span data-stu-id="72b00-157">schedule</span></span>|[<span data-ttu-id="72b00-158">requestSchedule</span><span class="sxs-lookup"><span data-stu-id="72b00-158">requestSchedule</span></span>](requestschedule.md)| <span data-ttu-id="72b00-159">Quando a atribuição de acesso deve estar no local.</span><span class="sxs-lookup"><span data-stu-id="72b00-159">When the access assignment is to be in place.</span></span> <span data-ttu-id="72b00-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b00-160">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72b00-161">Relações</span><span class="sxs-lookup"><span data-stu-id="72b00-161">Relationships</span></span>

| <span data-ttu-id="72b00-162">Relação</span><span class="sxs-lookup"><span data-stu-id="72b00-162">Relationship</span></span> | <span data-ttu-id="72b00-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="72b00-163">Type</span></span>        | <span data-ttu-id="72b00-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="72b00-164">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="72b00-165">accessPackage</span><span class="sxs-lookup"><span data-stu-id="72b00-165">accessPackage</span></span>|[<span data-ttu-id="72b00-166">accessPackage</span><span class="sxs-lookup"><span data-stu-id="72b00-166">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="72b00-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b00-167">Read-only.</span></span> <span data-ttu-id="72b00-168">Anulável.</span><span class="sxs-lookup"><span data-stu-id="72b00-168">Nullable.</span></span>|
|<span data-ttu-id="72b00-169">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="72b00-169">accessPackageAssignmentPolicy</span></span>|[<span data-ttu-id="72b00-170">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="72b00-170">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md)| <span data-ttu-id="72b00-171">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b00-171">Read-only.</span></span> <span data-ttu-id="72b00-172">Anulável.</span><span class="sxs-lookup"><span data-stu-id="72b00-172">Nullable.</span></span>|
|<span data-ttu-id="72b00-173">accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="72b00-173">accessPackageAssignmentResourceRoles</span></span>|<span data-ttu-id="72b00-174">coleção [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="72b00-174">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span>| <span data-ttu-id="72b00-175">As funções de recurso entregues ao usuário de destino para esta atribuição.</span><span class="sxs-lookup"><span data-stu-id="72b00-175">The resource roles delivered to the target user for this assignment.</span></span> <span data-ttu-id="72b00-176">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b00-176">Read-only.</span></span> <span data-ttu-id="72b00-177">Anulável.</span><span class="sxs-lookup"><span data-stu-id="72b00-177">Nullable.</span></span>|
|<span data-ttu-id="72b00-178">destino</span><span class="sxs-lookup"><span data-stu-id="72b00-178">target</span></span>|[<span data-ttu-id="72b00-179">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="72b00-179">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="72b00-180">O assunto da atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="72b00-180">The subject of the access package assignment.</span></span> <span data-ttu-id="72b00-181">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b00-181">Read-only.</span></span> <span data-ttu-id="72b00-182">Anulável.</span><span class="sxs-lookup"><span data-stu-id="72b00-182">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="72b00-183">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="72b00-183">JSON representation</span></span>

<span data-ttu-id="72b00-184">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="72b00-184">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignment",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
   "id":"9bdae7b4-6ece-487b-9eb8-9679dbd67aa2",
   "catalogId":"cc30dc98-6d3c-4fa0-bed8-fd76d0efd993",
   "accessPackageId":"e3f47362-993f-4fcb-8a38-532ffca16150",
   "assignmentPolicyId":"63ebd106-8116-40e7-a0ab-01ae475d11bb",
   "targetId":"ab4291f6-66b7-42bf-b597-a05b29414f5c",
   "assignmentStatus":"ExpiredNotificationTriggered",
   "assignmentState":"Expired",
   "isExtended":false,
   "expiredDateTime":"2019-04-25T23:45:40.42Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


