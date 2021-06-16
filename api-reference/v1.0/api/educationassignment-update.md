---
title: Atualizar educationassignment
description: Atualizar um objeto educationAssigment.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d5a0015ae6c98e2a8a3355f0602027f15751c21e
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941442"
---
# <a name="update-educationassignment"></a><span data-ttu-id="4af8b-103">Atualizar educationassignment</span><span class="sxs-lookup"><span data-stu-id="4af8b-103">Update educationassignment</span></span>

<span data-ttu-id="4af8b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4af8b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4af8b-105">Atualizar um objeto educationAssigment.</span><span class="sxs-lookup"><span data-stu-id="4af8b-105">Update an educationAssigment object.</span></span> 

<span data-ttu-id="4af8b-106">Somente os professores podem executar essa ação.</span><span class="sxs-lookup"><span data-stu-id="4af8b-106">Only teachers can perform this action.</span></span> 

<span data-ttu-id="4af8b-107">Como alternativa, solicite alterar o status de uma atribuição com a [ação de](../api/educationassignment-publish.md) publicação.</span><span class="sxs-lookup"><span data-stu-id="4af8b-107">Alternatively, request to change the status of an assignment with [publish](../api/educationassignment-publish.md) action.</span></span> <span data-ttu-id="4af8b-108">Não use uma operação PATCH para essa finalidade.</span><span class="sxs-lookup"><span data-stu-id="4af8b-108">Don't use a PATCH operation for this purpose.</span></span>

## <a name="permissions"></a><span data-ttu-id="4af8b-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="4af8b-109">Permissions</span></span>
<span data-ttu-id="4af8b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4af8b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4af8b-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4af8b-112">Permission type</span></span>      | <span data-ttu-id="4af8b-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4af8b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4af8b-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4af8b-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="4af8b-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4af8b-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="4af8b-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4af8b-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4af8b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4af8b-117">Not supported.</span></span>  |
|<span data-ttu-id="4af8b-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4af8b-118">Application</span></span> | <span data-ttu-id="4af8b-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4af8b-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4af8b-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4af8b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454
```
## <a name="request-headers"></a><span data-ttu-id="4af8b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4af8b-121">Request headers</span></span>
| <span data-ttu-id="4af8b-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4af8b-122">Header</span></span>       | <span data-ttu-id="4af8b-123">Valor</span><span class="sxs-lookup"><span data-stu-id="4af8b-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4af8b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4af8b-124">Authorization</span></span>  | <span data-ttu-id="4af8b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4af8b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4af8b-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4af8b-127">Content-Type</span></span>  | <span data-ttu-id="4af8b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4af8b-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4af8b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4af8b-129">Request body</span></span>
<span data-ttu-id="4af8b-130">No corpo da solicitação, fornece apenas os valores dos campos que você deseja atualizar.</span><span class="sxs-lookup"><span data-stu-id="4af8b-130">In the request body, supply only the values of the fields you want to update.</span></span> 

<span data-ttu-id="4af8b-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="4af8b-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4af8b-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="4af8b-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4af8b-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4af8b-133">Property</span></span>     | <span data-ttu-id="4af8b-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="4af8b-134">Type</span></span>   |<span data-ttu-id="4af8b-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="4af8b-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4af8b-136">addedStudentAction</span><span class="sxs-lookup"><span data-stu-id="4af8b-136">addedStudentAction</span></span>|<span data-ttu-id="4af8b-137">String</span><span class="sxs-lookup"><span data-stu-id="4af8b-137">String</span></span>| <span data-ttu-id="4af8b-138">Descreve se a atribuição deve ser distribuída aos alunos que são adicionados após a data de publicação da atribuição.</span><span class="sxs-lookup"><span data-stu-id="4af8b-138">Describes if the assignment should be distributed to students who are added after the assignment publication date.</span></span>|
|<span data-ttu-id="4af8b-139">allowLateSubmissions</span><span class="sxs-lookup"><span data-stu-id="4af8b-139">allowLateSubmissions</span></span>|<span data-ttu-id="4af8b-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="4af8b-140">Boolean</span></span>| <span data-ttu-id="4af8b-141">Se os alunos podem enviar envio após a data de vencimento.</span><span class="sxs-lookup"><span data-stu-id="4af8b-141">Whether students can send submission after the due date.</span></span>|
|<span data-ttu-id="4af8b-142">allowStudentsToAddResourcesToSubmission</span><span class="sxs-lookup"><span data-stu-id="4af8b-142">allowStudentsToAddResourcesToSubmission</span></span>|<span data-ttu-id="4af8b-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="4af8b-143">Boolean</span></span>| <span data-ttu-id="4af8b-144">Se um aluno pode adicionar recursos a um envio ou não.</span><span class="sxs-lookup"><span data-stu-id="4af8b-144">Whether a student can add resources to a submission or not.</span></span> <span data-ttu-id="4af8b-145">Além disso, indica se todos os recursos no envio correspondem à lista de recursos de atribuição.</span><span class="sxs-lookup"><span data-stu-id="4af8b-145">Also, indicates whether all resources in the submission correspond to the assignment resource list.</span></span> |
|<span data-ttu-id="4af8b-146">assignDateTime</span><span class="sxs-lookup"><span data-stu-id="4af8b-146">assignDateTime</span></span>|<span data-ttu-id="4af8b-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4af8b-147">DateTimeOffset</span></span>| <span data-ttu-id="4af8b-148">Indica a data para publicar a atribuição aos alunos.</span><span class="sxs-lookup"><span data-stu-id="4af8b-148">Indicates the date to publish the assignment to students.</span></span> |
|<span data-ttu-id="4af8b-149">assignTo</span><span class="sxs-lookup"><span data-stu-id="4af8b-149">assignTo</span></span>|<span data-ttu-id="4af8b-150">educationAssignmentRecipient</span><span class="sxs-lookup"><span data-stu-id="4af8b-150">educationAssignmentRecipient</span></span>| <span data-ttu-id="4af8b-151">Alunos que receberão a atribuição.</span><span class="sxs-lookup"><span data-stu-id="4af8b-151">Students who get the assignment.</span></span>|
|<span data-ttu-id="4af8b-152">closeDateTime</span><span class="sxs-lookup"><span data-stu-id="4af8b-152">closeDateTime</span></span>|<span data-ttu-id="4af8b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4af8b-153">DateTimeOffset</span></span>| <span data-ttu-id="4af8b-154">Data em que a atribuição será fechada para envios.</span><span class="sxs-lookup"><span data-stu-id="4af8b-154">Date when the assignment will be closed for submissions.</span></span> <span data-ttu-id="4af8b-155">Este é um campo opcional que pode ser nulo se a atribuição não permitirLateSubmissions ou closeDateTime for igual ao dueDateTime, mas se especificado, ele deve ser maior ou igual ao dueDateTime.</span><span class="sxs-lookup"><span data-stu-id="4af8b-155">This is an optional field that can be null if the assignment does not allowLateSubmissions or the closeDateTime is the same as the dueDateTime but if specified, it must be greater than or equal to the dueDateTime.</span></span>|
|<span data-ttu-id="4af8b-156">displayName</span><span class="sxs-lookup"><span data-stu-id="4af8b-156">displayName</span></span>|<span data-ttu-id="4af8b-157">String</span><span class="sxs-lookup"><span data-stu-id="4af8b-157">String</span></span>| <span data-ttu-id="4af8b-158">Nome da atribuição.</span><span class="sxs-lookup"><span data-stu-id="4af8b-158">Name of assignment.</span></span> |
|<span data-ttu-id="4af8b-159">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="4af8b-159">dueDateTime</span></span>|<span data-ttu-id="4af8b-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4af8b-160">DateTimeOffset</span></span>| <span data-ttu-id="4af8b-161">A atribuição de data é devido.</span><span class="sxs-lookup"><span data-stu-id="4af8b-161">Date assignment is due.</span></span> |
|<span data-ttu-id="4af8b-162">grading</span><span class="sxs-lookup"><span data-stu-id="4af8b-162">grading</span></span>|<span data-ttu-id="4af8b-163">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="4af8b-163">educationAssignmentGradeType</span></span>| <span data-ttu-id="4af8b-164">Como a atribuição será gradeada.</span><span class="sxs-lookup"><span data-stu-id="4af8b-164">How the assignment will be graded.</span></span>|
|<span data-ttu-id="4af8b-165">instructions</span><span class="sxs-lookup"><span data-stu-id="4af8b-165">instructions</span></span>|<span data-ttu-id="4af8b-166">itemBody</span><span class="sxs-lookup"><span data-stu-id="4af8b-166">itemBody</span></span>| <span data-ttu-id="4af8b-167">Instruções a serem fornecidas aos alunos juntamente com a atribuição.</span><span class="sxs-lookup"><span data-stu-id="4af8b-167">Instructions to be given to the students along with the assignment.</span></span> |
|<span data-ttu-id="4af8b-168">notificationChannelUrl</span><span class="sxs-lookup"><span data-stu-id="4af8b-168">notificationChannelUrl</span></span>|<span data-ttu-id="4af8b-169">String</span><span class="sxs-lookup"><span data-stu-id="4af8b-169">String</span></span>| <span data-ttu-id="4af8b-170">O canal para comunicar notificações relacionadas à atribuição.</span><span class="sxs-lookup"><span data-stu-id="4af8b-170">The channel to communicate notifications related to the assignment.</span></span> <span data-ttu-id="4af8b-171">Para alterar a URL, de definir `assignTo` o valor [como educationAssignmentClassRecipient](../resources/educationassignmentclassrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="4af8b-171">To change the URL, set the `assignTo` value to [educationAssignmentClassRecipient](../resources/educationassignmentclassrecipient.md).</span></span> <span data-ttu-id="4af8b-172">A URL do canal não pode ser mudada após a publicação da atribuição.</span><span class="sxs-lookup"><span data-stu-id="4af8b-172">The channel URL can't change after the publication of the assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="4af8b-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="4af8b-173">Response</span></span>
<span data-ttu-id="4af8b-174">Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [educationAssignment](../resources/educationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4af8b-174">If successful, this method returns a `200 OK` response code and an updated [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4af8b-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4af8b-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="4af8b-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4af8b-176">Request</span></span>
<span data-ttu-id="4af8b-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4af8b-177">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["ad8afb28-c138-4ad7-b7f5-a6986c2655a8"],
  "name": "update_educationassignment"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8
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

### <a name="response"></a><span data-ttu-id="4af8b-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="4af8b-178">Response</span></span>
<span data-ttu-id="4af8b-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4af8b-179">The following is an example of the response.</span></span> 

><span data-ttu-id="4af8b-180">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4af8b-180">**Note:** The response object shown here might be shortened for readability.</span></span>

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


