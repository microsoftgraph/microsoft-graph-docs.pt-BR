---
title: Tipo de recurso accessPackageAssignment
description: Uma atribuição de pacote de acesso é uma atribuição de um pacote de acesso a um assunto específico, por um período de tempo.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: fd352fe67c3afabb1819ffc58d7081dbdae1525c
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52298509"
---
# <a name="accesspackageassignment-resource-type"></a><span data-ttu-id="c33b4-103">Tipo de recurso accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="c33b4-103">accessPackageAssignment resource type</span></span>

<span data-ttu-id="c33b4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c33b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c33b4-105">No [Azure AD Entitlement Management](entitlementmanagement-root.md), uma atribuição de pacote de acesso é uma atribuição de um pacote de acesso a um assunto específico, por um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="c33b4-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), an access package assignment is an assignment of an access package to a particular subject, for a period of time.</span></span>  <span data-ttu-id="c33b4-106">Por exemplo, uma atribuição de pacote de acesso pode dizer que a usuária Alice recebeu acesso por meio do pacote de acesso Vendas do período de janeiro de 2019 a julho de 2019.</span><span class="sxs-lookup"><span data-stu-id="c33b4-106">For example, an access package assignment can state that user Alice has been assigned access via the access package Sales for the period January 2019 through July 2019.</span></span>

## <a name="methods"></a><span data-ttu-id="c33b4-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="c33b4-107">Methods</span></span>

| <span data-ttu-id="c33b4-108">Método</span><span class="sxs-lookup"><span data-stu-id="c33b4-108">Method</span></span>       | <span data-ttu-id="c33b4-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c33b4-109">Return Type</span></span> | <span data-ttu-id="c33b4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c33b4-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c33b4-111">Listar accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="c33b4-111">List accessPackageAssignments</span></span>](../api/accesspackageassignment-list.md) | <span data-ttu-id="c33b4-112">[Coleção accessPackageAssignment](accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c33b4-112">[accessPackageAssignment](accesspackageassignment.md) collection</span></span> | <span data-ttu-id="c33b4-113">Recupere uma lista de **objetos accessPackageAssignment.**</span><span class="sxs-lookup"><span data-stu-id="c33b4-113">Retrieve a list of **accessPackageAssignment** objects.</span></span> |
|[<span data-ttu-id="c33b4-114">filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="c33b4-114">filterByCurrentUser</span></span>](../api/accesspackageassignment-filterbycurrentuser.md)|<span data-ttu-id="c33b4-115">[Coleção accessPackageAssignment](../resources/accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c33b4-115">[accessPackageAssignment](../resources/accesspackageassignment.md) collection</span></span>|<span data-ttu-id="c33b4-116">Recupere a lista de **objetos accessPackageAssignment** filtrados no usuário de entrada.</span><span class="sxs-lookup"><span data-stu-id="c33b4-116">Retrieve the list of **accessPackageAssignment** objects filtered on the signed-in user.</span></span>|

><span data-ttu-id="c33b4-117">**Observação:** Não é possível usar um método para criar ou remover uma atribuição de pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="c33b4-117">**Note:** You can't use a method to create or remove an access package assignment.</span></span> <span data-ttu-id="c33b4-118">Em vez disso, um cliente que deseja solicitar uma atribuição de pacote de acesso para um usuário ou remover uma atribuição de pacote de acesso de um usuário pode criar um [accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).</span><span class="sxs-lookup"><span data-stu-id="c33b4-118">Instead, a client that wants to request an access package assignment for a user, or remove an access package assignment from a user, can [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c33b4-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c33b4-119">Properties</span></span>

| <span data-ttu-id="c33b4-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c33b4-120">Property</span></span>     | <span data-ttu-id="c33b4-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c33b4-121">Type</span></span>        | <span data-ttu-id="c33b4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c33b4-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c33b4-123">accessPackageId</span><span class="sxs-lookup"><span data-stu-id="c33b4-123">accessPackageId</span></span>|<span data-ttu-id="c33b4-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c33b4-124">String</span></span>|<span data-ttu-id="c33b4-125">O identificador do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="c33b4-125">The identifier of the access package.</span></span> <span data-ttu-id="c33b4-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c33b4-126">Read-only.</span></span>|
|<span data-ttu-id="c33b4-127">assignmentPolicyId</span><span class="sxs-lookup"><span data-stu-id="c33b4-127">assignmentPolicyId</span></span>|<span data-ttu-id="c33b4-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c33b4-128">String</span></span>|<span data-ttu-id="c33b4-129">O identificador da política de atribuição do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="c33b4-129">The identifier of the access package assignment policy.</span></span> <span data-ttu-id="c33b4-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c33b4-130">Read-only.</span></span>|
|<span data-ttu-id="c33b4-131">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c33b4-131">assignmentState</span></span>|<span data-ttu-id="c33b4-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c33b4-132">String</span></span>|<span data-ttu-id="c33b4-133">O estado da atribuição do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="c33b4-133">The state of the access package assignment.</span></span> <span data-ttu-id="c33b4-134">Os valores possíveis `Delivering` são `Delivered` , ou `Expired` .</span><span class="sxs-lookup"><span data-stu-id="c33b4-134">Possible values are `Delivering`, `Delivered`, or `Expired`.</span></span> <span data-ttu-id="c33b4-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c33b4-135">Read-only.</span></span>|
|<span data-ttu-id="c33b4-136">assignmentStatus</span><span class="sxs-lookup"><span data-stu-id="c33b4-136">assignmentStatus</span></span>|<span data-ttu-id="c33b4-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c33b4-137">String</span></span>|<span data-ttu-id="c33b4-138">Mais informações sobre o ciclo de vida da atribuição.</span><span class="sxs-lookup"><span data-stu-id="c33b4-138">More information about the assignment lifecycle.</span></span>  <span data-ttu-id="c33b4-139">Os valores possíveis `Delivering` `Delivered` incluem , `NearExpiry1DayNotificationTriggered` , ou `ExpiredNotificationTriggered` .</span><span class="sxs-lookup"><span data-stu-id="c33b4-139">Possible values include `Delivering`, `Delivered`, `NearExpiry1DayNotificationTriggered`, or `ExpiredNotificationTriggered`.</span></span>  <span data-ttu-id="c33b4-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c33b4-140">Read-only.</span></span>|
|<span data-ttu-id="c33b4-141">catalogId</span><span class="sxs-lookup"><span data-stu-id="c33b4-141">catalogId</span></span>|<span data-ttu-id="c33b4-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c33b4-142">String</span></span>|<span data-ttu-id="c33b4-143">O identificador do catálogo que contém o pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="c33b4-143">The identifier of the catalog containing the access package.</span></span> <span data-ttu-id="c33b4-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c33b4-144">Read-only.</span></span>|
|<span data-ttu-id="c33b4-145">expiredDateTime</span><span class="sxs-lookup"><span data-stu-id="c33b4-145">expiredDateTime</span></span>|<span data-ttu-id="c33b4-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c33b4-146">DateTimeOffset</span></span>|<span data-ttu-id="c33b4-147">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="c33b4-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c33b4-148">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="c33b4-148">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="c33b4-149">id</span><span class="sxs-lookup"><span data-stu-id="c33b4-149">id</span></span>|<span data-ttu-id="c33b4-150">String</span><span class="sxs-lookup"><span data-stu-id="c33b4-150">String</span></span>| <span data-ttu-id="c33b4-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c33b4-151">Read-only.</span></span>|
|<span data-ttu-id="c33b4-152">isExtended</span><span class="sxs-lookup"><span data-stu-id="c33b4-152">isExtended</span></span>|<span data-ttu-id="c33b4-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="c33b4-153">Boolean</span></span>|<span data-ttu-id="c33b4-154">Indica se a atribuição do pacote de acesso foi estendida.</span><span class="sxs-lookup"><span data-stu-id="c33b4-154">Indicates whether the access package assignment is extended.</span></span> <span data-ttu-id="c33b4-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c33b4-155">Read-only.</span></span>|
|<span data-ttu-id="c33b4-156">targetId</span><span class="sxs-lookup"><span data-stu-id="c33b4-156">targetId</span></span>|<span data-ttu-id="c33b4-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c33b4-157">String</span></span>| <span data-ttu-id="c33b4-158">A ID do assunto com a atribuição.</span><span class="sxs-lookup"><span data-stu-id="c33b4-158">The ID of the subject with the assignment.</span></span> <span data-ttu-id="c33b4-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c33b4-159">Read-only.</span></span>|
|<span data-ttu-id="c33b4-160">Cronograma</span><span class="sxs-lookup"><span data-stu-id="c33b4-160">schedule</span></span>|[<span data-ttu-id="c33b4-161">requestSchedule</span><span class="sxs-lookup"><span data-stu-id="c33b4-161">requestSchedule</span></span>](requestschedule.md)| <span data-ttu-id="c33b4-162">Quando a atribuição de acesso estiver no local.</span><span class="sxs-lookup"><span data-stu-id="c33b4-162">When the access assignment is to be in place.</span></span> <span data-ttu-id="c33b4-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c33b4-163">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c33b4-164">Relações</span><span class="sxs-lookup"><span data-stu-id="c33b4-164">Relationships</span></span>

| <span data-ttu-id="c33b4-165">Relação</span><span class="sxs-lookup"><span data-stu-id="c33b4-165">Relationship</span></span> | <span data-ttu-id="c33b4-166">Tipo</span><span class="sxs-lookup"><span data-stu-id="c33b4-166">Type</span></span>        | <span data-ttu-id="c33b4-167">Descrição</span><span class="sxs-lookup"><span data-stu-id="c33b4-167">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c33b4-168">accessPackage</span><span class="sxs-lookup"><span data-stu-id="c33b4-168">accessPackage</span></span>|[<span data-ttu-id="c33b4-169">accessPackage</span><span class="sxs-lookup"><span data-stu-id="c33b4-169">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="c33b4-p112">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="c33b4-p112">Read-only. Nullable.</span></span>|
|<span data-ttu-id="c33b4-172">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="c33b4-172">accessPackageAssignmentPolicy</span></span>|[<span data-ttu-id="c33b4-173">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="c33b4-173">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md)| <span data-ttu-id="c33b4-p113">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="c33b4-p113">Read-only. Nullable.</span></span>|
|<span data-ttu-id="c33b4-176">accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="c33b4-176">accessPackageAssignmentResourceRoles</span></span>|<span data-ttu-id="c33b4-177">[Coleção accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="c33b4-177">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span>| <span data-ttu-id="c33b4-178">As funções de recurso entregues ao usuário de destino para essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="c33b4-178">The resource roles delivered to the target user for this assignment.</span></span> <span data-ttu-id="c33b4-179">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c33b4-179">Read-only.</span></span> <span data-ttu-id="c33b4-180">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c33b4-180">Nullable.</span></span>|
|<span data-ttu-id="c33b4-181">destino</span><span class="sxs-lookup"><span data-stu-id="c33b4-181">target</span></span>|[<span data-ttu-id="c33b4-182">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="c33b4-182">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="c33b4-183">O assunto da atribuição do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="c33b4-183">The subject of the access package assignment.</span></span> <span data-ttu-id="c33b4-184">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c33b4-184">Read-only.</span></span> <span data-ttu-id="c33b4-185">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c33b4-185">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c33b4-186">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c33b4-186">JSON representation</span></span>

<span data-ttu-id="c33b4-187">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c33b4-187">The following is a JSON representation of the resource.</span></span>

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


