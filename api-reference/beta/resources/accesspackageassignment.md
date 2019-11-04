---
title: tipo de recurso accessPackageAssignment
description: Uma atribuição de pacote do Access é uma atribuição de um pacote do Access a um assunto específico, por um período de tempo.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 234aad48e11a2b6c5c2a47c494216fa15fbc139b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939212"
---
# <a name="accesspackageassignment-resource-type"></a><span data-ttu-id="90072-103">tipo de recurso accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="90072-103">accessPackageAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90072-104">No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma atribuição de pacote de acesso é uma atribuição de um pacote do Access a um assunto específico, por um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="90072-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment is an assignment of an access package to a particular subject, for a period of time.</span></span>  <span data-ttu-id="90072-105">Por exemplo, uma atribuição de pacote de acesso pode indicar que o usuário ' Alice ' tem o acesso atribuído por meio do pacote de acesso ' Sales ' para o período de janeiro de 2019 a julho de 2019.</span><span class="sxs-lookup"><span data-stu-id="90072-105">For example, an access package assignment could state that user 'Alice' has the been assigned access via the access package 'Sales' for the period January 2019 through July 2019.</span></span>

## <a name="methods"></a><span data-ttu-id="90072-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="90072-106">Methods</span></span>

| <span data-ttu-id="90072-107">Método</span><span class="sxs-lookup"><span data-stu-id="90072-107">Method</span></span>       | <span data-ttu-id="90072-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="90072-108">Return Type</span></span> | <span data-ttu-id="90072-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="90072-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="90072-110">Listar accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="90072-110">List accessPackageAssignments</span></span>](../api/accesspackageassignment-list.md) | <span data-ttu-id="90072-111">coleção [accessPackageAssignment](accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="90072-111">[accessPackageAssignment](accesspackageassignment.md) collection</span></span> | <span data-ttu-id="90072-112">Recupere uma lista de objetos **accesspackageassignment** .</span><span class="sxs-lookup"><span data-stu-id="90072-112">Retrieve a list of **accesspackageassignment** objects.</span></span> |

><span data-ttu-id="90072-113">**Observação:** Você não pode usar um método para criar uma atribuição de pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="90072-113">**Note:** You can't use a method to create an access package assignment.</span></span> <span data-ttu-id="90072-114">Em vez disso, um cliente que deseja solicitar uma atribuição de pacote de acesso para um usuário pode [criar um accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).</span><span class="sxs-lookup"><span data-stu-id="90072-114">Instead, a client that wants to request an access package assignment for a user can [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).</span></span>

## <a name="properties"></a><span data-ttu-id="90072-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="90072-115">Properties</span></span>

| <span data-ttu-id="90072-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90072-116">Property</span></span>     | <span data-ttu-id="90072-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="90072-117">Type</span></span>        | <span data-ttu-id="90072-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="90072-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="90072-119">accessPackageId</span><span class="sxs-lookup"><span data-stu-id="90072-119">accessPackageId</span></span>|<span data-ttu-id="90072-120">String</span><span class="sxs-lookup"><span data-stu-id="90072-120">String</span></span>|<span data-ttu-id="90072-121">O identificador do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="90072-121">The identifier of the access package.</span></span> <span data-ttu-id="90072-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90072-122">Read-only.</span></span>|
|<span data-ttu-id="90072-123">assignmentPolicyId</span><span class="sxs-lookup"><span data-stu-id="90072-123">assignmentPolicyId</span></span>|<span data-ttu-id="90072-124">String</span><span class="sxs-lookup"><span data-stu-id="90072-124">String</span></span>|<span data-ttu-id="90072-125">O identificador da política de atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="90072-125">The identifier of the access package assignment policy.</span></span> <span data-ttu-id="90072-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90072-126">Read-only.</span></span>|
|<span data-ttu-id="90072-127">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="90072-127">assignmentState</span></span>|<span data-ttu-id="90072-128">String</span><span class="sxs-lookup"><span data-stu-id="90072-128">String</span></span>|<span data-ttu-id="90072-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90072-129">Read-only.</span></span>|
|<span data-ttu-id="90072-130">assignmentStatus</span><span class="sxs-lookup"><span data-stu-id="90072-130">assignmentStatus</span></span>|<span data-ttu-id="90072-131">String</span><span class="sxs-lookup"><span data-stu-id="90072-131">String</span></span>|<span data-ttu-id="90072-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90072-132">Read-only.</span></span>|
|<span data-ttu-id="90072-133">catalogID</span><span class="sxs-lookup"><span data-stu-id="90072-133">catalogId</span></span>|<span data-ttu-id="90072-134">String</span><span class="sxs-lookup"><span data-stu-id="90072-134">String</span></span>|<span data-ttu-id="90072-135">O identificador do catálogo que contém o pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="90072-135">The identifier of the catalog containing the access package.</span></span> <span data-ttu-id="90072-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90072-136">Read-only.</span></span>|
|<span data-ttu-id="90072-137">expiredDateTime</span><span class="sxs-lookup"><span data-stu-id="90072-137">expiredDateTime</span></span>|<span data-ttu-id="90072-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90072-138">DateTimeOffset</span></span>|<span data-ttu-id="90072-p106">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="90072-p106">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="90072-141">id</span><span class="sxs-lookup"><span data-stu-id="90072-141">id</span></span>|<span data-ttu-id="90072-142">String</span><span class="sxs-lookup"><span data-stu-id="90072-142">String</span></span>| <span data-ttu-id="90072-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90072-143">Read-only.</span></span>|
|<span data-ttu-id="90072-144">Extended</span><span class="sxs-lookup"><span data-stu-id="90072-144">isExtended</span></span>|<span data-ttu-id="90072-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="90072-145">Boolean</span></span>|<span data-ttu-id="90072-146">Indica se a atribuição de pacote de acesso é estendida.</span><span class="sxs-lookup"><span data-stu-id="90072-146">Indicates whether the access package assignment is extended.</span></span> <span data-ttu-id="90072-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90072-147">Read-only.</span></span>|
|<span data-ttu-id="90072-148">targetId</span><span class="sxs-lookup"><span data-stu-id="90072-148">targetId</span></span>|<span data-ttu-id="90072-149">String</span><span class="sxs-lookup"><span data-stu-id="90072-149">String</span></span>| <span data-ttu-id="90072-150">A ID do assunto com a atribuição.</span><span class="sxs-lookup"><span data-stu-id="90072-150">The ID of the subject with the assignment.</span></span> <span data-ttu-id="90072-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90072-151">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90072-152">Relações</span><span class="sxs-lookup"><span data-stu-id="90072-152">Relationships</span></span>

| <span data-ttu-id="90072-153">Relação</span><span class="sxs-lookup"><span data-stu-id="90072-153">Relationship</span></span> | <span data-ttu-id="90072-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="90072-154">Type</span></span>        | <span data-ttu-id="90072-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="90072-155">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="90072-156">accessPackage</span><span class="sxs-lookup"><span data-stu-id="90072-156">accessPackage</span></span>|[<span data-ttu-id="90072-157">accessPackage</span><span class="sxs-lookup"><span data-stu-id="90072-157">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="90072-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90072-158">Read-only.</span></span> <span data-ttu-id="90072-159">Anulável.</span><span class="sxs-lookup"><span data-stu-id="90072-159">Nullable.</span></span>|
|<span data-ttu-id="90072-160">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="90072-160">accessPackageAssignmentPolicy</span></span>|[<span data-ttu-id="90072-161">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="90072-161">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md)| <span data-ttu-id="90072-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90072-162">Read-only.</span></span> <span data-ttu-id="90072-163">Anulável.</span><span class="sxs-lookup"><span data-stu-id="90072-163">Nullable.</span></span>|
|<span data-ttu-id="90072-164">accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="90072-164">accessPackageAssignmentResourceRoles</span></span>|<span data-ttu-id="90072-165">coleção [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="90072-165">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span>| <span data-ttu-id="90072-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90072-166">Read-only.</span></span> <span data-ttu-id="90072-167">Anulável.</span><span class="sxs-lookup"><span data-stu-id="90072-167">Nullable.</span></span>|
|<span data-ttu-id="90072-168">destino</span><span class="sxs-lookup"><span data-stu-id="90072-168">target</span></span>|[<span data-ttu-id="90072-169">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="90072-169">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="90072-170">O assunto da atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="90072-170">The subject of the access package assignment.</span></span> <span data-ttu-id="90072-171">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90072-171">Read-only.</span></span> <span data-ttu-id="90072-172">Anulável.</span><span class="sxs-lookup"><span data-stu-id="90072-172">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="90072-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="90072-173">JSON representation</span></span>

<span data-ttu-id="90072-174">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="90072-174">The following is a JSON representation of the resource.</span></span>

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
