---
title: tipo de recurso accessPackageAssignmentRequest
description: Uma solicitação de atribuição de pacote do Access é criada por um usuário que deseja obter uma atribuição de pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0fd9f5ea9cd15abac7eea693b2af5c595b145ac7
ms.sourcegitcommit: f51ba08d604d93f5f6af9ee8979cbf76baa285ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/19/2020
ms.locfileid: "42108438"
---
# <a name="accesspackageassignmentrequest-resource-type"></a><span data-ttu-id="e208c-103">tipo de recurso accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="e208c-103">accessPackageAssignmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e208c-104">No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma solicitação de atribuição de pacote de acesso é criada por um usuário que deseja obter uma atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="e208c-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="e208c-105">Se a solicitação for bem-sucedida, com todas as aprovações necessárias, o usuário receberá uma atribuição de pacote de acesso e será o assunto dessa atribuição de pacote de acesso resultante.</span><span class="sxs-lookup"><span data-stu-id="e208c-105">If the request is successful, with any necessary approvals, the user receives an access package assignment, and is the subject of that resulting access package assignment.</span></span>


## <a name="methods"></a><span data-ttu-id="e208c-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="e208c-106">Methods</span></span>

| <span data-ttu-id="e208c-107">Método</span><span class="sxs-lookup"><span data-stu-id="e208c-107">Method</span></span>       | <span data-ttu-id="e208c-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e208c-108">Return Type</span></span> | <span data-ttu-id="e208c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e208c-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e208c-110">Listar accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="e208c-110">List accessPackageAssignmentRequests</span></span>](../api/accesspackageassignmentrequest-list.md) | <span data-ttu-id="e208c-111">coleção [accessPackageAssignmentRequest](accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="e208c-111">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) collection</span></span> | <span data-ttu-id="e208c-112">Recupere uma lista de objetos accesspackageassignmentrequest.</span><span class="sxs-lookup"><span data-stu-id="e208c-112">Retrieve a list of accesspackageassignmentrequest objects.</span></span> |
| [<span data-ttu-id="e208c-113">Criar accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="e208c-113">Create accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-post.md) | [<span data-ttu-id="e208c-114">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="e208c-114">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="e208c-115">Criar um novo accessPackageAssignmentRequest.</span><span class="sxs-lookup"><span data-stu-id="e208c-115">Create a new accessPackageAssignmentRequest.</span></span> |
| [<span data-ttu-id="e208c-116">Obter accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="e208c-116">Get accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-get.md) | [<span data-ttu-id="e208c-117">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="e208c-117">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="e208c-118">Ler propriedades e relações de um objeto accessPackageAssignmentRequest.</span><span class="sxs-lookup"><span data-stu-id="e208c-118">Read properties and relationships of an accessPackageAssignmentRequest object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e208c-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e208c-119">Properties</span></span>

| <span data-ttu-id="e208c-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e208c-120">Property</span></span>     | <span data-ttu-id="e208c-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e208c-121">Type</span></span>        | <span data-ttu-id="e208c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e208c-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e208c-123">completedDate</span><span class="sxs-lookup"><span data-stu-id="e208c-123">completedDate</span></span>|<span data-ttu-id="e208c-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e208c-124">DateTimeOffset</span></span>|<span data-ttu-id="e208c-125">A data do final do processamento, bem como êxito ou falha, de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="e208c-125">The date of the end of processing, either successful or failure, of a request.</span></span> <span data-ttu-id="e208c-126">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="e208c-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e208c-127">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e208c-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="e208c-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e208c-128">Read-only.</span></span>|
|<span data-ttu-id="e208c-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e208c-129">createdDateTime</span></span>|<span data-ttu-id="e208c-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e208c-130">DateTimeOffset</span></span>|<span data-ttu-id="e208c-131">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="e208c-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e208c-132">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e208c-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="e208c-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e208c-133">Read-only.</span></span>|
|<span data-ttu-id="e208c-134">id</span><span class="sxs-lookup"><span data-stu-id="e208c-134">id</span></span>|<span data-ttu-id="e208c-135">String</span><span class="sxs-lookup"><span data-stu-id="e208c-135">String</span></span>| <span data-ttu-id="e208c-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e208c-136">Read-only.</span></span>|
|<span data-ttu-id="e208c-137">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="e208c-137">isValidationOnly</span></span>|<span data-ttu-id="e208c-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="e208c-138">Boolean</span></span>|<span data-ttu-id="e208c-139">True se a solicitação não deve ser processada para a atribuição.</span><span class="sxs-lookup"><span data-stu-id="e208c-139">True if the request is not to be processed for assignment.</span></span>|
|<span data-ttu-id="e208c-140">elabora</span><span class="sxs-lookup"><span data-stu-id="e208c-140">justification</span></span>|<span data-ttu-id="e208c-141">String</span><span class="sxs-lookup"><span data-stu-id="e208c-141">String</span></span>|<span data-ttu-id="e208c-142">A justificativa fornecida pelo solicitante.</span><span class="sxs-lookup"><span data-stu-id="e208c-142">The requestor's supplied justification.</span></span>|
|<span data-ttu-id="e208c-143">RequestState</span><span class="sxs-lookup"><span data-stu-id="e208c-143">requestState</span></span>|<span data-ttu-id="e208c-144">String</span><span class="sxs-lookup"><span data-stu-id="e208c-144">String</span></span>|<span data-ttu-id="e208c-145">Um de `Denied`, `Delivered` `PartiallyDelivered` ou `Submitted`.</span><span class="sxs-lookup"><span data-stu-id="e208c-145">One of `Denied`, `Delivered`, `PartiallyDelivered` or `Submitted`.</span></span> <span data-ttu-id="e208c-146">Apenas leitura.</span><span class="sxs-lookup"><span data-stu-id="e208c-146">Read-only.</span></span>|
|<span data-ttu-id="e208c-147">requestStatus</span><span class="sxs-lookup"><span data-stu-id="e208c-147">requestStatus</span></span>|<span data-ttu-id="e208c-148">String</span><span class="sxs-lookup"><span data-stu-id="e208c-148">String</span></span>|<span data-ttu-id="e208c-149">Mais informações sobre o status do processamento da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e208c-149">More information on the request processing status.</span></span> <span data-ttu-id="e208c-150">Apenas leitura.</span><span class="sxs-lookup"><span data-stu-id="e208c-150">Read-only.</span></span>|
|<span data-ttu-id="e208c-151">RequestType</span><span class="sxs-lookup"><span data-stu-id="e208c-151">requestType</span></span>|<span data-ttu-id="e208c-152">String</span><span class="sxs-lookup"><span data-stu-id="e208c-152">String</span></span>|<span data-ttu-id="e208c-153">Um de `UserAdd`, `UserRemove` `AdminAdd` ou `AdminRemove`.</span><span class="sxs-lookup"><span data-stu-id="e208c-153">One of `UserAdd`, `UserRemove`, `AdminAdd` or `AdminRemove`.</span></span> <span data-ttu-id="e208c-154">Apenas leitura.</span><span class="sxs-lookup"><span data-stu-id="e208c-154">Read-only.</span></span>|
|<span data-ttu-id="e208c-155">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="e208c-155">accessPackageAssignment</span></span>|[<span data-ttu-id="e208c-156">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="e208c-156">accessPackageAssignment</span></span>](accesspackageassignment.md)| <span data-ttu-id="e208c-157">Uma atribuição de pacote de acesso solicitada foi criada.</span><span class="sxs-lookup"><span data-stu-id="e208c-157">An access package assignment requested to be created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e208c-158">Relações</span><span class="sxs-lookup"><span data-stu-id="e208c-158">Relationships</span></span>

| <span data-ttu-id="e208c-159">Relação</span><span class="sxs-lookup"><span data-stu-id="e208c-159">Relationship</span></span> | <span data-ttu-id="e208c-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="e208c-160">Type</span></span>        | <span data-ttu-id="e208c-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="e208c-161">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e208c-162">solicitante</span><span class="sxs-lookup"><span data-stu-id="e208c-162">requestor</span></span>|[<span data-ttu-id="e208c-163">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="e208c-163">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="e208c-164">O assunto que solicitou ou, se uma atribuição direta, foi atribuído.</span><span class="sxs-lookup"><span data-stu-id="e208c-164">The subject who requested or, if a direct assignment, was assigned.</span></span> <span data-ttu-id="e208c-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e208c-165">Read-only.</span></span> <span data-ttu-id="e208c-166">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e208c-166">Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e208c-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e208c-167">JSON representation</span></span>

<span data-ttu-id="e208c-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e208c-168">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdDateTime": "2020-02-12T22:06:58.303Z",
  "completedDate": "2020-02-12T22:14:28.19Z",
  "id": "1244d439-5baa-4b9a-be5f-e8fdef5a998b",
  "requestType": "UserAdd",
  "requestState": "Delivered",
  "requestStatus": "FulfilledNotificationTriggered",
  "isValidationOnly": false,
  "justification": ""
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
