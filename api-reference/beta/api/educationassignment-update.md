---
title: Atualizar educationassignment
description: Atualize o objeto assignment. Somente os professores da classe podem fazer isso. Observe que você não pode usar uma solicitação PATCH para alterar o status de uma atribuição. Use a ação publicar para alterar o status da atribuição.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 39f9f1a56fca07078b4be74447de563b7b7f8d31
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2021
ms.locfileid: "52780768"
---
# <a name="update-educationassignment"></a><span data-ttu-id="a26fb-106">Atualizar educationassignment</span><span class="sxs-lookup"><span data-stu-id="a26fb-106">Update educationassignment</span></span>

<span data-ttu-id="a26fb-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a26fb-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a26fb-108">Atualize o objeto assignment.</span><span class="sxs-lookup"><span data-stu-id="a26fb-108">Update the assignment object.</span></span> <span data-ttu-id="a26fb-109">Somente os professores da classe podem fazer isso.</span><span class="sxs-lookup"><span data-stu-id="a26fb-109">Only teachers in the class can do this.</span></span> <span data-ttu-id="a26fb-110">Observe que você não pode usar uma solicitação PATCH para alterar o status de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="a26fb-110">Note that you can't use a PATCH request to change the status of an assignment.</span></span> <span data-ttu-id="a26fb-111">Use a [ação publicar](../api/educationassignment-publish.md) para alterar o status da atribuição.</span><span class="sxs-lookup"><span data-stu-id="a26fb-111">Use the [publish](../api/educationassignment-publish.md) action to change the assignment status.</span></span>

## <a name="permissions"></a><span data-ttu-id="a26fb-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="a26fb-112">Permissions</span></span>
<span data-ttu-id="a26fb-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a26fb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a26fb-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a26fb-115">Permission type</span></span>      | <span data-ttu-id="a26fb-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a26fb-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a26fb-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a26fb-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="a26fb-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a26fb-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="a26fb-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a26fb-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a26fb-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a26fb-120">Not supported.</span></span>  |
|<span data-ttu-id="a26fb-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a26fb-121">Application</span></span> | <span data-ttu-id="a26fb-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a26fb-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a26fb-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a26fb-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a26fb-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a26fb-124">Request headers</span></span>
| <span data-ttu-id="a26fb-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a26fb-125">Header</span></span>       | <span data-ttu-id="a26fb-126">Valor</span><span class="sxs-lookup"><span data-stu-id="a26fb-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a26fb-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="a26fb-127">Authorization</span></span>  | <span data-ttu-id="a26fb-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a26fb-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a26fb-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a26fb-130">Content-Type</span></span>  | <span data-ttu-id="a26fb-131">application/json</span><span class="sxs-lookup"><span data-stu-id="a26fb-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a26fb-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a26fb-132">Request body</span></span>
<span data-ttu-id="a26fb-133">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="a26fb-133">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a26fb-134">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="a26fb-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a26fb-135">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="a26fb-135">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a26fb-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a26fb-136">Property</span></span>     | <span data-ttu-id="a26fb-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="a26fb-137">Type</span></span>   |<span data-ttu-id="a26fb-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="a26fb-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a26fb-139">addedStudentAction</span><span class="sxs-lookup"><span data-stu-id="a26fb-139">addedStudentAction</span></span>|<span data-ttu-id="a26fb-140">String</span><span class="sxs-lookup"><span data-stu-id="a26fb-140">String</span></span>| <span data-ttu-id="a26fb-141">Controla o comportamento dos alunos que são adicionados após a publicação da atribuição.</span><span class="sxs-lookup"><span data-stu-id="a26fb-141">Controls the behavior for students who are added after the assignment is published.</span></span>|
|<span data-ttu-id="a26fb-142">allowLateSubmissions</span><span class="sxs-lookup"><span data-stu-id="a26fb-142">allowLateSubmissions</span></span>|<span data-ttu-id="a26fb-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="a26fb-143">Boolean</span></span>| <span data-ttu-id="a26fb-144">Se os envios podem ser enviados após a data de vencimento.</span><span class="sxs-lookup"><span data-stu-id="a26fb-144">Whether submissions can be submitted after the due date.</span></span>|
|<span data-ttu-id="a26fb-145">allowStudentsToAddResourcesToSubmission</span><span class="sxs-lookup"><span data-stu-id="a26fb-145">allowStudentsToAddResourcesToSubmission</span></span>|<span data-ttu-id="a26fb-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="a26fb-146">Boolean</span></span>| <span data-ttu-id="a26fb-147">Se um aluno pode adicionar recursos a um envio.</span><span class="sxs-lookup"><span data-stu-id="a26fb-147">Whether a student can add resources to a submission.</span></span> <span data-ttu-id="a26fb-148">Indica se os únicos itens no envio vieram da lista de recursos de atribuição.</span><span class="sxs-lookup"><span data-stu-id="a26fb-148">Indicated whether the only items on the submission came from the assignment resource list.</span></span> |
|<span data-ttu-id="a26fb-149">assignDateTime</span><span class="sxs-lookup"><span data-stu-id="a26fb-149">assignDateTime</span></span>|<span data-ttu-id="a26fb-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a26fb-150">DateTimeOffset</span></span>| <span data-ttu-id="a26fb-151">Data em que a atribuição deve ser publicada para os alunos.</span><span class="sxs-lookup"><span data-stu-id="a26fb-151">Date the assignment should be published to students.</span></span> |
|<span data-ttu-id="a26fb-152">assignTo</span><span class="sxs-lookup"><span data-stu-id="a26fb-152">assignTo</span></span>|<span data-ttu-id="a26fb-153">educationAssignmentRecipient</span><span class="sxs-lookup"><span data-stu-id="a26fb-153">educationAssignmentRecipient</span></span>| <span data-ttu-id="a26fb-154">Alunos que receberão a atribuição.</span><span class="sxs-lookup"><span data-stu-id="a26fb-154">Students who get the assignment.</span></span>|
|<span data-ttu-id="a26fb-155">closeDateTime</span><span class="sxs-lookup"><span data-stu-id="a26fb-155">closeDateTime</span></span>|<span data-ttu-id="a26fb-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a26fb-156">DateTimeOffset</span></span>| <span data-ttu-id="a26fb-157">Data em que a atribuição será fechada para envios.</span><span class="sxs-lookup"><span data-stu-id="a26fb-157">Date when the assignment will be closed for submissions.</span></span> <span data-ttu-id="a26fb-158">Este é um campo opcional que pode ser nulo se a atribuição não permitirLateSubmissions ou closeDateTime for igual ao dueDateTime, mas se especificado, ele deve ser maior ou igual ao dueDateTime.</span><span class="sxs-lookup"><span data-stu-id="a26fb-158">This is an optional field that can be null if the assignment does not allowLateSubmissions or the closeDateTime is the same as the dueDateTime but if specified, it must be greater than or equal to the dueDateTime.</span></span>|
|<span data-ttu-id="a26fb-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a26fb-159">displayName</span></span>|<span data-ttu-id="a26fb-160">String</span><span class="sxs-lookup"><span data-stu-id="a26fb-160">String</span></span>| <span data-ttu-id="a26fb-161">Nome da atribuição.</span><span class="sxs-lookup"><span data-stu-id="a26fb-161">Name of assignment.</span></span> |
|<span data-ttu-id="a26fb-162">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="a26fb-162">dueDateTime</span></span>|<span data-ttu-id="a26fb-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a26fb-163">DateTimeOffset</span></span>| <span data-ttu-id="a26fb-164">A atribuição de data é devido.</span><span class="sxs-lookup"><span data-stu-id="a26fb-164">Date assignment is due.</span></span> |
|<span data-ttu-id="a26fb-165">grading</span><span class="sxs-lookup"><span data-stu-id="a26fb-165">grading</span></span>|<span data-ttu-id="a26fb-166">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="a26fb-166">educationAssignmentGradeType</span></span>| <span data-ttu-id="a26fb-167">Como a atribuição será gradeada.</span><span class="sxs-lookup"><span data-stu-id="a26fb-167">How the assignment will be graded.</span></span>|
|<span data-ttu-id="a26fb-168">instructions</span><span class="sxs-lookup"><span data-stu-id="a26fb-168">instructions</span></span>|<span data-ttu-id="a26fb-169">itemBody</span><span class="sxs-lookup"><span data-stu-id="a26fb-169">itemBody</span></span>| <span data-ttu-id="a26fb-170">Instruções a serem fornecidas aos alunos juntamente com a atribuição.</span><span class="sxs-lookup"><span data-stu-id="a26fb-170">Instructions to be given to the students along with the assignment.</span></span> |
|<span data-ttu-id="a26fb-171">notificationChannelUrl</span><span class="sxs-lookup"><span data-stu-id="a26fb-171">notificationChannelUrl</span></span>|<span data-ttu-id="a26fb-172">String</span><span class="sxs-lookup"><span data-stu-id="a26fb-172">String</span></span>| <span data-ttu-id="a26fb-173">Canal para postar notificação de publicação de atribuição.</span><span class="sxs-lookup"><span data-stu-id="a26fb-173">Channel to post assignment publish notification.</span></span> <span data-ttu-id="a26fb-174">A atualização da URL do canal não é permitida após a publicação da atribuição e só é permitida quando o valor **assignTo** é [educationAssignmentClassRecipient](../resources/educationassignmentclassrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="a26fb-174">Updating the channel URL is not allowed after the assignment has been published and is only allowed when the **assignTo** value is [educationAssignmentClassRecipient](../resources/educationassignmentclassrecipient.md).</span></span>|

## <a name="response"></a><span data-ttu-id="a26fb-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="a26fb-175">Response</span></span>
<span data-ttu-id="a26fb-176">Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [educationAssignment](../resources/educationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a26fb-176">If successful, this method returns a `200 OK` response code and an updated [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a26fb-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a26fb-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="a26fb-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a26fb-178">Request</span></span>
<span data-ttu-id="a26fb-179">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a26fb-179">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a26fb-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="a26fb-180">HTTP</span></span>](#tab/http)
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
  "dueDateTime": "2014-02-01T00:00:00Z",
  "addedStudentAction": "none",
  "addToCalendarAction": "studentsAndPublisher",
}
```
# <a name="c"></a>[<span data-ttu-id="a26fb-181">C#</span><span class="sxs-lookup"><span data-stu-id="a26fb-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a26fb-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a26fb-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a26fb-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a26fb-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a26fb-184">Java</span><span class="sxs-lookup"><span data-stu-id="a26fb-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="a26fb-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="a26fb-185">Response</span></span>
<span data-ttu-id="a26fb-186">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a26fb-186">The following is an example of the response.</span></span> 

><span data-ttu-id="a26fb-187">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a26fb-187">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "addToCalendarAction": "studentsAndPublisher",
  "dueDateTime": "2014-02-01T00:00:00Z",
  "assignDateTime": "2014-01-01T00:00:00Z",
  "assignedDateTime": "2014-01-01T00:00:00Z",
  "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!0sGAoOieeE6iSj1WXCV-nYYTuh2luKRDvUVGQBLOmvYpRzc5ARnCRorRht6P3MhU/items/01N74NOEZL7P3VK22SQFDKBZ3PHVPKDVAQ",
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


