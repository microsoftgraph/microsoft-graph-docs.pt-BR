---
title: Atualizar educationassignment
description: Atualize o objeto assignment. Somente os professores da turma podem fazer isso. Observe que você não pode usar uma solicitação PATCH para alterar o status de uma atribuição. Use a ação publicar para alterar o status da atribuição.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d0f0f965eece0d7998769e72afe58b56c7acd159
ms.sourcegitcommit: 86d427ac670ebc3fdcf8e06541218bb74d39279d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2020
ms.locfileid: "49675996"
---
# <a name="update-educationassignment"></a><span data-ttu-id="da4da-106">Atualizar educationassignment</span><span class="sxs-lookup"><span data-stu-id="da4da-106">Update educationassignment</span></span>

<span data-ttu-id="da4da-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da4da-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da4da-108">Atualize o objeto assignment.</span><span class="sxs-lookup"><span data-stu-id="da4da-108">Update the assignment object.</span></span> <span data-ttu-id="da4da-109">Somente os professores da turma podem fazer isso.</span><span class="sxs-lookup"><span data-stu-id="da4da-109">Only teachers in the class can do this.</span></span> <span data-ttu-id="da4da-110">Observe que você não pode usar uma solicitação PATCH para alterar o status de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="da4da-110">Note that you can't use a PATCH request to change the status of an assignment.</span></span> <span data-ttu-id="da4da-111">Use a ação [publicar](../api/educationassignment-publish.md) para alterar o status da atribuição.</span><span class="sxs-lookup"><span data-stu-id="da4da-111">Use the [publish](../api/educationassignment-publish.md) action to change the assignment status.</span></span>

## <a name="permissions"></a><span data-ttu-id="da4da-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="da4da-112">Permissions</span></span>
<span data-ttu-id="da4da-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da4da-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da4da-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da4da-115">Permission type</span></span>      | <span data-ttu-id="da4da-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da4da-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da4da-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da4da-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="da4da-118">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da4da-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="da4da-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da4da-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="da4da-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da4da-120">Not supported.</span></span>  |
|<span data-ttu-id="da4da-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da4da-121">Application</span></span> | <span data-ttu-id="da4da-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da4da-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="da4da-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da4da-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="da4da-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da4da-124">Request headers</span></span>
| <span data-ttu-id="da4da-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="da4da-125">Header</span></span>       | <span data-ttu-id="da4da-126">Valor</span><span class="sxs-lookup"><span data-stu-id="da4da-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="da4da-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="da4da-127">Authorization</span></span>  | <span data-ttu-id="da4da-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da4da-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="da4da-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="da4da-130">Content-Type</span></span>  | <span data-ttu-id="da4da-131">application/json</span><span class="sxs-lookup"><span data-stu-id="da4da-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="da4da-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da4da-132">Request body</span></span>
<span data-ttu-id="da4da-133">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="da4da-133">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="da4da-134">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="da4da-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="da4da-135">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="da4da-135">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="da4da-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da4da-136">Property</span></span>     | <span data-ttu-id="da4da-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="da4da-137">Type</span></span>   |<span data-ttu-id="da4da-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="da4da-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da4da-139">addedStudentAction</span><span class="sxs-lookup"><span data-stu-id="da4da-139">addedStudentAction</span></span>|<span data-ttu-id="da4da-140">String</span><span class="sxs-lookup"><span data-stu-id="da4da-140">String</span></span>| <span data-ttu-id="da4da-141">Controla o comportamento para estudantes que são adicionados após a atribuição ser publicada.</span><span class="sxs-lookup"><span data-stu-id="da4da-141">Controls the behavior for students who are added after the assignment is published.</span></span>|
|<span data-ttu-id="da4da-142">allowLateSubmissions</span><span class="sxs-lookup"><span data-stu-id="da4da-142">allowLateSubmissions</span></span>|<span data-ttu-id="da4da-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="da4da-143">Boolean</span></span>| <span data-ttu-id="da4da-144">Se os envios podem ser enviados após a data de conclusão.</span><span class="sxs-lookup"><span data-stu-id="da4da-144">Whether submissions can be submitted after the due date.</span></span>|
|<span data-ttu-id="da4da-145">allowStudentsToAddResourcesToSubmission</span><span class="sxs-lookup"><span data-stu-id="da4da-145">allowStudentsToAddResourcesToSubmission</span></span>|<span data-ttu-id="da4da-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="da4da-146">Boolean</span></span>| <span data-ttu-id="da4da-147">Se um aluno pode adicionar recursos a um envio.</span><span class="sxs-lookup"><span data-stu-id="da4da-147">Whether a student can add resources to a submission.</span></span> <span data-ttu-id="da4da-148">Indica se os únicos itens no envio vieram da lista de recursos de atribuição.</span><span class="sxs-lookup"><span data-stu-id="da4da-148">Indicated whether the only items on the submission came from the assignment resource list.</span></span> |
|<span data-ttu-id="da4da-149">assignDateTime</span><span class="sxs-lookup"><span data-stu-id="da4da-149">assignDateTime</span></span>|<span data-ttu-id="da4da-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da4da-150">DateTimeOffset</span></span>| <span data-ttu-id="da4da-151">Data em que a atribuição deve ser publicada para os alunos.</span><span class="sxs-lookup"><span data-stu-id="da4da-151">Date the assignment should be published to students.</span></span> |
|<span data-ttu-id="da4da-152">atribuir</span><span class="sxs-lookup"><span data-stu-id="da4da-152">assignTo</span></span>|<span data-ttu-id="da4da-153">educationAssignmentRecipient</span><span class="sxs-lookup"><span data-stu-id="da4da-153">educationAssignmentRecipient</span></span>| <span data-ttu-id="da4da-154">Estudantes que obtêm a atribuição.</span><span class="sxs-lookup"><span data-stu-id="da4da-154">Students who get the assignment.</span></span>|
|<span data-ttu-id="da4da-155">closeDateTime</span><span class="sxs-lookup"><span data-stu-id="da4da-155">closeDateTime</span></span>|<span data-ttu-id="da4da-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da4da-156">DateTimeOffset</span></span>| <span data-ttu-id="da4da-157">Data em que a atribuição será fechada para envios.</span><span class="sxs-lookup"><span data-stu-id="da4da-157">Date when the assignment will be closed for submissions.</span></span> <span data-ttu-id="da4da-158">Este é um campo opcional que pode ser nulo se a atribuição não allowLateSubmissions ou o closeDateTime for igual ao dueDateTime, mas se especificado, ele deve ser maior ou igual ao dueDateTime.</span><span class="sxs-lookup"><span data-stu-id="da4da-158">This is an optional field that can be null if the assignment does not allowLateSubmissions or the closeDateTime is the same as the dueDateTime but if specified, it must be greater than or equal to the dueDateTime.</span></span>|
|<span data-ttu-id="da4da-159">displayName</span><span class="sxs-lookup"><span data-stu-id="da4da-159">displayName</span></span>|<span data-ttu-id="da4da-160">String</span><span class="sxs-lookup"><span data-stu-id="da4da-160">String</span></span>| <span data-ttu-id="da4da-161">Nome da atribuição.</span><span class="sxs-lookup"><span data-stu-id="da4da-161">Name of assignment.</span></span> |
|<span data-ttu-id="da4da-162">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="da4da-162">dueDateTime</span></span>|<span data-ttu-id="da4da-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da4da-163">DateTimeOffset</span></span>| <span data-ttu-id="da4da-164">A atribuição de data deve ser concluída.</span><span class="sxs-lookup"><span data-stu-id="da4da-164">Date assignment is due.</span></span> |
|<span data-ttu-id="da4da-165">notas</span><span class="sxs-lookup"><span data-stu-id="da4da-165">grading</span></span>|<span data-ttu-id="da4da-166">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="da4da-166">educationAssignmentGradeType</span></span>| <span data-ttu-id="da4da-167">Como a atribuição será classificada.</span><span class="sxs-lookup"><span data-stu-id="da4da-167">How the assignment will be graded.</span></span>|
|<span data-ttu-id="da4da-168">contida</span><span class="sxs-lookup"><span data-stu-id="da4da-168">instructions</span></span>|<span data-ttu-id="da4da-169">itemBody</span><span class="sxs-lookup"><span data-stu-id="da4da-169">itemBody</span></span>| <span data-ttu-id="da4da-170">Instruções a serem dadas aos alunos junto com a atribuição.</span><span class="sxs-lookup"><span data-stu-id="da4da-170">Instructions to be given to the students along with the assignment.</span></span> |
|<span data-ttu-id="da4da-171">notificationChannelUrl</span><span class="sxs-lookup"><span data-stu-id="da4da-171">notificationChannelUrl</span></span>|<span data-ttu-id="da4da-172">String</span><span class="sxs-lookup"><span data-stu-id="da4da-172">String</span></span>| <span data-ttu-id="da4da-173">Canal para lançar a notificação de publicação de atribuição.</span><span class="sxs-lookup"><span data-stu-id="da4da-173">Channel to post assignment publish notification.</span></span> <span data-ttu-id="da4da-174">A atualização da URL do canal não é permitida após a atribuição ter sido publicada e só é permitida quando o valor **assignTo** é [educationAssignmentClassRecipient](../resources/educationassignmentclassrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="da4da-174">Updating the channel URL is not allowed after the assignment has been published and is only allowed when the **assignTo** value is [educationAssignmentClassRecipient](../resources/educationassignmentclassrecipient.md).</span></span>|

## <a name="response"></a><span data-ttu-id="da4da-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="da4da-175">Response</span></span>
<span data-ttu-id="da4da-176">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [educationAssignment](../resources/educationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da4da-176">If successful, this method returns a `200 OK` response code and an updated [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="da4da-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da4da-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="da4da-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da4da-178">Request</span></span>
<span data-ttu-id="da4da-179">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="da4da-179">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="da4da-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="da4da-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationassignment"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11021/assignments/19002
Content-type: application/json
Content-length: 279

{
  "displayName": "Week 1 reading assignment",
  "instructions": {
    "contentType": "Text",
    "content": "Read chapters 1 through 3"
  },
  "dueDateTime": "2014-02-01T00:00:00Z"
}
```
# <a name="c"></a>[<span data-ttu-id="da4da-181">C#</span><span class="sxs-lookup"><span data-stu-id="da4da-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da4da-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da4da-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da4da-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da4da-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="da4da-184">Java</span><span class="sxs-lookup"><span data-stu-id="da4da-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="da4da-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="da4da-185">Response</span></span>
<span data-ttu-id="da4da-186">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="da4da-186">The following is an example of the response.</span></span> 

><span data-ttu-id="da4da-187">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="da4da-187">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="da4da-188">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da4da-188">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
  "classId": "11021",
  "displayName": "Week 1 reading assignment",
  "instructions": {
    "contentType": "Text",
    "content": "Read chapters 1 through 3"
  },
  "closeDateTime": "2014-02-11T00:00:00Z",
  "dueDateTime": "2014-02-01T00:00:00Z",
  "assignDateTime": "2014-01-01T00:00:00Z",
  "assignedDateTime": "2014-01-01T00:00:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update educationassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


