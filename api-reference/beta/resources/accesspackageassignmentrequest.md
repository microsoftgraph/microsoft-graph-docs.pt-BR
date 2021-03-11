---
title: Tipo de recurso accessPackageAssignmentRequest
description: Uma solicitação de atribuição de pacote de acesso é criada por um usuário que deseja obter uma atribuição de pacote de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 83218058d375a9f78a24b2af837c39fb5ee77a2c
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720435"
---
# <a name="accesspackageassignmentrequest-resource-type"></a><span data-ttu-id="2879e-103">Tipo de recurso accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="2879e-103">accessPackageAssignmentRequest resource type</span></span>

<span data-ttu-id="2879e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2879e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2879e-105">No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)uma solicitação de atribuição de pacote de acesso é criada por ou em nome de um usuário que deseja obter uma atribuição de pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="2879e-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by or on behalf of a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="2879e-106">Se a solicitação for bem-sucedida, com todas as aprovações necessárias, o usuário receberá uma atribuição de pacote de acesso e será o assunto dessa atribuição de pacote de acesso resultante.</span><span class="sxs-lookup"><span data-stu-id="2879e-106">If the request is successful, with any necessary approvals, the user receives an access package assignment, and is the subject of that resulting access package assignment.</span></span>  <span data-ttu-id="2879e-107">O Azure AD também cria solicitações de atribuição de pacote de acesso automaticamente para controlar a remoção de acesso.</span><span class="sxs-lookup"><span data-stu-id="2879e-107">Azure AD also creates access package assignment requests automatically for tracking access removal.</span></span>

## <a name="methods"></a><span data-ttu-id="2879e-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="2879e-108">Methods</span></span>

| <span data-ttu-id="2879e-109">Método</span><span class="sxs-lookup"><span data-stu-id="2879e-109">Method</span></span>       | <span data-ttu-id="2879e-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2879e-110">Return Type</span></span> | <span data-ttu-id="2879e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2879e-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2879e-112">Listar accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="2879e-112">List accessPackageAssignmentRequests</span></span>](../api/accesspackageassignmentrequest-list.md) | <span data-ttu-id="2879e-113">[coleção accessPackageAssignmentRequest](accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="2879e-113">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) collection</span></span> | <span data-ttu-id="2879e-114">Recupere uma lista de objetos accesspackageassignmentrequest.</span><span class="sxs-lookup"><span data-stu-id="2879e-114">Retrieve a list of accesspackageassignmentrequest objects.</span></span> |
| [<span data-ttu-id="2879e-115">Criar accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="2879e-115">Create accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-post.md) | [<span data-ttu-id="2879e-116">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="2879e-116">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="2879e-117">Crie um novo accessPackageAssignmentRequest.</span><span class="sxs-lookup"><span data-stu-id="2879e-117">Create a new accessPackageAssignmentRequest.</span></span> |
| [<span data-ttu-id="2879e-118">Obter accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="2879e-118">Get accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-get.md) | [<span data-ttu-id="2879e-119">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="2879e-119">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="2879e-120">Leia propriedades e relações de um objeto accessPackageAssignmentRequest.</span><span class="sxs-lookup"><span data-stu-id="2879e-120">Read properties and relationships of an accessPackageAssignmentRequest object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2879e-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2879e-121">Properties</span></span>

| <span data-ttu-id="2879e-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2879e-122">Property</span></span>     | <span data-ttu-id="2879e-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="2879e-123">Type</span></span>        | <span data-ttu-id="2879e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="2879e-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2879e-125">completedDate</span><span class="sxs-lookup"><span data-stu-id="2879e-125">completedDate</span></span>|<span data-ttu-id="2879e-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2879e-126">DateTimeOffset</span></span>|<span data-ttu-id="2879e-127">A data do final do processamento, bem-sucedida ou falha, de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="2879e-127">The date of the end of processing, either successful or failure, of a request.</span></span> <span data-ttu-id="2879e-128">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2879e-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2879e-129">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="2879e-129">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="2879e-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2879e-130">Read-only.</span></span>|
|<span data-ttu-id="2879e-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2879e-131">createdDateTime</span></span>|<span data-ttu-id="2879e-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2879e-132">DateTimeOffset</span></span>|<span data-ttu-id="2879e-133">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2879e-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2879e-134">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="2879e-134">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="2879e-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2879e-135">Read-only.</span></span>|
|<span data-ttu-id="2879e-136">id</span><span class="sxs-lookup"><span data-stu-id="2879e-136">id</span></span>|<span data-ttu-id="2879e-137">String</span><span class="sxs-lookup"><span data-stu-id="2879e-137">String</span></span>| <span data-ttu-id="2879e-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2879e-138">Read-only.</span></span>|
|<span data-ttu-id="2879e-139">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="2879e-139">isValidationOnly</span></span>|<span data-ttu-id="2879e-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="2879e-140">Boolean</span></span>|<span data-ttu-id="2879e-141">True se a solicitação não for processada para atribuição.</span><span class="sxs-lookup"><span data-stu-id="2879e-141">True if the request is not to be processed for assignment.</span></span>|
|<span data-ttu-id="2879e-142">justification</span><span class="sxs-lookup"><span data-stu-id="2879e-142">justification</span></span>|<span data-ttu-id="2879e-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2879e-143">String</span></span>|<span data-ttu-id="2879e-144">A justificativa fornecida pelo solicitante.</span><span class="sxs-lookup"><span data-stu-id="2879e-144">The requestor's supplied justification.</span></span>|
|<span data-ttu-id="2879e-145">requestState</span><span class="sxs-lookup"><span data-stu-id="2879e-145">requestState</span></span>|<span data-ttu-id="2879e-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2879e-146">String</span></span>|<span data-ttu-id="2879e-147">Um dos `PendingApproval` , , , , , ou `Canceled`  `Denied` `Delivering` `Delivered` `PartiallyDelivered` `Submitted` `Scheduled` .</span><span class="sxs-lookup"><span data-stu-id="2879e-147">One of `PendingApproval`, `Canceled`,  `Denied`, `Delivering`, `Delivered`, `PartiallyDelivered`, `Submitted` or `Scheduled`.</span></span> <span data-ttu-id="2879e-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2879e-148">Read-only.</span></span>|
|<span data-ttu-id="2879e-149">requestStatus</span><span class="sxs-lookup"><span data-stu-id="2879e-149">requestStatus</span></span>|<span data-ttu-id="2879e-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2879e-150">String</span></span>|<span data-ttu-id="2879e-151">Mais informações sobre o status do processamento de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2879e-151">More information on the request processing status.</span></span> <span data-ttu-id="2879e-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2879e-152">Read-only.</span></span>|
|<span data-ttu-id="2879e-153">requestType</span><span class="sxs-lookup"><span data-stu-id="2879e-153">requestType</span></span>|<span data-ttu-id="2879e-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2879e-154">String</span></span>|<span data-ttu-id="2879e-155">Um dos `UserAdd` , `UserRemove` , ou `AdminAdd` `AdminRemove` `SystemRemove` .</span><span class="sxs-lookup"><span data-stu-id="2879e-155">One of `UserAdd`, `UserRemove`, `AdminAdd`, `AdminRemove` or `SystemRemove`.</span></span> <span data-ttu-id="2879e-156">Uma solicitação do próprio usuário teria requestType de `UserAdd` ou `UserRemove` .</span><span class="sxs-lookup"><span data-stu-id="2879e-156">A request from the user themselves would have requestType of `UserAdd` or `UserRemove`.</span></span> <span data-ttu-id="2879e-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2879e-157">Read-only.</span></span>|
|<span data-ttu-id="2879e-158">Cronograma</span><span class="sxs-lookup"><span data-stu-id="2879e-158">schedule</span></span>|[<span data-ttu-id="2879e-159">requestSchedule</span><span class="sxs-lookup"><span data-stu-id="2879e-159">requestSchedule</span></span>](requestschedule.md)| <span data-ttu-id="2879e-160">O intervalo de datas que o acesso deve ser atribuído ao solicitante.</span><span class="sxs-lookup"><span data-stu-id="2879e-160">The range of dates that access is to be assigned to the requestor.</span></span> <span data-ttu-id="2879e-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2879e-161">Read-only.</span></span>|
|<span data-ttu-id="2879e-162">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="2879e-162">accessPackageAssignment</span></span>|[<span data-ttu-id="2879e-163">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="2879e-163">accessPackageAssignment</span></span>](accesspackageassignment.md)| <span data-ttu-id="2879e-164">Para um requestType de `UserAdd` ou , esta é uma `AdminAdd` atribuição de pacote de acesso solicitada a ser criada.</span><span class="sxs-lookup"><span data-stu-id="2879e-164">For a requestType of `UserAdd` or `AdminAdd`, this is an access package assignment requested to be created.</span></span>  <span data-ttu-id="2879e-165">Para um requestType `UserRemove` de , ou , isso tem a propriedade de uma `AdminRemove` `SystemRemove` `id` atribuição existente a ser removida.</span><span class="sxs-lookup"><span data-stu-id="2879e-165">For a requestType of `UserRemove`, `AdminRemove` or `SystemRemove`, this has the `id` property of an existing assignment to be removed.</span></span>|
|<span data-ttu-id="2879e-166">answers</span><span class="sxs-lookup"><span data-stu-id="2879e-166">answers</span></span>|<span data-ttu-id="2879e-167">[Coleção accessPackageAnswer](accesspackageanswer.md)</span><span class="sxs-lookup"><span data-stu-id="2879e-167">[accessPackageAnswer](accesspackageanswer.md) collection</span></span>|<span data-ttu-id="2879e-168">Respostas fornecidas pelo solicitante para [acessarPackageQuestions solicitadas](accesspackagequestion.md) no momento da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2879e-168">Answers provided by the requestor to [accessPackageQuestions](accesspackagequestion.md) asked of them at the time of request.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2879e-169">Relações</span><span class="sxs-lookup"><span data-stu-id="2879e-169">Relationships</span></span>

| <span data-ttu-id="2879e-170">Relação</span><span class="sxs-lookup"><span data-stu-id="2879e-170">Relationship</span></span> | <span data-ttu-id="2879e-171">Tipo</span><span class="sxs-lookup"><span data-stu-id="2879e-171">Type</span></span>        | <span data-ttu-id="2879e-172">Descrição</span><span class="sxs-lookup"><span data-stu-id="2879e-172">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2879e-173">requestor</span><span class="sxs-lookup"><span data-stu-id="2879e-173">requestor</span></span>|[<span data-ttu-id="2879e-174">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="2879e-174">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="2879e-175">O assunto que solicitou ou, se uma atribuição direta, foi atribuído.</span><span class="sxs-lookup"><span data-stu-id="2879e-175">The subject who requested or, if a direct assignment, was assigned.</span></span> <span data-ttu-id="2879e-176">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2879e-176">Read-only.</span></span> <span data-ttu-id="2879e-177">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2879e-177">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2879e-178">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2879e-178">JSON representation</span></span>

<span data-ttu-id="2879e-179">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2879e-179">The following is a JSON representation of the resource.</span></span>

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

