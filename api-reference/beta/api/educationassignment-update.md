---
title: Atualizar educationassignment
description: Atualize o objeto assignment. Somente os professores da turma podem fazer isso. Observe que você não pode usar uma solicitação PATCH para alterar o status de uma atribuição. Use a ação publicar para alterar o status da atribuição.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e8efe5064196e179fade55704d4ea28a349fb801
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966486"
---
# <a name="update-educationassignment"></a><span data-ttu-id="44038-106">Atualizar educationassignment</span><span class="sxs-lookup"><span data-stu-id="44038-106">Update educationassignment</span></span>

<span data-ttu-id="44038-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44038-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44038-108">Atualize o objeto assignment.</span><span class="sxs-lookup"><span data-stu-id="44038-108">Update the assignment object.</span></span> <span data-ttu-id="44038-109">Somente os professores da turma podem fazer isso.</span><span class="sxs-lookup"><span data-stu-id="44038-109">Only teachers in the class can do this.</span></span> <span data-ttu-id="44038-110">Observe que você não pode usar uma solicitação PATCH para alterar o status de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="44038-110">Note that you can't use a PATCH request to change the status of an assignment.</span></span> <span data-ttu-id="44038-111">Use a ação [publicar](../api/educationassignment-publish.md) para alterar o status da atribuição.</span><span class="sxs-lookup"><span data-stu-id="44038-111">Use the [publish](../api/educationassignment-publish.md) action to change the assignment status.</span></span>

## <a name="permissions"></a><span data-ttu-id="44038-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="44038-112">Permissions</span></span>
<span data-ttu-id="44038-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44038-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44038-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44038-115">Permission type</span></span>      | <span data-ttu-id="44038-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="44038-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44038-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44038-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="44038-118">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44038-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="44038-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44038-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="44038-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44038-120">Not supported.</span></span>  |
|<span data-ttu-id="44038-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="44038-121">Application</span></span> | <span data-ttu-id="44038-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44038-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="44038-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44038-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="44038-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44038-124">Request headers</span></span>
| <span data-ttu-id="44038-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="44038-125">Header</span></span>       | <span data-ttu-id="44038-126">Valor</span><span class="sxs-lookup"><span data-stu-id="44038-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="44038-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="44038-127">Authorization</span></span>  | <span data-ttu-id="44038-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44038-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="44038-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="44038-130">Content-Type</span></span>  | <span data-ttu-id="44038-131">application/json</span><span class="sxs-lookup"><span data-stu-id="44038-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="44038-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="44038-132">Request body</span></span>
<span data-ttu-id="44038-133">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="44038-133">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="44038-134">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="44038-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="44038-135">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="44038-135">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="44038-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44038-136">Property</span></span>     | <span data-ttu-id="44038-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="44038-137">Type</span></span>   |<span data-ttu-id="44038-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="44038-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44038-139">allowLateSubmissions</span><span class="sxs-lookup"><span data-stu-id="44038-139">allowLateSubmissions</span></span>|<span data-ttu-id="44038-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="44038-140">Boolean</span></span>| <span data-ttu-id="44038-141">Se os envios podem ser enviados após a data de conclusão.</span><span class="sxs-lookup"><span data-stu-id="44038-141">Whether submissions can be submitted after the due date.</span></span>|
|<span data-ttu-id="44038-142">allowStudentsToAddResourcesToSubmission</span><span class="sxs-lookup"><span data-stu-id="44038-142">allowStudentsToAddResourcesToSubmission</span></span>|<span data-ttu-id="44038-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="44038-143">Boolean</span></span>| <span data-ttu-id="44038-144">Se um aluno pode adicionar recursos a um envio.</span><span class="sxs-lookup"><span data-stu-id="44038-144">Whether a student can add resources to a submission.</span></span> <span data-ttu-id="44038-145">Indica se os únicos itens no envio vieram da lista de recursos de atribuição.</span><span class="sxs-lookup"><span data-stu-id="44038-145">Indicated whether the only items on the submission came from the assignment resource list.</span></span> |
|<span data-ttu-id="44038-146">assignDateTime</span><span class="sxs-lookup"><span data-stu-id="44038-146">assignDateTime</span></span>|<span data-ttu-id="44038-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44038-147">DateTimeOffset</span></span>| <span data-ttu-id="44038-148">Data em que a atribuição deve ser publicada para os alunos.</span><span class="sxs-lookup"><span data-stu-id="44038-148">Date the assignment should be published to students.</span></span> |
|<span data-ttu-id="44038-149">atribuir</span><span class="sxs-lookup"><span data-stu-id="44038-149">assignTo</span></span>|<span data-ttu-id="44038-150">educationAssignmentRecipient</span><span class="sxs-lookup"><span data-stu-id="44038-150">educationAssignmentRecipient</span></span>| <span data-ttu-id="44038-151">Estudantes que obtêm a atribuição.</span><span class="sxs-lookup"><span data-stu-id="44038-151">Students who get the assignment.</span></span>|
|<span data-ttu-id="44038-152">closeDateTime</span><span class="sxs-lookup"><span data-stu-id="44038-152">closeDateTime</span></span>|<span data-ttu-id="44038-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44038-153">DateTimeOffset</span></span>| <span data-ttu-id="44038-154">Data em que a atribuição será fechada para envios.</span><span class="sxs-lookup"><span data-stu-id="44038-154">Date when the assignment will be closed for submissions.</span></span> <span data-ttu-id="44038-155">Este é um campo opcional que pode ser nulo se a atribuição não allowLateSubmissions ou o closeDateTime for igual ao dueDateTime, mas se especificado, ele deve ser maior ou igual ao dueDateTime.</span><span class="sxs-lookup"><span data-stu-id="44038-155">This is an optional field that can be null if the assignment does not allowLateSubmissions or the closeDateTime is the same as the dueDateTime but if specified, it must be greater than or equal to the dueDateTime.</span></span>|
|<span data-ttu-id="44038-156">displayName</span><span class="sxs-lookup"><span data-stu-id="44038-156">displayName</span></span>|<span data-ttu-id="44038-157">String</span><span class="sxs-lookup"><span data-stu-id="44038-157">String</span></span>| <span data-ttu-id="44038-158">Nome da atribuição.</span><span class="sxs-lookup"><span data-stu-id="44038-158">Name of assignment.</span></span> |
|<span data-ttu-id="44038-159">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="44038-159">dueDateTime</span></span>|<span data-ttu-id="44038-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44038-160">DateTimeOffset</span></span>| <span data-ttu-id="44038-161">A atribuição de data deve ser concluída.</span><span class="sxs-lookup"><span data-stu-id="44038-161">Date assignment is due.</span></span> |
|<span data-ttu-id="44038-162">notas</span><span class="sxs-lookup"><span data-stu-id="44038-162">grading</span></span>|<span data-ttu-id="44038-163">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="44038-163">educationAssignmentGradeType</span></span>| <span data-ttu-id="44038-164">Como a atribuição será classificada.</span><span class="sxs-lookup"><span data-stu-id="44038-164">How the assignment will be graded.</span></span>|
|<span data-ttu-id="44038-165">contida</span><span class="sxs-lookup"><span data-stu-id="44038-165">instructions</span></span>|<span data-ttu-id="44038-166">itemBody</span><span class="sxs-lookup"><span data-stu-id="44038-166">itemBody</span></span>| <span data-ttu-id="44038-167">Instruções a serem dadas aos alunos junto com a atribuição.</span><span class="sxs-lookup"><span data-stu-id="44038-167">Instructions to be given to the students along with the assignment.</span></span> |

## <a name="response"></a><span data-ttu-id="44038-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="44038-168">Response</span></span>
<span data-ttu-id="44038-169">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [educationAssignment](../resources/educationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44038-169">If successful, this method returns a `200 OK` response code and an updated [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="44038-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44038-170">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44038-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44038-171">Request</span></span>
<span data-ttu-id="44038-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="44038-172">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="44038-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="44038-173">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="44038-174">C#</span><span class="sxs-lookup"><span data-stu-id="44038-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44038-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44038-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44038-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44038-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="44038-177">Java</span><span class="sxs-lookup"><span data-stu-id="44038-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="44038-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="44038-178">Response</span></span>
<span data-ttu-id="44038-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="44038-179">The following is an example of the response.</span></span> 

><span data-ttu-id="44038-180">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="44038-180">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="44038-181">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="44038-181">All of the properties will be returned from an actual call.</span></span>

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


