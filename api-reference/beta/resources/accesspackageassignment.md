---
title: tipo de recurso accessPackageAssignment
description: Uma atribuição de pacote do Access é uma atribuição de um pacote do Access a um assunto específico, por um período de tempo.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f7a2fe772dc7b3be328fad452a5b193ccf7a7ed0
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319453"
---
# <a name="accesspackageassignment-resource-type"></a><span data-ttu-id="46e57-103">tipo de recurso accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="46e57-103">accessPackageAssignment resource type</span></span>

<span data-ttu-id="46e57-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46e57-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46e57-105">No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma atribuição de pacote de acesso é uma atribuição de um pacote do Access a um assunto específico, por um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="46e57-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment is an assignment of an access package to a particular subject, for a period of time.</span></span>  <span data-ttu-id="46e57-106">Por exemplo, uma atribuição de pacote de acesso pode indicar que o usuário ' Alice ' tem o acesso atribuído por meio do pacote de acesso ' Sales ' para o período de janeiro de 2019 a julho de 2019.</span><span class="sxs-lookup"><span data-stu-id="46e57-106">For example, an access package assignment could state that user 'Alice' has the been assigned access via the access package 'Sales' for the period January 2019 through July 2019.</span></span>

## <a name="methods"></a><span data-ttu-id="46e57-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="46e57-107">Methods</span></span>

| <span data-ttu-id="46e57-108">Método</span><span class="sxs-lookup"><span data-stu-id="46e57-108">Method</span></span>       | <span data-ttu-id="46e57-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="46e57-109">Return Type</span></span> | <span data-ttu-id="46e57-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="46e57-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="46e57-111">Listar accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="46e57-111">List accessPackageAssignments</span></span>](../api/accesspackageassignment-list.md) | <span data-ttu-id="46e57-112">coleção [accessPackageAssignment](accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="46e57-112">[accessPackageAssignment](accesspackageassignment.md) collection</span></span> | <span data-ttu-id="46e57-113">Recupere uma lista de objetos **accesspackageassignment** .</span><span class="sxs-lookup"><span data-stu-id="46e57-113">Retrieve a list of **accesspackageassignment** objects.</span></span> |

><span data-ttu-id="46e57-114">**Observação:** Você não pode usar um método para criar ou remover uma atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="46e57-114">**Note:** You can't use a method to create or remove an access package assignment.</span></span> <span data-ttu-id="46e57-115">Em vez disso, um cliente que deseja solicitar uma atribuição de pacote do Access para um usuário ou remover uma atribuição de pacote de acesso de um usuário, pode [criar um accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).</span><span class="sxs-lookup"><span data-stu-id="46e57-115">Instead, a client that wants to request an access package assignment for a user, or remove an access package assignment from a user, can [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).</span></span>

## <a name="properties"></a><span data-ttu-id="46e57-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="46e57-116">Properties</span></span>

| <span data-ttu-id="46e57-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46e57-117">Property</span></span>     | <span data-ttu-id="46e57-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="46e57-118">Type</span></span>        | <span data-ttu-id="46e57-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="46e57-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="46e57-120">accessPackageId</span><span class="sxs-lookup"><span data-stu-id="46e57-120">accessPackageId</span></span>|<span data-ttu-id="46e57-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46e57-121">String</span></span>|<span data-ttu-id="46e57-122">O identificador do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="46e57-122">The identifier of the access package.</span></span> <span data-ttu-id="46e57-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46e57-123">Read-only.</span></span>|
|<span data-ttu-id="46e57-124">assignmentPolicyId</span><span class="sxs-lookup"><span data-stu-id="46e57-124">assignmentPolicyId</span></span>|<span data-ttu-id="46e57-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46e57-125">String</span></span>|<span data-ttu-id="46e57-126">O identificador da política de atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="46e57-126">The identifier of the access package assignment policy.</span></span> <span data-ttu-id="46e57-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46e57-127">Read-only.</span></span>|
|<span data-ttu-id="46e57-128">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="46e57-128">assignmentState</span></span>|<span data-ttu-id="46e57-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46e57-129">String</span></span>|<span data-ttu-id="46e57-130">O estado do pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="46e57-130">The state of the access package.</span></span> <span data-ttu-id="46e57-131">Os valores possíveis são `Delivered` ou `Expired` .</span><span class="sxs-lookup"><span data-stu-id="46e57-131">Possible values are `Delivered` or `Expired`.</span></span> <span data-ttu-id="46e57-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46e57-132">Read-only.</span></span>|
|<span data-ttu-id="46e57-133">assignmentStatus</span><span class="sxs-lookup"><span data-stu-id="46e57-133">assignmentStatus</span></span>|<span data-ttu-id="46e57-134">String</span><span class="sxs-lookup"><span data-stu-id="46e57-134">String</span></span>|<span data-ttu-id="46e57-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46e57-135">Read-only.</span></span>|
|<span data-ttu-id="46e57-136">catalogID</span><span class="sxs-lookup"><span data-stu-id="46e57-136">catalogId</span></span>|<span data-ttu-id="46e57-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46e57-137">String</span></span>|<span data-ttu-id="46e57-138">O identificador do catálogo que contém o pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="46e57-138">The identifier of the catalog containing the access package.</span></span> <span data-ttu-id="46e57-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46e57-139">Read-only.</span></span>|
|<span data-ttu-id="46e57-140">expiredDateTime</span><span class="sxs-lookup"><span data-stu-id="46e57-140">expiredDateTime</span></span>|<span data-ttu-id="46e57-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46e57-141">DateTimeOffset</span></span>|<span data-ttu-id="46e57-p107">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="46e57-p107">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="46e57-144">id</span><span class="sxs-lookup"><span data-stu-id="46e57-144">id</span></span>|<span data-ttu-id="46e57-145">String</span><span class="sxs-lookup"><span data-stu-id="46e57-145">String</span></span>| <span data-ttu-id="46e57-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46e57-146">Read-only.</span></span>|
|<span data-ttu-id="46e57-147">Extended</span><span class="sxs-lookup"><span data-stu-id="46e57-147">isExtended</span></span>|<span data-ttu-id="46e57-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="46e57-148">Boolean</span></span>|<span data-ttu-id="46e57-149">Indica se a atribuição de pacote de acesso é estendida.</span><span class="sxs-lookup"><span data-stu-id="46e57-149">Indicates whether the access package assignment is extended.</span></span> <span data-ttu-id="46e57-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46e57-150">Read-only.</span></span>|
|<span data-ttu-id="46e57-151">targetId</span><span class="sxs-lookup"><span data-stu-id="46e57-151">targetId</span></span>|<span data-ttu-id="46e57-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46e57-152">String</span></span>| <span data-ttu-id="46e57-153">A ID do assunto com a atribuição.</span><span class="sxs-lookup"><span data-stu-id="46e57-153">The ID of the subject with the assignment.</span></span> <span data-ttu-id="46e57-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46e57-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="46e57-155">Relações</span><span class="sxs-lookup"><span data-stu-id="46e57-155">Relationships</span></span>

| <span data-ttu-id="46e57-156">Relação</span><span class="sxs-lookup"><span data-stu-id="46e57-156">Relationship</span></span> | <span data-ttu-id="46e57-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="46e57-157">Type</span></span>        | <span data-ttu-id="46e57-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="46e57-158">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="46e57-159">accessPackage</span><span class="sxs-lookup"><span data-stu-id="46e57-159">accessPackage</span></span>|[<span data-ttu-id="46e57-160">accessPackage</span><span class="sxs-lookup"><span data-stu-id="46e57-160">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="46e57-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46e57-161">Read-only.</span></span> <span data-ttu-id="46e57-162">Anulável.</span><span class="sxs-lookup"><span data-stu-id="46e57-162">Nullable.</span></span>|
|<span data-ttu-id="46e57-163">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="46e57-163">accessPackageAssignmentPolicy</span></span>|[<span data-ttu-id="46e57-164">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="46e57-164">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md)| <span data-ttu-id="46e57-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46e57-165">Read-only.</span></span> <span data-ttu-id="46e57-166">Anulável.</span><span class="sxs-lookup"><span data-stu-id="46e57-166">Nullable.</span></span>|
|<span data-ttu-id="46e57-167">accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="46e57-167">accessPackageAssignmentResourceRoles</span></span>|<span data-ttu-id="46e57-168">coleção [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="46e57-168">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span>| <span data-ttu-id="46e57-169">As funções de recurso entregues ao usuário de destino para esta atribuição.</span><span class="sxs-lookup"><span data-stu-id="46e57-169">The resource roles delivered to the target user for this assignment.</span></span> <span data-ttu-id="46e57-170">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46e57-170">Read-only.</span></span> <span data-ttu-id="46e57-171">Anulável.</span><span class="sxs-lookup"><span data-stu-id="46e57-171">Nullable.</span></span>|
|<span data-ttu-id="46e57-172">destino</span><span class="sxs-lookup"><span data-stu-id="46e57-172">target</span></span>|[<span data-ttu-id="46e57-173">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="46e57-173">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="46e57-174">O assunto da atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="46e57-174">The subject of the access package assignment.</span></span> <span data-ttu-id="46e57-175">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46e57-175">Read-only.</span></span> <span data-ttu-id="46e57-176">Anulável.</span><span class="sxs-lookup"><span data-stu-id="46e57-176">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="46e57-177">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="46e57-177">JSON representation</span></span>

<span data-ttu-id="46e57-178">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="46e57-178">The following is a JSON representation of the resource.</span></span>

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
