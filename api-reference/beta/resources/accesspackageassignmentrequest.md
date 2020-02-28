---
title: tipo de recurso accessPackageAssignmentRequest
description: Uma solicitação de atribuição de pacote do Access é criada por um usuário que deseja obter uma atribuição de pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c2440dfc7e798ea5b0a197f60b62acce4199b4ca
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331266"
---
# <a name="accesspackageassignmentrequest-resource-type"></a><span data-ttu-id="cd778-103">tipo de recurso accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="cd778-103">accessPackageAssignmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd778-104">No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma solicitação de atribuição de pacote de acesso é criada por um usuário que deseja obter uma atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="cd778-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="cd778-105">Se a solicitação for bem-sucedida, com todas as aprovações necessárias, o usuário receberá uma atribuição de pacote de acesso e será o assunto dessa atribuição de pacote de acesso resultante.</span><span class="sxs-lookup"><span data-stu-id="cd778-105">If the request is successful, with any necessary approvals, the user receives an access package assignment, and is the subject of that resulting access package assignment.</span></span>  <span data-ttu-id="cd778-106">O Azure AD também cria solicitações de atribuição de pacote de acesso automaticamente para rastrear a remoção do acesso.</span><span class="sxs-lookup"><span data-stu-id="cd778-106">Azure AD also creates access package assignment requests automatically for tracking access removal.</span></span>


## <a name="methods"></a><span data-ttu-id="cd778-107">Methods</span><span class="sxs-lookup"><span data-stu-id="cd778-107">Methods</span></span>

| <span data-ttu-id="cd778-108">Método</span><span class="sxs-lookup"><span data-stu-id="cd778-108">Method</span></span>       | <span data-ttu-id="cd778-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cd778-109">Return Type</span></span> | <span data-ttu-id="cd778-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd778-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="cd778-111">Listar accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="cd778-111">List accessPackageAssignmentRequests</span></span>](../api/accesspackageassignmentrequest-list.md) | <span data-ttu-id="cd778-112">coleção [accessPackageAssignmentRequest](accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="cd778-112">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) collection</span></span> | <span data-ttu-id="cd778-113">Recupere uma lista de objetos accesspackageassignmentrequest.</span><span class="sxs-lookup"><span data-stu-id="cd778-113">Retrieve a list of accesspackageassignmentrequest objects.</span></span> |
| [<span data-ttu-id="cd778-114">Criar accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="cd778-114">Create accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-post.md) | [<span data-ttu-id="cd778-115">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="cd778-115">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="cd778-116">Criar um novo accessPackageAssignmentRequest.</span><span class="sxs-lookup"><span data-stu-id="cd778-116">Create a new accessPackageAssignmentRequest.</span></span> |
| [<span data-ttu-id="cd778-117">Obter accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="cd778-117">Get accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-get.md) | [<span data-ttu-id="cd778-118">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="cd778-118">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="cd778-119">Ler propriedades e relações de um objeto accessPackageAssignmentRequest.</span><span class="sxs-lookup"><span data-stu-id="cd778-119">Read properties and relationships of an accessPackageAssignmentRequest object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cd778-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cd778-120">Properties</span></span>

| <span data-ttu-id="cd778-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd778-121">Property</span></span>     | <span data-ttu-id="cd778-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd778-122">Type</span></span>        | <span data-ttu-id="cd778-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd778-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cd778-124">completedDate</span><span class="sxs-lookup"><span data-stu-id="cd778-124">completedDate</span></span>|<span data-ttu-id="cd778-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd778-125">DateTimeOffset</span></span>|<span data-ttu-id="cd778-126">A data do final do processamento, bem como êxito ou falha, de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd778-126">The date of the end of processing, either successful or failure, of a request.</span></span> <span data-ttu-id="cd778-127">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="cd778-127">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cd778-128">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="cd778-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="cd778-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cd778-129">Read-only.</span></span>|
|<span data-ttu-id="cd778-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cd778-130">createdDateTime</span></span>|<span data-ttu-id="cd778-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd778-131">DateTimeOffset</span></span>|<span data-ttu-id="cd778-132">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="cd778-132">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cd778-133">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="cd778-133">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="cd778-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cd778-134">Read-only.</span></span>|
|<span data-ttu-id="cd778-135">id</span><span class="sxs-lookup"><span data-stu-id="cd778-135">id</span></span>|<span data-ttu-id="cd778-136">String</span><span class="sxs-lookup"><span data-stu-id="cd778-136">String</span></span>| <span data-ttu-id="cd778-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cd778-137">Read-only.</span></span>|
|<span data-ttu-id="cd778-138">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="cd778-138">isValidationOnly</span></span>|<span data-ttu-id="cd778-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="cd778-139">Boolean</span></span>|<span data-ttu-id="cd778-140">True se a solicitação não deve ser processada para a atribuição.</span><span class="sxs-lookup"><span data-stu-id="cd778-140">True if the request is not to be processed for assignment.</span></span>|
|<span data-ttu-id="cd778-141">elabora</span><span class="sxs-lookup"><span data-stu-id="cd778-141">justification</span></span>|<span data-ttu-id="cd778-142">String</span><span class="sxs-lookup"><span data-stu-id="cd778-142">String</span></span>|<span data-ttu-id="cd778-143">A justificativa fornecida pelo solicitante.</span><span class="sxs-lookup"><span data-stu-id="cd778-143">The requestor's supplied justification.</span></span>|
|<span data-ttu-id="cd778-144">RequestState</span><span class="sxs-lookup"><span data-stu-id="cd778-144">requestState</span></span>|<span data-ttu-id="cd778-145">String</span><span class="sxs-lookup"><span data-stu-id="cd778-145">String</span></span>|<span data-ttu-id="cd778-146">Um de `Denied`, `Delivered`, `PartiallyDelivered` `Submitted` ou `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="cd778-146">One of `Denied`, `Delivered`, `PartiallyDelivered`, `Submitted` or `Scheduled`.</span></span> <span data-ttu-id="cd778-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cd778-147">Read-only.</span></span>|
|<span data-ttu-id="cd778-148">requestStatus</span><span class="sxs-lookup"><span data-stu-id="cd778-148">requestStatus</span></span>|<span data-ttu-id="cd778-149">String</span><span class="sxs-lookup"><span data-stu-id="cd778-149">String</span></span>|<span data-ttu-id="cd778-150">Mais informações sobre o status do processamento da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd778-150">More information on the request processing status.</span></span> <span data-ttu-id="cd778-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cd778-151">Read-only.</span></span>|
|<span data-ttu-id="cd778-152">RequestType</span><span class="sxs-lookup"><span data-stu-id="cd778-152">requestType</span></span>|<span data-ttu-id="cd778-153">String</span><span class="sxs-lookup"><span data-stu-id="cd778-153">String</span></span>|<span data-ttu-id="cd778-154">Um de `UserAdd`, `UserRemove`, `AdminAdd` `AdminRemove` ou `SystemRemove`.</span><span class="sxs-lookup"><span data-stu-id="cd778-154">One of `UserAdd`, `UserRemove`, `AdminAdd`, `AdminRemove` or `SystemRemove`.</span></span> <span data-ttu-id="cd778-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cd778-155">Read-only.</span></span>|
|<span data-ttu-id="cd778-156">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="cd778-156">accessPackageAssignment</span></span>|[<span data-ttu-id="cd778-157">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="cd778-157">accessPackageAssignment</span></span>](accesspackageassignment.md)| <span data-ttu-id="cd778-158">Uma atribuição de pacote de acesso solicitada foi criada.</span><span class="sxs-lookup"><span data-stu-id="cd778-158">An access package assignment requested to be created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd778-159">Relações</span><span class="sxs-lookup"><span data-stu-id="cd778-159">Relationships</span></span>

| <span data-ttu-id="cd778-160">Relação</span><span class="sxs-lookup"><span data-stu-id="cd778-160">Relationship</span></span> | <span data-ttu-id="cd778-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd778-161">Type</span></span>        | <span data-ttu-id="cd778-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd778-162">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cd778-163">solicitante</span><span class="sxs-lookup"><span data-stu-id="cd778-163">requestor</span></span>|[<span data-ttu-id="cd778-164">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="cd778-164">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="cd778-165">O assunto que solicitou ou, se uma atribuição direta, foi atribuído.</span><span class="sxs-lookup"><span data-stu-id="cd778-165">The subject who requested or, if a direct assignment, was assigned.</span></span> <span data-ttu-id="cd778-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cd778-166">Read-only.</span></span> <span data-ttu-id="cd778-167">Anulável.</span><span class="sxs-lookup"><span data-stu-id="cd778-167">Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="cd778-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cd778-168">JSON representation</span></span>

<span data-ttu-id="cd778-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cd778-169">The following is a JSON representation of the resource.</span></span>

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
