---
title: tipo de recurso accessPackageAssignmentRequest
description: Uma solicitação de atribuição de pacote do Access é criada por um usuário que deseja obter uma atribuição de pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a6be3fa431a2216ef8b31b673a5f73ef6067fff9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939198"
---
# <a name="accesspackageassignmentrequest-resource-type"></a><span data-ttu-id="f373d-103">tipo de recurso accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f373d-103">accessPackageAssignmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f373d-104">No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma solicitação de atribuição de pacote de acesso é criada por um usuário que deseja obter uma atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="f373d-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="f373d-105">Se a solicitação for bem-sucedida, com todas as aprovações necessárias, o usuário receberá uma atribuição de pacote de acesso e será o assunto dessa atribuição de pacote de acesso resultante.</span><span class="sxs-lookup"><span data-stu-id="f373d-105">If the request is successful, with any necessary approvals, the user receives an access package assignment, and is the subject of that resulting access package assignment.</span></span>


## <a name="methods"></a><span data-ttu-id="f373d-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="f373d-106">Methods</span></span>

| <span data-ttu-id="f373d-107">Método</span><span class="sxs-lookup"><span data-stu-id="f373d-107">Method</span></span>       | <span data-ttu-id="f373d-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f373d-108">Return Type</span></span> | <span data-ttu-id="f373d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f373d-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f373d-110">Listar accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="f373d-110">List accessPackageAssignmentRequests</span></span>](../api/accesspackageassignmentrequest-list.md) | <span data-ttu-id="f373d-111">coleção [accessPackageAssignmentRequest](accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="f373d-111">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) collection</span></span> | <span data-ttu-id="f373d-112">Recupere uma lista de objetos accesspackageassignmentrequest.</span><span class="sxs-lookup"><span data-stu-id="f373d-112">Retrieve a list of accesspackageassignmentrequest objects.</span></span> |
| [<span data-ttu-id="f373d-113">Criar accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f373d-113">Create accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-post.md) | [<span data-ttu-id="f373d-114">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f373d-114">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="f373d-115">Criar um novo accessPackageAssignmentRequest.</span><span class="sxs-lookup"><span data-stu-id="f373d-115">Create a new accessPackageAssignmentRequest.</span></span> |
| [<span data-ttu-id="f373d-116">Obter accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f373d-116">Get accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-get.md) | [<span data-ttu-id="f373d-117">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f373d-117">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="f373d-118">Ler propriedades e relações de um objeto accessPackageAssignmentRequest.</span><span class="sxs-lookup"><span data-stu-id="f373d-118">Read properties and relationships of an accessPackageAssignmentRequest object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f373d-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f373d-119">Properties</span></span>

| <span data-ttu-id="f373d-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f373d-120">Property</span></span>     | <span data-ttu-id="f373d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="f373d-121">Type</span></span>        | <span data-ttu-id="f373d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f373d-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f373d-123">completedDate</span><span class="sxs-lookup"><span data-stu-id="f373d-123">completedDate</span></span>|<span data-ttu-id="f373d-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f373d-124">DateTimeOffset</span></span>|<span data-ttu-id="f373d-125">A data do final do processamento, bem como êxito ou falha, de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="f373d-125">The date of the end of processing, either successful or failure, of a request.</span></span> <span data-ttu-id="f373d-126">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f373d-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f373d-127">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f373d-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="f373d-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f373d-128">Read-only.</span></span>|
|<span data-ttu-id="f373d-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f373d-129">createdDateTime</span></span>|<span data-ttu-id="f373d-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f373d-130">DateTimeOffset</span></span>|<span data-ttu-id="f373d-131">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f373d-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f373d-132">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f373d-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="f373d-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f373d-133">Read-only.</span></span>|
|<span data-ttu-id="f373d-134">id</span><span class="sxs-lookup"><span data-stu-id="f373d-134">id</span></span>|<span data-ttu-id="f373d-135">String</span><span class="sxs-lookup"><span data-stu-id="f373d-135">String</span></span>| <span data-ttu-id="f373d-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f373d-136">Read-only.</span></span>|
|<span data-ttu-id="f373d-137">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="f373d-137">isValidationOnly</span></span>|<span data-ttu-id="f373d-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="f373d-138">Boolean</span></span>|<span data-ttu-id="f373d-139">True se a solicitação não deve ser processada para a atribuição.</span><span class="sxs-lookup"><span data-stu-id="f373d-139">True if the request is not to be processed for assignment.</span></span>|
|<span data-ttu-id="f373d-140">elabora</span><span class="sxs-lookup"><span data-stu-id="f373d-140">justification</span></span>|<span data-ttu-id="f373d-141">String</span><span class="sxs-lookup"><span data-stu-id="f373d-141">String</span></span>|<span data-ttu-id="f373d-142">A justificativa fornecida pelo solicitante.</span><span class="sxs-lookup"><span data-stu-id="f373d-142">The requestor's supplied justification.</span></span>|
|<span data-ttu-id="f373d-143">RequestState</span><span class="sxs-lookup"><span data-stu-id="f373d-143">requestState</span></span>|<span data-ttu-id="f373d-144">String</span><span class="sxs-lookup"><span data-stu-id="f373d-144">String</span></span>|<span data-ttu-id="f373d-145">Um dos `Denied`, `Delivered`, `PartiallyDelivered`,.</span><span class="sxs-lookup"><span data-stu-id="f373d-145">One of `Denied`, `Delivered`, `PartiallyDelivered`.</span></span> <span data-ttu-id="f373d-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f373d-146">Read-only.</span></span>|
|<span data-ttu-id="f373d-147">requestStatus</span><span class="sxs-lookup"><span data-stu-id="f373d-147">requestStatus</span></span>|<span data-ttu-id="f373d-148">String</span><span class="sxs-lookup"><span data-stu-id="f373d-148">String</span></span>|<span data-ttu-id="f373d-149">Mais informações sobre o status do processamento da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f373d-149">More information on the request processing status.</span></span> <span data-ttu-id="f373d-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f373d-150">Read-only.</span></span>|
|<span data-ttu-id="f373d-151">RequestType</span><span class="sxs-lookup"><span data-stu-id="f373d-151">requestType</span></span>|<span data-ttu-id="f373d-152">String</span><span class="sxs-lookup"><span data-stu-id="f373d-152">String</span></span>|<span data-ttu-id="f373d-153">Um `UserAdd` ou `UserRemove`.</span><span class="sxs-lookup"><span data-stu-id="f373d-153">One of `UserAdd` or `UserRemove`.</span></span> <span data-ttu-id="f373d-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f373d-154">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="f373d-155">Relações</span><span class="sxs-lookup"><span data-stu-id="f373d-155">Relationships</span></span>

| <span data-ttu-id="f373d-156">Relação</span><span class="sxs-lookup"><span data-stu-id="f373d-156">Relationship</span></span> | <span data-ttu-id="f373d-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="f373d-157">Type</span></span>        | <span data-ttu-id="f373d-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="f373d-158">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f373d-159">solicitante</span><span class="sxs-lookup"><span data-stu-id="f373d-159">requestor</span></span>|[<span data-ttu-id="f373d-160">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="f373d-160">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="f373d-161">O assunto que solicitou ou, se uma atribuição direta, foi atribuído.</span><span class="sxs-lookup"><span data-stu-id="f373d-161">The subject who requested or, if a direct assignment, was assigned.</span></span> <span data-ttu-id="f373d-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f373d-162">Read-only.</span></span> <span data-ttu-id="f373d-163">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f373d-163">Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f373d-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f373d-164">JSON representation</span></span>

<span data-ttu-id="f373d-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f373d-165">The following is a JSON representation of the resource.</span></span>

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
