---
title: Tipo de recurso accessPackageAssignmentRequest
description: Uma solicitação de atribuição de pacote de acesso é criada por um usuário que deseja obter uma atribuição de pacote de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7825b19e80274c8bcd54a5d8d03aa1dd40cf49c9
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52298495"
---
# <a name="accesspackageassignmentrequest-resource-type"></a><span data-ttu-id="38f96-103">Tipo de recurso accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="38f96-103">accessPackageAssignmentRequest resource type</span></span>

<span data-ttu-id="38f96-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38f96-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38f96-105">No [Azure AD Entitlement Management](entitlementmanagement-root.md), uma solicitação de atribuição de pacote de acesso é criada por ou em nome de um usuário que deseja obter uma atribuição de pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="38f96-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), an access package assignment request is created by or on behalf of a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="38f96-106">Se a solicitação for bem-sucedida, com todas as aprovações necessárias, o usuário receberá uma atribuição de pacote de acesso e será o assunto dessa atribuição de pacote de acesso resultante.</span><span class="sxs-lookup"><span data-stu-id="38f96-106">If the request is successful, with any necessary approvals, the user receives an access package assignment, and is the subject of that resulting access package assignment.</span></span>  <span data-ttu-id="38f96-107">O Azure AD também cria solicitações de atribuição de pacote de acesso automaticamente para controlar a remoção de acesso.</span><span class="sxs-lookup"><span data-stu-id="38f96-107">Azure AD also creates access package assignment requests automatically for tracking access removal.</span></span>

## <a name="methods"></a><span data-ttu-id="38f96-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="38f96-108">Methods</span></span>

| <span data-ttu-id="38f96-109">Método</span><span class="sxs-lookup"><span data-stu-id="38f96-109">Method</span></span>       | <span data-ttu-id="38f96-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="38f96-110">Return Type</span></span> | <span data-ttu-id="38f96-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="38f96-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="38f96-112">Listar accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="38f96-112">List accessPackageAssignmentRequests</span></span>](../api/accesspackageassignmentrequest-list.md) | <span data-ttu-id="38f96-113">[coleção accessPackageAssignmentRequest](accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="38f96-113">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) collection</span></span> | <span data-ttu-id="38f96-114">Recupere uma lista **de objetos accesspackageassignmentrequest.**</span><span class="sxs-lookup"><span data-stu-id="38f96-114">Retrieve a list of **accesspackageassignmentrequest** objects.</span></span> |
| [<span data-ttu-id="38f96-115">Criar accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="38f96-115">Create accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-post.md) | [<span data-ttu-id="38f96-116">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="38f96-116">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="38f96-117">Crie um novo **accessPackageAssignmentRequest**.</span><span class="sxs-lookup"><span data-stu-id="38f96-117">Create a new **accessPackageAssignmentRequest**.</span></span> |
| [<span data-ttu-id="38f96-118">Obter accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="38f96-118">Get accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-get.md) | [<span data-ttu-id="38f96-119">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="38f96-119">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="38f96-120">Leia propriedades e relações de um **objeto accessPackageAssignmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="38f96-120">Read properties and relationships of an **accessPackageAssignmentRequest** object.</span></span> |
|[<span data-ttu-id="38f96-121">filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="38f96-121">filterByCurrentUser</span></span>](../api/accesspackageassignmentrequest-filterbycurrentuser.md)|<span data-ttu-id="38f96-122">[coleção accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="38f96-122">[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) collection</span></span>|<span data-ttu-id="38f96-123">Recupere a lista de **objetos accessPackageAssignmentRequest** filtrados no usuário de entrada.</span><span class="sxs-lookup"><span data-stu-id="38f96-123">Retrieve the list of **accessPackageAssignmentRequest** objects filtered on the signed-in user.</span></span>|
|[<span data-ttu-id="38f96-124">cancel</span><span class="sxs-lookup"><span data-stu-id="38f96-124">cancel</span></span>](../api/accesspackageassignmentrequest-cancel.md)|<span data-ttu-id="38f96-125">[coleção accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="38f96-125">[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) collection</span></span>|<span data-ttu-id="38f96-126">Cancele **um objeto accessPackageAssignmentRequest** que está em estado cancelável.</span><span class="sxs-lookup"><span data-stu-id="38f96-126">Cancel an **accessPackageAssignmentRequest** object that is in a cancellable state.</span></span>|

## <a name="properties"></a><span data-ttu-id="38f96-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="38f96-127">Properties</span></span>

| <span data-ttu-id="38f96-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38f96-128">Property</span></span>     | <span data-ttu-id="38f96-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="38f96-129">Type</span></span>        | <span data-ttu-id="38f96-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="38f96-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="38f96-131">completedDate</span><span class="sxs-lookup"><span data-stu-id="38f96-131">completedDate</span></span>|<span data-ttu-id="38f96-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38f96-132">DateTimeOffset</span></span>|<span data-ttu-id="38f96-133">A data do final do processamento, bem-sucedida ou falha, de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="38f96-133">The date of the end of processing, either successful or failure, of a request.</span></span> <span data-ttu-id="38f96-134">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="38f96-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="38f96-135">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="38f96-135">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="38f96-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38f96-136">Read-only.</span></span>|
|<span data-ttu-id="38f96-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="38f96-137">createdDateTime</span></span>|<span data-ttu-id="38f96-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38f96-138">DateTimeOffset</span></span>|<span data-ttu-id="38f96-139">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="38f96-139">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="38f96-140">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="38f96-140">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="38f96-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38f96-141">Read-only.</span></span>|
|<span data-ttu-id="38f96-142">id</span><span class="sxs-lookup"><span data-stu-id="38f96-142">id</span></span>|<span data-ttu-id="38f96-143">String</span><span class="sxs-lookup"><span data-stu-id="38f96-143">String</span></span>| <span data-ttu-id="38f96-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38f96-144">Read-only.</span></span>|
|<span data-ttu-id="38f96-145">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="38f96-145">isValidationOnly</span></span>|<span data-ttu-id="38f96-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="38f96-146">Boolean</span></span>|<span data-ttu-id="38f96-147">True se a solicitação não for processada para atribuição.</span><span class="sxs-lookup"><span data-stu-id="38f96-147">True if the request is not to be processed for assignment.</span></span>|
|<span data-ttu-id="38f96-148">justification</span><span class="sxs-lookup"><span data-stu-id="38f96-148">justification</span></span>|<span data-ttu-id="38f96-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38f96-149">String</span></span>|<span data-ttu-id="38f96-150">A justificativa fornecida pelo solicitante.</span><span class="sxs-lookup"><span data-stu-id="38f96-150">The requestor's supplied justification.</span></span>|
|<span data-ttu-id="38f96-151">requestState</span><span class="sxs-lookup"><span data-stu-id="38f96-151">requestState</span></span>|<span data-ttu-id="38f96-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38f96-152">String</span></span>|<span data-ttu-id="38f96-153">Um dos `PendingApproval` , , , , , ou `Canceled`  `Denied` `Delivering` `Delivered` `PartiallyDelivered` `Submitted` `Scheduled` .</span><span class="sxs-lookup"><span data-stu-id="38f96-153">One of `PendingApproval`, `Canceled`,  `Denied`, `Delivering`, `Delivered`, `PartiallyDelivered`, `Submitted` or `Scheduled`.</span></span> <span data-ttu-id="38f96-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38f96-154">Read-only.</span></span>|
|<span data-ttu-id="38f96-155">requestStatus</span><span class="sxs-lookup"><span data-stu-id="38f96-155">requestStatus</span></span>|<span data-ttu-id="38f96-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38f96-156">String</span></span>|<span data-ttu-id="38f96-157">Mais informações sobre o status do processamento de solicitação.</span><span class="sxs-lookup"><span data-stu-id="38f96-157">More information on the request processing status.</span></span> <span data-ttu-id="38f96-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38f96-158">Read-only.</span></span>|
|<span data-ttu-id="38f96-159">requestType</span><span class="sxs-lookup"><span data-stu-id="38f96-159">requestType</span></span>|<span data-ttu-id="38f96-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38f96-160">String</span></span>|<span data-ttu-id="38f96-161">Um dos `UserAdd` , `UserRemove` , ou `AdminAdd` `AdminRemove` `SystemRemove` .</span><span class="sxs-lookup"><span data-stu-id="38f96-161">One of `UserAdd`, `UserRemove`, `AdminAdd`, `AdminRemove` or `SystemRemove`.</span></span> <span data-ttu-id="38f96-162">Uma solicitação do próprio usuário teria requestType de `UserAdd` ou `UserRemove` .</span><span class="sxs-lookup"><span data-stu-id="38f96-162">A request from the user themselves would have requestType of `UserAdd` or `UserRemove`.</span></span> <span data-ttu-id="38f96-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38f96-163">Read-only.</span></span>|
|<span data-ttu-id="38f96-164">Cronograma</span><span class="sxs-lookup"><span data-stu-id="38f96-164">schedule</span></span>|[<span data-ttu-id="38f96-165">requestSchedule</span><span class="sxs-lookup"><span data-stu-id="38f96-165">requestSchedule</span></span>](requestschedule.md)| <span data-ttu-id="38f96-166">O intervalo de datas que o acesso deve ser atribuído ao solicitante.</span><span class="sxs-lookup"><span data-stu-id="38f96-166">The range of dates that access is to be assigned to the requestor.</span></span> <span data-ttu-id="38f96-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38f96-167">Read-only.</span></span>|
|<span data-ttu-id="38f96-168">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="38f96-168">accessPackageAssignment</span></span>|[<span data-ttu-id="38f96-169">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="38f96-169">accessPackageAssignment</span></span>](accesspackageassignment.md)| <span data-ttu-id="38f96-170">Para um requestType de `UserAdd` ou , esta é uma `AdminAdd` atribuição de pacote de acesso solicitada a ser criada.</span><span class="sxs-lookup"><span data-stu-id="38f96-170">For a requestType of `UserAdd` or `AdminAdd`, this is an access package assignment requested to be created.</span></span>  <span data-ttu-id="38f96-171">Para um requestType `UserRemove` de , ou , isso tem a propriedade de uma `AdminRemove` `SystemRemove` `id` atribuição existente a ser removida.</span><span class="sxs-lookup"><span data-stu-id="38f96-171">For a requestType of `UserRemove`, `AdminRemove` or `SystemRemove`, this has the `id` property of an existing assignment to be removed.</span></span>|
|<span data-ttu-id="38f96-172">answers</span><span class="sxs-lookup"><span data-stu-id="38f96-172">answers</span></span>|<span data-ttu-id="38f96-173">[Coleção accessPackageAnswer](accesspackageanswer.md)</span><span class="sxs-lookup"><span data-stu-id="38f96-173">[accessPackageAnswer](accesspackageanswer.md) collection</span></span>|<span data-ttu-id="38f96-174">Respostas fornecidas pelo solicitante para [acessarPackageQuestions solicitadas](accesspackagequestion.md) no momento da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38f96-174">Answers provided by the requestor to [accessPackageQuestions](accesspackagequestion.md) asked of them at the time of request.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38f96-175">Relações</span><span class="sxs-lookup"><span data-stu-id="38f96-175">Relationships</span></span>

| <span data-ttu-id="38f96-176">Relação</span><span class="sxs-lookup"><span data-stu-id="38f96-176">Relationship</span></span> | <span data-ttu-id="38f96-177">Tipo</span><span class="sxs-lookup"><span data-stu-id="38f96-177">Type</span></span>        | <span data-ttu-id="38f96-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="38f96-178">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="38f96-179">accessPackage</span><span class="sxs-lookup"><span data-stu-id="38f96-179">accessPackage</span></span>|[<span data-ttu-id="38f96-180">accessPackage</span><span class="sxs-lookup"><span data-stu-id="38f96-180">accessPackage</span></span>](../resources/accesspackage.md)|<span data-ttu-id="38f96-181">O pacote de acesso associado ao accessPackageAssignmentRequest.</span><span class="sxs-lookup"><span data-stu-id="38f96-181">The access package associated with the accessPackageAssignmentRequest.</span></span> <span data-ttu-id="38f96-182">Um pacote de acesso define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos.</span><span class="sxs-lookup"><span data-stu-id="38f96-182">An access package defines the collections of resource roles and the policies for how one or more users can get access to those resources.</span></span> <span data-ttu-id="38f96-183">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38f96-183">Read-only.</span></span> <span data-ttu-id="38f96-184">Anulável.</span><span class="sxs-lookup"><span data-stu-id="38f96-184">Nullable.</span></span>|
|<span data-ttu-id="38f96-185">requestor</span><span class="sxs-lookup"><span data-stu-id="38f96-185">requestor</span></span>|[<span data-ttu-id="38f96-186">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="38f96-186">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="38f96-187">O assunto que solicitou ou, se uma atribuição direta, foi atribuído.</span><span class="sxs-lookup"><span data-stu-id="38f96-187">The subject who requested or, if a direct assignment, was assigned.</span></span> <span data-ttu-id="38f96-188">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38f96-188">Read-only.</span></span> <span data-ttu-id="38f96-189">Anulável.</span><span class="sxs-lookup"><span data-stu-id="38f96-189">Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="38f96-190">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="38f96-190">JSON representation</span></span>

<span data-ttu-id="38f96-191">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="38f96-191">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "keyProperty": "id"
}-->

```json
{
    "createdDateTime": "string",
    "completedDate": "string",
    "id": "string",
    "requestType": "string",
    "requestState": "string",
    "requestStatus": "string",
    "isValidationOnly": false,
    "justification": "string",
    "answers": [{
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "string",
        "answeredQuestion": {
            "id": "string",
            "text": {
                "defaultText": "string",
                "localizedTexts": [{
                    "text": "string",
                    "languageCode": "string"
                }]
            },
            "isRequired": true,
            "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
            "isSingleLineQuestion": true
        }
    }]
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

