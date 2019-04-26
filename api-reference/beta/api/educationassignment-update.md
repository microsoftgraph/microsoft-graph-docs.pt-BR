---
title: Atualizar educationassignment
description: Atualize o objeto assignment. Somente os professores da turma podem fazer isso. Observe que você não pode usar uma solicitação PATCH para alterar o status de uma atribuição. Use a ação publicar para alterar o status da atribuição.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: c8b6659d0af1ae57829add1f64c19cb954b8413f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325015"
---
# <a name="update-educationassignment"></a><span data-ttu-id="233b0-106">Atualizar educationassignment</span><span class="sxs-lookup"><span data-stu-id="233b0-106">Update educationassignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="233b0-107">Atualize o objeto assignment.</span><span class="sxs-lookup"><span data-stu-id="233b0-107">Update the assignment object.</span></span> <span data-ttu-id="233b0-108">Somente os professores da turma podem fazer isso.</span><span class="sxs-lookup"><span data-stu-id="233b0-108">Only teachers in the class can do this.</span></span> <span data-ttu-id="233b0-109">Observe que você não pode usar uma solicitação PATCH para alterar o status de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="233b0-109">Note that you can't use a PATCH request to change the status of an assignment.</span></span> <span data-ttu-id="233b0-110">Use a ação [publicar](../api/educationassignment-publish.md) para alterar o status da atribuição.</span><span class="sxs-lookup"><span data-stu-id="233b0-110">Use the [publish](../api/educationassignment-publish.md) action to change the assignment status.</span></span>

## <a name="permissions"></a><span data-ttu-id="233b0-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="233b0-111">Permissions</span></span>
<span data-ttu-id="233b0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="233b0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="233b0-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="233b0-114">Permission type</span></span>      | <span data-ttu-id="233b0-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="233b0-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="233b0-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="233b0-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="233b0-117">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="233b0-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="233b0-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="233b0-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="233b0-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="233b0-119">Not supported.</span></span>  |
|<span data-ttu-id="233b0-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="233b0-120">Application</span></span> | <span data-ttu-id="233b0-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="233b0-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="233b0-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="233b0-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="233b0-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="233b0-123">Request headers</span></span>
| <span data-ttu-id="233b0-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="233b0-124">Header</span></span>       | <span data-ttu-id="233b0-125">Valor</span><span class="sxs-lookup"><span data-stu-id="233b0-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="233b0-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="233b0-126">Authorization</span></span>  | <span data-ttu-id="233b0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="233b0-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="233b0-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="233b0-129">Content-Type</span></span>  | <span data-ttu-id="233b0-130">application/json</span><span class="sxs-lookup"><span data-stu-id="233b0-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="233b0-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="233b0-131">Request body</span></span>
<span data-ttu-id="233b0-132">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="233b0-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="233b0-133">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="233b0-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="233b0-134">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="233b0-134">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="233b0-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="233b0-135">Property</span></span>     | <span data-ttu-id="233b0-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="233b0-136">Type</span></span>   |<span data-ttu-id="233b0-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="233b0-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="233b0-138">allowLateSubmissions</span><span class="sxs-lookup"><span data-stu-id="233b0-138">allowLateSubmissions</span></span>|<span data-ttu-id="233b0-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="233b0-139">Boolean</span></span>| <span data-ttu-id="233b0-140">Se os envios podem ser enviados após a data de conclusão.</span><span class="sxs-lookup"><span data-stu-id="233b0-140">Whether submissions can be submitted after the due date.</span></span>|
|<span data-ttu-id="233b0-141">allowStudentsToAddResourcesToSubmission</span><span class="sxs-lookup"><span data-stu-id="233b0-141">allowStudentsToAddResourcesToSubmission</span></span>|<span data-ttu-id="233b0-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="233b0-142">Boolean</span></span>| <span data-ttu-id="233b0-143">Se um aluno pode adicionar recursos a um envio.</span><span class="sxs-lookup"><span data-stu-id="233b0-143">Whether a student can add resources to a submission.</span></span> <span data-ttu-id="233b0-144">Indica se os únicos itens no envio vieram da lista de recursos de atribuição.</span><span class="sxs-lookup"><span data-stu-id="233b0-144">Indicated whether the only items on the submission came from the assignment resource list.</span></span> |
|<span data-ttu-id="233b0-145">assignDateTime</span><span class="sxs-lookup"><span data-stu-id="233b0-145">assignDateTime</span></span>|<span data-ttu-id="233b0-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="233b0-146">DateTimeOffset</span></span>| <span data-ttu-id="233b0-147">Data em que a atribuição deve ser publicada para os alunos.</span><span class="sxs-lookup"><span data-stu-id="233b0-147">Date the assignment should be published to students.</span></span> |
|<span data-ttu-id="233b0-148">atribuir</span><span class="sxs-lookup"><span data-stu-id="233b0-148">assignTo</span></span>|<span data-ttu-id="233b0-149">educationAssignmentRecipient</span><span class="sxs-lookup"><span data-stu-id="233b0-149">educationAssignmentRecipient</span></span>| <span data-ttu-id="233b0-150">Estudantes que obtêm a atribuição.</span><span class="sxs-lookup"><span data-stu-id="233b0-150">Students who get the assignment.</span></span>|
|<span data-ttu-id="233b0-151">displayName</span><span class="sxs-lookup"><span data-stu-id="233b0-151">displayName</span></span>|<span data-ttu-id="233b0-152">String</span><span class="sxs-lookup"><span data-stu-id="233b0-152">String</span></span>| <span data-ttu-id="233b0-153">Nome da atribuição.</span><span class="sxs-lookup"><span data-stu-id="233b0-153">Name of assignment.</span></span> |
|<span data-ttu-id="233b0-154">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="233b0-154">dueDateTime</span></span>|<span data-ttu-id="233b0-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="233b0-155">DateTimeOffset</span></span>| <span data-ttu-id="233b0-156">A atribuição de data deve ser concluída.</span><span class="sxs-lookup"><span data-stu-id="233b0-156">Date assignment is due.</span></span> |
|<span data-ttu-id="233b0-157">notas</span><span class="sxs-lookup"><span data-stu-id="233b0-157">grading</span></span>|<span data-ttu-id="233b0-158">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="233b0-158">educationAssignmentGradeType</span></span>| <span data-ttu-id="233b0-159">Como a atribuição será classificada.</span><span class="sxs-lookup"><span data-stu-id="233b0-159">How the assignment will be graded.</span></span>|
|<span data-ttu-id="233b0-160">contida</span><span class="sxs-lookup"><span data-stu-id="233b0-160">instructions</span></span>|<span data-ttu-id="233b0-161">itemBody</span><span class="sxs-lookup"><span data-stu-id="233b0-161">itemBody</span></span>| <span data-ttu-id="233b0-162">Instruções a serem dadas aos alunos junto com a atribuição.</span><span class="sxs-lookup"><span data-stu-id="233b0-162">Instructions to be given to the students along with the assignment.</span></span> |

## <a name="response"></a><span data-ttu-id="233b0-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="233b0-163">Response</span></span>
<span data-ttu-id="233b0-164">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [educationAssignment](../resources/educationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="233b0-164">If successful, this method returns a `200 OK` response code and an updated [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="233b0-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="233b0-165">Example</span></span>
##### <a name="request"></a><span data-ttu-id="233b0-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="233b0-166">Request</span></span>
<span data-ttu-id="233b0-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="233b0-167">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="233b0-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="233b0-168">Response</span></span>
<span data-ttu-id="233b0-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="233b0-169">The following is an example of the response.</span></span> 

><span data-ttu-id="233b0-170">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="233b0-170">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="233b0-171">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="233b0-171">All of the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->
