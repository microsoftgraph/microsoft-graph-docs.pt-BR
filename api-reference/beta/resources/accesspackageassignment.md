---
title: Tipo de recurso accessPackageAssignment
description: Uma atribuição de pacote de acesso é uma atribuição de um pacote de acesso a um assunto específico, por um período de tempo.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3a7d9a947490676b48a170130fac2bf9e776c183
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155619"
---
# <a name="accesspackageassignment-resource-type"></a><span data-ttu-id="d4422-103">Tipo de recurso accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="d4422-103">accessPackageAssignment resource type</span></span>

<span data-ttu-id="d4422-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4422-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4422-105">No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)uma atribuição de pacote de acesso é uma atribuição de um pacote de acesso a um assunto específico, por um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="d4422-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment is an assignment of an access package to a particular subject, for a period of time.</span></span>  <span data-ttu-id="d4422-106">Por exemplo, uma atribuição de pacote de acesso pode dizer que a usuária Alice recebeu acesso por meio do pacote de acesso Vendas do período de janeiro de 2019 a julho de 2019.</span><span class="sxs-lookup"><span data-stu-id="d4422-106">For example, an access package assignment can state that user Alice has been assigned access via the access package Sales for the period January 2019 through July 2019.</span></span>

## <a name="methods"></a><span data-ttu-id="d4422-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="d4422-107">Methods</span></span>

| <span data-ttu-id="d4422-108">Método</span><span class="sxs-lookup"><span data-stu-id="d4422-108">Method</span></span>       | <span data-ttu-id="d4422-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d4422-109">Return Type</span></span> | <span data-ttu-id="d4422-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4422-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d4422-111">Listar accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="d4422-111">List accessPackageAssignments</span></span>](../api/accesspackageassignment-list.md) | <span data-ttu-id="d4422-112">[Coleção accessPackageAssignment](accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d4422-112">[accessPackageAssignment](accesspackageassignment.md) collection</span></span> | <span data-ttu-id="d4422-113">Recupere uma lista de **objetos accesspackageassignment.**</span><span class="sxs-lookup"><span data-stu-id="d4422-113">Retrieve a list of **accesspackageassignment** objects.</span></span> |

><span data-ttu-id="d4422-114">**Observação:** Você não pode usar um método para criar ou remover uma atribuição de pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="d4422-114">**Note:** You can't use a method to create or remove an access package assignment.</span></span> <span data-ttu-id="d4422-115">Em vez disso, um cliente que deseja solicitar uma atribuição de pacote de acesso para um usuário ou remover uma atribuição de pacote de acesso de um usuário, pode criar um [accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).</span><span class="sxs-lookup"><span data-stu-id="d4422-115">Instead, a client that wants to request an access package assignment for a user, or remove an access package assignment from a user, can [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d4422-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d4422-116">Properties</span></span>

| <span data-ttu-id="d4422-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4422-117">Property</span></span>     | <span data-ttu-id="d4422-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4422-118">Type</span></span>        | <span data-ttu-id="d4422-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4422-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d4422-120">accessPackageId</span><span class="sxs-lookup"><span data-stu-id="d4422-120">accessPackageId</span></span>|<span data-ttu-id="d4422-121">String</span><span class="sxs-lookup"><span data-stu-id="d4422-121">String</span></span>|<span data-ttu-id="d4422-122">O identificador do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="d4422-122">The identifier of the access package.</span></span> <span data-ttu-id="d4422-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d4422-123">Read-only.</span></span>|
|<span data-ttu-id="d4422-124">assignmentPolicyId</span><span class="sxs-lookup"><span data-stu-id="d4422-124">assignmentPolicyId</span></span>|<span data-ttu-id="d4422-125">String</span><span class="sxs-lookup"><span data-stu-id="d4422-125">String</span></span>|<span data-ttu-id="d4422-126">O identificador da política de atribuição do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="d4422-126">The identifier of the access package assignment policy.</span></span> <span data-ttu-id="d4422-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d4422-127">Read-only.</span></span>|
|<span data-ttu-id="d4422-128">assignmentState</span><span class="sxs-lookup"><span data-stu-id="d4422-128">assignmentState</span></span>|<span data-ttu-id="d4422-129">String</span><span class="sxs-lookup"><span data-stu-id="d4422-129">String</span></span>|<span data-ttu-id="d4422-130">O estado da atribuição do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="d4422-130">The state of the access package assignment.</span></span> <span data-ttu-id="d4422-131">Os valores possíveis `Delivering` `Delivered` são , ou `Expired` .</span><span class="sxs-lookup"><span data-stu-id="d4422-131">Possible values are `Delivering`, `Delivered`, or `Expired`.</span></span> <span data-ttu-id="d4422-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d4422-132">Read-only.</span></span>|
|<span data-ttu-id="d4422-133">assignmentStatus</span><span class="sxs-lookup"><span data-stu-id="d4422-133">assignmentStatus</span></span>|<span data-ttu-id="d4422-134">String</span><span class="sxs-lookup"><span data-stu-id="d4422-134">String</span></span>|<span data-ttu-id="d4422-135">Mais informações sobre o ciclo de vida de atribuição.</span><span class="sxs-lookup"><span data-stu-id="d4422-135">More information about the assignment lifecycle.</span></span>  <span data-ttu-id="d4422-136">Os valores possíveis `Delivering` `Delivered` incluem `NearExpiry1DayNotificationTriggered` , ou `ExpiredNotificationTriggered` .</span><span class="sxs-lookup"><span data-stu-id="d4422-136">Possible values include `Delivering`, `Delivered`, `NearExpiry1DayNotificationTriggered`, or `ExpiredNotificationTriggered`.</span></span>  <span data-ttu-id="d4422-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d4422-137">Read-only.</span></span>|
|<span data-ttu-id="d4422-138">catalogId</span><span class="sxs-lookup"><span data-stu-id="d4422-138">catalogId</span></span>|<span data-ttu-id="d4422-139">String</span><span class="sxs-lookup"><span data-stu-id="d4422-139">String</span></span>|<span data-ttu-id="d4422-140">O identificador do catálogo que contém o pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="d4422-140">The identifier of the catalog containing the access package.</span></span> <span data-ttu-id="d4422-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d4422-141">Read-only.</span></span>|
|<span data-ttu-id="d4422-142">expiredDateTime</span><span class="sxs-lookup"><span data-stu-id="d4422-142">expiredDateTime</span></span>|<span data-ttu-id="d4422-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4422-143">DateTimeOffset</span></span>|<span data-ttu-id="d4422-p108">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d4422-p108">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d4422-146">id</span><span class="sxs-lookup"><span data-stu-id="d4422-146">id</span></span>|<span data-ttu-id="d4422-147">String</span><span class="sxs-lookup"><span data-stu-id="d4422-147">String</span></span>| <span data-ttu-id="d4422-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d4422-148">Read-only.</span></span>|
|<span data-ttu-id="d4422-149">isExtended</span><span class="sxs-lookup"><span data-stu-id="d4422-149">isExtended</span></span>|<span data-ttu-id="d4422-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4422-150">Boolean</span></span>|<span data-ttu-id="d4422-151">Indica se a atribuição do pacote de acesso foi estendida.</span><span class="sxs-lookup"><span data-stu-id="d4422-151">Indicates whether the access package assignment is extended.</span></span> <span data-ttu-id="d4422-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d4422-152">Read-only.</span></span>|
|<span data-ttu-id="d4422-153">targetId</span><span class="sxs-lookup"><span data-stu-id="d4422-153">targetId</span></span>|<span data-ttu-id="d4422-154">String</span><span class="sxs-lookup"><span data-stu-id="d4422-154">String</span></span>| <span data-ttu-id="d4422-155">A ID do assunto com a atribuição.</span><span class="sxs-lookup"><span data-stu-id="d4422-155">The ID of the subject with the assignment.</span></span> <span data-ttu-id="d4422-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d4422-156">Read-only.</span></span>|
|<span data-ttu-id="d4422-157">Cronograma</span><span class="sxs-lookup"><span data-stu-id="d4422-157">schedule</span></span>|[<span data-ttu-id="d4422-158">requestSchedule</span><span class="sxs-lookup"><span data-stu-id="d4422-158">requestSchedule</span></span>](requestschedule.md)| <span data-ttu-id="d4422-159">Quando a atribuição de acesso deve estar no lugar.</span><span class="sxs-lookup"><span data-stu-id="d4422-159">When the access assignment is to be in place.</span></span> <span data-ttu-id="d4422-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d4422-160">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4422-161">Relações</span><span class="sxs-lookup"><span data-stu-id="d4422-161">Relationships</span></span>

| <span data-ttu-id="d4422-162">Relação</span><span class="sxs-lookup"><span data-stu-id="d4422-162">Relationship</span></span> | <span data-ttu-id="d4422-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4422-163">Type</span></span>        | <span data-ttu-id="d4422-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4422-164">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d4422-165">accessPackage</span><span class="sxs-lookup"><span data-stu-id="d4422-165">accessPackage</span></span>|[<span data-ttu-id="d4422-166">accessPackage</span><span class="sxs-lookup"><span data-stu-id="d4422-166">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="d4422-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d4422-167">Read-only.</span></span> <span data-ttu-id="d4422-168">Anulável.</span><span class="sxs-lookup"><span data-stu-id="d4422-168">Nullable.</span></span>|
|<span data-ttu-id="d4422-169">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="d4422-169">accessPackageAssignmentPolicy</span></span>|[<span data-ttu-id="d4422-170">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="d4422-170">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md)| <span data-ttu-id="d4422-171">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d4422-171">Read-only.</span></span> <span data-ttu-id="d4422-172">Anulável.</span><span class="sxs-lookup"><span data-stu-id="d4422-172">Nullable.</span></span>|
|<span data-ttu-id="d4422-173">accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="d4422-173">accessPackageAssignmentResourceRoles</span></span>|<span data-ttu-id="d4422-174">[Coleção accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="d4422-174">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span>| <span data-ttu-id="d4422-175">As funções de recurso entregues ao usuário de destino para esta atribuição.</span><span class="sxs-lookup"><span data-stu-id="d4422-175">The resource roles delivered to the target user for this assignment.</span></span> <span data-ttu-id="d4422-176">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d4422-176">Read-only.</span></span> <span data-ttu-id="d4422-177">Anulável.</span><span class="sxs-lookup"><span data-stu-id="d4422-177">Nullable.</span></span>|
|<span data-ttu-id="d4422-178">destino</span><span class="sxs-lookup"><span data-stu-id="d4422-178">target</span></span>|[<span data-ttu-id="d4422-179">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="d4422-179">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="d4422-180">O assunto da atribuição do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="d4422-180">The subject of the access package assignment.</span></span> <span data-ttu-id="d4422-181">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d4422-181">Read-only.</span></span> <span data-ttu-id="d4422-182">Anulável.</span><span class="sxs-lookup"><span data-stu-id="d4422-182">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4422-183">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d4422-183">JSON representation</span></span>

<span data-ttu-id="d4422-184">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d4422-184">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignment",
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


