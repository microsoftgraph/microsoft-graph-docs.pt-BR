---
title: tipo de recurso accessPackageAssignment
description: Uma atribuição de pacote do Access é uma atribuição de um pacote do Access a um assunto específico, por um período de tempo.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7147378e308faac7ca1fea931a465e1ea54f22ef
ms.sourcegitcommit: f51ba08d604d93f5f6af9ee8979cbf76baa285ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/19/2020
ms.locfileid: "42108445"
---
# <a name="accesspackageassignment-resource-type"></a><span data-ttu-id="ad18a-103">tipo de recurso accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="ad18a-103">accessPackageAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad18a-104">No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma atribuição de pacote de acesso é uma atribuição de um pacote do Access a um assunto específico, por um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="ad18a-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment is an assignment of an access package to a particular subject, for a period of time.</span></span>  <span data-ttu-id="ad18a-105">Por exemplo, uma atribuição de pacote de acesso pode indicar que o usuário ' Alice ' tem o acesso atribuído por meio do pacote de acesso ' Sales ' para o período de janeiro de 2019 a julho de 2019.</span><span class="sxs-lookup"><span data-stu-id="ad18a-105">For example, an access package assignment could state that user 'Alice' has the been assigned access via the access package 'Sales' for the period January 2019 through July 2019.</span></span>

## <a name="methods"></a><span data-ttu-id="ad18a-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="ad18a-106">Methods</span></span>

| <span data-ttu-id="ad18a-107">Método</span><span class="sxs-lookup"><span data-stu-id="ad18a-107">Method</span></span>       | <span data-ttu-id="ad18a-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ad18a-108">Return Type</span></span> | <span data-ttu-id="ad18a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad18a-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ad18a-110">Listar accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="ad18a-110">List accessPackageAssignments</span></span>](../api/accesspackageassignment-list.md) | <span data-ttu-id="ad18a-111">coleção [accessPackageAssignment](accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ad18a-111">[accessPackageAssignment](accesspackageassignment.md) collection</span></span> | <span data-ttu-id="ad18a-112">Recupere uma lista de objetos **accesspackageassignment** .</span><span class="sxs-lookup"><span data-stu-id="ad18a-112">Retrieve a list of **accesspackageassignment** objects.</span></span> |

><span data-ttu-id="ad18a-113">**Observação:** Você não pode usar um método para criar ou remover uma atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="ad18a-113">**Note:** You can't use a method to create or remove an access package assignment.</span></span> <span data-ttu-id="ad18a-114">Em vez disso, um cliente que deseja solicitar uma atribuição de pacote do Access para um usuário ou remover uma atribuição de pacote de acesso de um usuário, pode [criar um accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).</span><span class="sxs-lookup"><span data-stu-id="ad18a-114">Instead, a client that wants to request an access package assignment for a user, or remove an access package assignment from a user, can [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ad18a-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ad18a-115">Properties</span></span>

| <span data-ttu-id="ad18a-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ad18a-116">Property</span></span>     | <span data-ttu-id="ad18a-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad18a-117">Type</span></span>        | <span data-ttu-id="ad18a-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad18a-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ad18a-119">accessPackageId</span><span class="sxs-lookup"><span data-stu-id="ad18a-119">accessPackageId</span></span>|<span data-ttu-id="ad18a-120">String</span><span class="sxs-lookup"><span data-stu-id="ad18a-120">String</span></span>|<span data-ttu-id="ad18a-121">O identificador do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="ad18a-121">The identifier of the access package.</span></span> <span data-ttu-id="ad18a-122">Apenas leitura.</span><span class="sxs-lookup"><span data-stu-id="ad18a-122">Read-only.</span></span>|
|<span data-ttu-id="ad18a-123">assignmentPolicyId</span><span class="sxs-lookup"><span data-stu-id="ad18a-123">assignmentPolicyId</span></span>|<span data-ttu-id="ad18a-124">String</span><span class="sxs-lookup"><span data-stu-id="ad18a-124">String</span></span>|<span data-ttu-id="ad18a-125">O identificador da política de atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="ad18a-125">The identifier of the access package assignment policy.</span></span> <span data-ttu-id="ad18a-126">Apenas leitura.</span><span class="sxs-lookup"><span data-stu-id="ad18a-126">Read-only.</span></span>|
|<span data-ttu-id="ad18a-127">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="ad18a-127">assignmentState</span></span>|<span data-ttu-id="ad18a-128">String</span><span class="sxs-lookup"><span data-stu-id="ad18a-128">String</span></span>|<span data-ttu-id="ad18a-129">O estado do pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="ad18a-129">The state of the access package.</span></span> <span data-ttu-id="ad18a-130">Os valores possíveis `Delivered` são `Expired`ou.</span><span class="sxs-lookup"><span data-stu-id="ad18a-130">Possible values are `Delivered` or `Expired`.</span></span> <span data-ttu-id="ad18a-131">Apenas leitura.</span><span class="sxs-lookup"><span data-stu-id="ad18a-131">Read-only.</span></span>|
|<span data-ttu-id="ad18a-132">assignmentStatus</span><span class="sxs-lookup"><span data-stu-id="ad18a-132">assignmentStatus</span></span>|<span data-ttu-id="ad18a-133">String</span><span class="sxs-lookup"><span data-stu-id="ad18a-133">String</span></span>|<span data-ttu-id="ad18a-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ad18a-134">Read-only.</span></span>|
|<span data-ttu-id="ad18a-135">catalogID</span><span class="sxs-lookup"><span data-stu-id="ad18a-135">catalogId</span></span>|<span data-ttu-id="ad18a-136">String</span><span class="sxs-lookup"><span data-stu-id="ad18a-136">String</span></span>|<span data-ttu-id="ad18a-137">O identificador do catálogo que contém o pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="ad18a-137">The identifier of the catalog containing the access package.</span></span> <span data-ttu-id="ad18a-138">Apenas leitura.</span><span class="sxs-lookup"><span data-stu-id="ad18a-138">Read-only.</span></span>|
|<span data-ttu-id="ad18a-139">expiredDateTime</span><span class="sxs-lookup"><span data-stu-id="ad18a-139">expiredDateTime</span></span>|<span data-ttu-id="ad18a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad18a-140">DateTimeOffset</span></span>|<span data-ttu-id="ad18a-p107">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ad18a-p107">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ad18a-143">id</span><span class="sxs-lookup"><span data-stu-id="ad18a-143">id</span></span>|<span data-ttu-id="ad18a-144">String</span><span class="sxs-lookup"><span data-stu-id="ad18a-144">String</span></span>| <span data-ttu-id="ad18a-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ad18a-145">Read-only.</span></span>|
|<span data-ttu-id="ad18a-146">Extended</span><span class="sxs-lookup"><span data-stu-id="ad18a-146">isExtended</span></span>|<span data-ttu-id="ad18a-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="ad18a-147">Boolean</span></span>|<span data-ttu-id="ad18a-148">Indica se a atribuição de pacote de acesso é estendida.</span><span class="sxs-lookup"><span data-stu-id="ad18a-148">Indicates whether the access package assignment is extended.</span></span> <span data-ttu-id="ad18a-149">Apenas leitura.</span><span class="sxs-lookup"><span data-stu-id="ad18a-149">Read-only.</span></span>|
|<span data-ttu-id="ad18a-150">targetId</span><span class="sxs-lookup"><span data-stu-id="ad18a-150">targetId</span></span>|<span data-ttu-id="ad18a-151">String</span><span class="sxs-lookup"><span data-stu-id="ad18a-151">String</span></span>| <span data-ttu-id="ad18a-152">A ID do assunto com a atribuição.</span><span class="sxs-lookup"><span data-stu-id="ad18a-152">The ID of the subject with the assignment.</span></span> <span data-ttu-id="ad18a-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ad18a-153">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad18a-154">Relações</span><span class="sxs-lookup"><span data-stu-id="ad18a-154">Relationships</span></span>

| <span data-ttu-id="ad18a-155">Relação</span><span class="sxs-lookup"><span data-stu-id="ad18a-155">Relationship</span></span> | <span data-ttu-id="ad18a-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad18a-156">Type</span></span>        | <span data-ttu-id="ad18a-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad18a-157">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ad18a-158">accessPackage</span><span class="sxs-lookup"><span data-stu-id="ad18a-158">accessPackage</span></span>|[<span data-ttu-id="ad18a-159">accessPackage</span><span class="sxs-lookup"><span data-stu-id="ad18a-159">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="ad18a-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ad18a-160">Read-only.</span></span> <span data-ttu-id="ad18a-161">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ad18a-161">Nullable.</span></span>|
|<span data-ttu-id="ad18a-162">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="ad18a-162">accessPackageAssignmentPolicy</span></span>|[<span data-ttu-id="ad18a-163">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="ad18a-163">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md)| <span data-ttu-id="ad18a-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ad18a-164">Read-only.</span></span> <span data-ttu-id="ad18a-165">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ad18a-165">Nullable.</span></span>|
|<span data-ttu-id="ad18a-166">accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="ad18a-166">accessPackageAssignmentResourceRoles</span></span>|<span data-ttu-id="ad18a-167">coleção [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="ad18a-167">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span>| <span data-ttu-id="ad18a-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ad18a-168">Read-only.</span></span> <span data-ttu-id="ad18a-169">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ad18a-169">Nullable.</span></span>|
|<span data-ttu-id="ad18a-170">destino</span><span class="sxs-lookup"><span data-stu-id="ad18a-170">target</span></span>|[<span data-ttu-id="ad18a-171">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="ad18a-171">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="ad18a-172">O assunto da atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="ad18a-172">The subject of the access package assignment.</span></span> <span data-ttu-id="ad18a-173">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ad18a-173">Read-only.</span></span> <span data-ttu-id="ad18a-174">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ad18a-174">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ad18a-175">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ad18a-175">JSON representation</span></span>

<span data-ttu-id="ad18a-176">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ad18a-176">The following is a JSON representation of the resource.</span></span>

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
            "id": "9bdae7b4-6ece-487b-9eb8-9679dbd67aa2",
            "catalogId": "cc30dc98-6d3c-4fa0-bed8-fd76d0efd993",
            "accessPackageId": "e3f47362-993f-4fcb-8a38-532ffca16150",
            "assignmentPolicyId": "63ebd106-8116-40e7-a0ab-01ae475d11bb",
            "targetId": "ab4291f6-66b7-42bf-b597-a05b29414f5c",
            "assignmentStatus": "ExpiredNotificationTriggered",
            "assignmentState": "Expired",
            "isExtended": false,
            "expiredDateTime": "2019-04-25T23:45:40.42Z"
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
