---
title: tipo de recurso accessPackageAssignmentRequest
description: Uma solicitação de atribuição de pacote do Access é criada por um usuário que deseja obter uma atribuição de pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3a3309df4106d30de2190b1c321adb3ea0b1a670
ms.sourcegitcommit: 01f73b4dce6f885da18d62fe800b387c286c7a8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/09/2020
ms.locfileid: "47413307"
---
# <a name="accesspackageassignmentrequest-resource-type"></a><span data-ttu-id="29725-103">tipo de recurso accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="29725-103">accessPackageAssignmentRequest resource type</span></span>

<span data-ttu-id="29725-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29725-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29725-105">No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma solicitação de atribuição de pacote de acesso é criada por ou em nome de um usuário que deseja obter uma atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="29725-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by or on behalf of a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="29725-106">Se a solicitação for bem-sucedida, com todas as aprovações necessárias, o usuário receberá uma atribuição de pacote de acesso e será o assunto dessa atribuição de pacote de acesso resultante.</span><span class="sxs-lookup"><span data-stu-id="29725-106">If the request is successful, with any necessary approvals, the user receives an access package assignment, and is the subject of that resulting access package assignment.</span></span>  <span data-ttu-id="29725-107">O Azure AD também cria solicitações de atribuição de pacote de acesso automaticamente para rastrear a remoção do acesso.</span><span class="sxs-lookup"><span data-stu-id="29725-107">Azure AD also creates access package assignment requests automatically for tracking access removal.</span></span>

## <a name="methods"></a><span data-ttu-id="29725-108">Methods</span><span class="sxs-lookup"><span data-stu-id="29725-108">Methods</span></span>

| <span data-ttu-id="29725-109">Método</span><span class="sxs-lookup"><span data-stu-id="29725-109">Method</span></span>       | <span data-ttu-id="29725-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="29725-110">Return Type</span></span> | <span data-ttu-id="29725-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="29725-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="29725-112">Listar accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="29725-112">List accessPackageAssignmentRequests</span></span>](../api/accesspackageassignmentrequest-list.md) | <span data-ttu-id="29725-113">coleção [accessPackageAssignmentRequest](accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="29725-113">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) collection</span></span> | <span data-ttu-id="29725-114">Recupere uma lista de objetos accesspackageassignmentrequest.</span><span class="sxs-lookup"><span data-stu-id="29725-114">Retrieve a list of accesspackageassignmentrequest objects.</span></span> |
| [<span data-ttu-id="29725-115">Criar accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="29725-115">Create accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-post.md) | [<span data-ttu-id="29725-116">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="29725-116">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="29725-117">Criar um novo accessPackageAssignmentRequest.</span><span class="sxs-lookup"><span data-stu-id="29725-117">Create a new accessPackageAssignmentRequest.</span></span> |
| [<span data-ttu-id="29725-118">Obter accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="29725-118">Get accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-get.md) | [<span data-ttu-id="29725-119">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="29725-119">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="29725-120">Ler propriedades e relações de um objeto accessPackageAssignmentRequest.</span><span class="sxs-lookup"><span data-stu-id="29725-120">Read properties and relationships of an accessPackageAssignmentRequest object.</span></span> |

## <a name="properties"></a><span data-ttu-id="29725-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="29725-121">Properties</span></span>

| <span data-ttu-id="29725-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29725-122">Property</span></span>     | <span data-ttu-id="29725-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="29725-123">Type</span></span>        | <span data-ttu-id="29725-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="29725-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="29725-125">completedDate</span><span class="sxs-lookup"><span data-stu-id="29725-125">completedDate</span></span>|<span data-ttu-id="29725-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29725-126">DateTimeOffset</span></span>|<span data-ttu-id="29725-127">A data do final do processamento, bem como êxito ou falha, de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="29725-127">The date of the end of processing, either successful or failure, of a request.</span></span> <span data-ttu-id="29725-128">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="29725-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="29725-129">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="29725-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="29725-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="29725-130">Read-only.</span></span>|
|<span data-ttu-id="29725-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29725-131">createdDateTime</span></span>|<span data-ttu-id="29725-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29725-132">DateTimeOffset</span></span>|<span data-ttu-id="29725-133">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="29725-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="29725-134">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="29725-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="29725-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="29725-135">Read-only.</span></span>|
|<span data-ttu-id="29725-136">id</span><span class="sxs-lookup"><span data-stu-id="29725-136">id</span></span>|<span data-ttu-id="29725-137">String</span><span class="sxs-lookup"><span data-stu-id="29725-137">String</span></span>| <span data-ttu-id="29725-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="29725-138">Read-only.</span></span>|
|<span data-ttu-id="29725-139">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="29725-139">isValidationOnly</span></span>|<span data-ttu-id="29725-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="29725-140">Boolean</span></span>|<span data-ttu-id="29725-141">True se a solicitação não deve ser processada para a atribuição.</span><span class="sxs-lookup"><span data-stu-id="29725-141">True if the request is not to be processed for assignment.</span></span>|
|<span data-ttu-id="29725-142">elabora</span><span class="sxs-lookup"><span data-stu-id="29725-142">justification</span></span>|<span data-ttu-id="29725-143">String</span><span class="sxs-lookup"><span data-stu-id="29725-143">String</span></span>|<span data-ttu-id="29725-144">A justificativa fornecida pelo solicitante.</span><span class="sxs-lookup"><span data-stu-id="29725-144">The requestor's supplied justification.</span></span>|
|<span data-ttu-id="29725-145">RequestState</span><span class="sxs-lookup"><span data-stu-id="29725-145">requestState</span></span>|<span data-ttu-id="29725-146">String</span><span class="sxs-lookup"><span data-stu-id="29725-146">String</span></span>|<span data-ttu-id="29725-147">Um dos `PendingApproval` , `Canceled` ,  `Denied` , `Delivering` , `Delivered` , `PartiallyDelivered` `Submitted` ou `Scheduled` .</span><span class="sxs-lookup"><span data-stu-id="29725-147">One of `PendingApproval`, `Canceled`,  `Denied`, `Delivering`, `Delivered`, `PartiallyDelivered`, `Submitted` or `Scheduled`.</span></span> <span data-ttu-id="29725-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="29725-148">Read-only.</span></span>|
|<span data-ttu-id="29725-149">requestStatus</span><span class="sxs-lookup"><span data-stu-id="29725-149">requestStatus</span></span>|<span data-ttu-id="29725-150">String</span><span class="sxs-lookup"><span data-stu-id="29725-150">String</span></span>|<span data-ttu-id="29725-151">Mais informações sobre o status do processamento da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29725-151">More information on the request processing status.</span></span> <span data-ttu-id="29725-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="29725-152">Read-only.</span></span>|
|<span data-ttu-id="29725-153">RequestType</span><span class="sxs-lookup"><span data-stu-id="29725-153">requestType</span></span>|<span data-ttu-id="29725-154">String</span><span class="sxs-lookup"><span data-stu-id="29725-154">String</span></span>|<span data-ttu-id="29725-155">Um de `UserAdd` , `UserRemove` , `AdminAdd` `AdminRemove` ou `SystemRemove` .</span><span class="sxs-lookup"><span data-stu-id="29725-155">One of `UserAdd`, `UserRemove`, `AdminAdd`, `AdminRemove` or `SystemRemove`.</span></span> <span data-ttu-id="29725-156">Uma solicitação do próprio usuário teria o RequestType de `UserAdd` ou `UserRemove` .</span><span class="sxs-lookup"><span data-stu-id="29725-156">A request from the user themselves would have requestType of `UserAdd` or `UserRemove`.</span></span> <span data-ttu-id="29725-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="29725-157">Read-only.</span></span>|
|<span data-ttu-id="29725-158">Cronograma</span><span class="sxs-lookup"><span data-stu-id="29725-158">schedule</span></span>|[<span data-ttu-id="29725-159">requestSchedule</span><span class="sxs-lookup"><span data-stu-id="29725-159">requestSchedule</span></span>](requestschedule.md)| <span data-ttu-id="29725-160">O intervalo de datas que o Access deve ser atribuído ao solicitante.</span><span class="sxs-lookup"><span data-stu-id="29725-160">The range of dates that access is to be assigned to the requestor.</span></span> <span data-ttu-id="29725-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="29725-161">Read-only.</span></span>|
|<span data-ttu-id="29725-162">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="29725-162">accessPackageAssignment</span></span>|[<span data-ttu-id="29725-163">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="29725-163">accessPackageAssignment</span></span>](accesspackageassignment.md)| <span data-ttu-id="29725-164">Para um RequestType `UserAdd` ou `AdminAdd` , esta é uma atribuição de pacote de acesso solicitada a ser criada.</span><span class="sxs-lookup"><span data-stu-id="29725-164">For a requestType of `UserAdd` or `AdminAdd`, this is an access package assignment requested to be created.</span></span>  <span data-ttu-id="29725-165">Para um RequestType de `UserRemove` , `AdminRemove` ou `SystemRemove` , isso tem a `id` propriedade de uma atribuição existente a ser removida.</span><span class="sxs-lookup"><span data-stu-id="29725-165">For a requestType of `UserRemove`, `AdminRemove` or `SystemRemove`, this has the `id` property of an existing assignment to be removed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29725-166">Relações</span><span class="sxs-lookup"><span data-stu-id="29725-166">Relationships</span></span>

| <span data-ttu-id="29725-167">Relação</span><span class="sxs-lookup"><span data-stu-id="29725-167">Relationship</span></span> | <span data-ttu-id="29725-168">Tipo</span><span class="sxs-lookup"><span data-stu-id="29725-168">Type</span></span>        | <span data-ttu-id="29725-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="29725-169">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="29725-170">solicitante</span><span class="sxs-lookup"><span data-stu-id="29725-170">requestor</span></span>|[<span data-ttu-id="29725-171">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="29725-171">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="29725-172">O assunto que solicitou ou, se uma atribuição direta, foi atribuído.</span><span class="sxs-lookup"><span data-stu-id="29725-172">The subject who requested or, if a direct assignment, was assigned.</span></span> <span data-ttu-id="29725-173">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="29725-173">Read-only.</span></span> <span data-ttu-id="29725-174">Anulável.</span><span class="sxs-lookup"><span data-stu-id="29725-174">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29725-175">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="29725-175">JSON representation</span></span>

<span data-ttu-id="29725-176">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="29725-176">The following is a JSON representation of the resource.</span></span>

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
