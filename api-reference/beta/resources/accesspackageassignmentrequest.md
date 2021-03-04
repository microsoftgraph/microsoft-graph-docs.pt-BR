---
title: Tipo de recurso accessPackageAssignmentRequest
description: Uma solicitação de atribuição de pacote de acesso é criada por um usuário que deseja obter uma atribuição de pacote de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 89977897860133b92fc445036296de283a56b922
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433261"
---
# <a name="accesspackageassignmentrequest-resource-type"></a><span data-ttu-id="178aa-103">Tipo de recurso accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="178aa-103">accessPackageAssignmentRequest resource type</span></span>

<span data-ttu-id="178aa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="178aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="178aa-105">No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)uma solicitação de atribuição de pacote de acesso é criada por ou em nome de um usuário que deseja obter uma atribuição de pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="178aa-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by or on behalf of a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="178aa-106">Se a solicitação for bem-sucedida, com todas as aprovações necessárias, o usuário receberá uma atribuição de pacote de acesso e será o assunto dessa atribuição de pacote de acesso resultante.</span><span class="sxs-lookup"><span data-stu-id="178aa-106">If the request is successful, with any necessary approvals, the user receives an access package assignment, and is the subject of that resulting access package assignment.</span></span>  <span data-ttu-id="178aa-107">O Azure AD também cria solicitações de atribuição de pacote de acesso automaticamente para controlar a remoção de acesso.</span><span class="sxs-lookup"><span data-stu-id="178aa-107">Azure AD also creates access package assignment requests automatically for tracking access removal.</span></span>

## <a name="methods"></a><span data-ttu-id="178aa-108">Methods</span><span class="sxs-lookup"><span data-stu-id="178aa-108">Methods</span></span>

| <span data-ttu-id="178aa-109">Método</span><span class="sxs-lookup"><span data-stu-id="178aa-109">Method</span></span>       | <span data-ttu-id="178aa-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="178aa-110">Return Type</span></span> | <span data-ttu-id="178aa-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="178aa-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="178aa-112">Listar accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="178aa-112">List accessPackageAssignmentRequests</span></span>](../api/accesspackageassignmentrequest-list.md) | <span data-ttu-id="178aa-113">[coleção accessPackageAssignmentRequest](accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="178aa-113">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) collection</span></span> | <span data-ttu-id="178aa-114">Recupere uma lista de objetos accesspackageassignmentrequest.</span><span class="sxs-lookup"><span data-stu-id="178aa-114">Retrieve a list of accesspackageassignmentrequest objects.</span></span> |
| [<span data-ttu-id="178aa-115">Criar accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="178aa-115">Create accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-post.md) | [<span data-ttu-id="178aa-116">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="178aa-116">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="178aa-117">Crie um novo accessPackageAssignmentRequest.</span><span class="sxs-lookup"><span data-stu-id="178aa-117">Create a new accessPackageAssignmentRequest.</span></span> |
| [<span data-ttu-id="178aa-118">Obter accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="178aa-118">Get accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-get.md) | [<span data-ttu-id="178aa-119">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="178aa-119">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="178aa-120">Leia propriedades e relações de um objeto accessPackageAssignmentRequest.</span><span class="sxs-lookup"><span data-stu-id="178aa-120">Read properties and relationships of an accessPackageAssignmentRequest object.</span></span> |

## <a name="properties"></a><span data-ttu-id="178aa-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="178aa-121">Properties</span></span>

| <span data-ttu-id="178aa-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="178aa-122">Property</span></span>     | <span data-ttu-id="178aa-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="178aa-123">Type</span></span>        | <span data-ttu-id="178aa-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="178aa-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="178aa-125">completedDate</span><span class="sxs-lookup"><span data-stu-id="178aa-125">completedDate</span></span>|<span data-ttu-id="178aa-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="178aa-126">DateTimeOffset</span></span>|<span data-ttu-id="178aa-127">A data do final do processamento, bem-sucedida ou falha, de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="178aa-127">The date of the end of processing, either successful or failure, of a request.</span></span> <span data-ttu-id="178aa-128">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="178aa-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="178aa-129">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="178aa-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="178aa-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="178aa-130">Read-only.</span></span>|
|<span data-ttu-id="178aa-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="178aa-131">createdDateTime</span></span>|<span data-ttu-id="178aa-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="178aa-132">DateTimeOffset</span></span>|<span data-ttu-id="178aa-133">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="178aa-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="178aa-134">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="178aa-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="178aa-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="178aa-135">Read-only.</span></span>|
|<span data-ttu-id="178aa-136">id</span><span class="sxs-lookup"><span data-stu-id="178aa-136">id</span></span>|<span data-ttu-id="178aa-137">String</span><span class="sxs-lookup"><span data-stu-id="178aa-137">String</span></span>| <span data-ttu-id="178aa-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="178aa-138">Read-only.</span></span>|
|<span data-ttu-id="178aa-139">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="178aa-139">isValidationOnly</span></span>|<span data-ttu-id="178aa-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="178aa-140">Boolean</span></span>|<span data-ttu-id="178aa-141">True se a solicitação não for processada para atribuição.</span><span class="sxs-lookup"><span data-stu-id="178aa-141">True if the request is not to be processed for assignment.</span></span>|
|<span data-ttu-id="178aa-142">justification</span><span class="sxs-lookup"><span data-stu-id="178aa-142">justification</span></span>|<span data-ttu-id="178aa-143">String</span><span class="sxs-lookup"><span data-stu-id="178aa-143">String</span></span>|<span data-ttu-id="178aa-144">A justificativa fornecida pelo solicitante.</span><span class="sxs-lookup"><span data-stu-id="178aa-144">The requestor's supplied justification.</span></span>|
|<span data-ttu-id="178aa-145">requestState</span><span class="sxs-lookup"><span data-stu-id="178aa-145">requestState</span></span>|<span data-ttu-id="178aa-146">String</span><span class="sxs-lookup"><span data-stu-id="178aa-146">String</span></span>|<span data-ttu-id="178aa-147">Um dos `PendingApproval` , , , , , ou `Canceled`  `Denied` `Delivering` `Delivered` `PartiallyDelivered` `Submitted` `Scheduled` .</span><span class="sxs-lookup"><span data-stu-id="178aa-147">One of `PendingApproval`, `Canceled`,  `Denied`, `Delivering`, `Delivered`, `PartiallyDelivered`, `Submitted` or `Scheduled`.</span></span> <span data-ttu-id="178aa-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="178aa-148">Read-only.</span></span>|
|<span data-ttu-id="178aa-149">requestStatus</span><span class="sxs-lookup"><span data-stu-id="178aa-149">requestStatus</span></span>|<span data-ttu-id="178aa-150">String</span><span class="sxs-lookup"><span data-stu-id="178aa-150">String</span></span>|<span data-ttu-id="178aa-151">Mais informações sobre o status do processamento de solicitação.</span><span class="sxs-lookup"><span data-stu-id="178aa-151">More information on the request processing status.</span></span> <span data-ttu-id="178aa-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="178aa-152">Read-only.</span></span>|
|<span data-ttu-id="178aa-153">requestType</span><span class="sxs-lookup"><span data-stu-id="178aa-153">requestType</span></span>|<span data-ttu-id="178aa-154">String</span><span class="sxs-lookup"><span data-stu-id="178aa-154">String</span></span>|<span data-ttu-id="178aa-155">Um dos `UserAdd` , `UserRemove` , ou `AdminAdd` `AdminRemove` `SystemRemove` .</span><span class="sxs-lookup"><span data-stu-id="178aa-155">One of `UserAdd`, `UserRemove`, `AdminAdd`, `AdminRemove` or `SystemRemove`.</span></span> <span data-ttu-id="178aa-156">Uma solicitação do próprio usuário teria requestType de `UserAdd` ou `UserRemove` .</span><span class="sxs-lookup"><span data-stu-id="178aa-156">A request from the user themselves would have requestType of `UserAdd` or `UserRemove`.</span></span> <span data-ttu-id="178aa-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="178aa-157">Read-only.</span></span>|
|<span data-ttu-id="178aa-158">Cronograma</span><span class="sxs-lookup"><span data-stu-id="178aa-158">schedule</span></span>|[<span data-ttu-id="178aa-159">requestSchedule</span><span class="sxs-lookup"><span data-stu-id="178aa-159">requestSchedule</span></span>](requestschedule.md)| <span data-ttu-id="178aa-160">O intervalo de datas que o acesso deve ser atribuído ao solicitante.</span><span class="sxs-lookup"><span data-stu-id="178aa-160">The range of dates that access is to be assigned to the requestor.</span></span> <span data-ttu-id="178aa-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="178aa-161">Read-only.</span></span>|
|<span data-ttu-id="178aa-162">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="178aa-162">accessPackageAssignment</span></span>|[<span data-ttu-id="178aa-163">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="178aa-163">accessPackageAssignment</span></span>](accesspackageassignment.md)| <span data-ttu-id="178aa-164">Para um requestType de `UserAdd` ou , esta é uma `AdminAdd` atribuição de pacote de acesso solicitada a ser criada.</span><span class="sxs-lookup"><span data-stu-id="178aa-164">For a requestType of `UserAdd` or `AdminAdd`, this is an access package assignment requested to be created.</span></span>  <span data-ttu-id="178aa-165">Para um requestType `UserRemove` de , ou , isso tem a propriedade de uma `AdminRemove` `SystemRemove` `id` atribuição existente a ser removida.</span><span class="sxs-lookup"><span data-stu-id="178aa-165">For a requestType of `UserRemove`, `AdminRemove` or `SystemRemove`, this has the `id` property of an existing assignment to be removed.</span></span>|
|<span data-ttu-id="178aa-166">answers</span><span class="sxs-lookup"><span data-stu-id="178aa-166">answers</span></span>|<span data-ttu-id="178aa-167">[Coleção accessPackageAnswer](accesspackageanswer.md)</span><span class="sxs-lookup"><span data-stu-id="178aa-167">[accessPackageAnswer](accesspackageanswer.md) collection</span></span>|<span data-ttu-id="178aa-168">Respostas fornecidas pelo solicitante para [acessarPackageQuestions solicitadas](accesspackagequestion.md) no momento da solicitação.</span><span class="sxs-lookup"><span data-stu-id="178aa-168">Answers provided by the requestor to [accessPackageQuestions](accesspackagequestion.md) asked of them at the time of request.</span></span>|

## <a name="relationships"></a><span data-ttu-id="178aa-169">Relações</span><span class="sxs-lookup"><span data-stu-id="178aa-169">Relationships</span></span>

| <span data-ttu-id="178aa-170">Relação</span><span class="sxs-lookup"><span data-stu-id="178aa-170">Relationship</span></span> | <span data-ttu-id="178aa-171">Tipo</span><span class="sxs-lookup"><span data-stu-id="178aa-171">Type</span></span>        | <span data-ttu-id="178aa-172">Descrição</span><span class="sxs-lookup"><span data-stu-id="178aa-172">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="178aa-173">requestor</span><span class="sxs-lookup"><span data-stu-id="178aa-173">requestor</span></span>|[<span data-ttu-id="178aa-174">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="178aa-174">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="178aa-175">O assunto que solicitou ou, se uma atribuição direta, foi atribuído.</span><span class="sxs-lookup"><span data-stu-id="178aa-175">The subject who requested or, if a direct assignment, was assigned.</span></span> <span data-ttu-id="178aa-176">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="178aa-176">Read-only.</span></span> <span data-ttu-id="178aa-177">Anulável.</span><span class="sxs-lookup"><span data-stu-id="178aa-177">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="178aa-178">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="178aa-178">JSON representation</span></span>

<span data-ttu-id="178aa-179">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="178aa-179">The following is a JSON representation of the resource.</span></span>

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

