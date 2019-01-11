---
title: Atualizar educationassignment
description: Atualize o objeto assignment. Somente professores na classe podem fazer isso. Observe que você não pode usar uma solicitação de PATCH para alterar o status de uma atribuição. Use a ação de publicação para alterar o status da atribuição.
localization_priority: Normal
ms.openlocfilehash: 78d5b526468fbdf35c3529084f878f8c35216c99
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838287"
---
# <a name="update-educationassignment"></a><span data-ttu-id="1f322-106">Atualizar educationassignment</span><span class="sxs-lookup"><span data-stu-id="1f322-106">Update educationassignment</span></span>

> <span data-ttu-id="1f322-107">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1f322-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f322-108">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1f322-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1f322-109">Atualize o objeto assignment.</span><span class="sxs-lookup"><span data-stu-id="1f322-109">Update the assignment object.</span></span> <span data-ttu-id="1f322-110">Somente professores na classe podem fazer isso.</span><span class="sxs-lookup"><span data-stu-id="1f322-110">Only teachers in the class can do this.</span></span> <span data-ttu-id="1f322-111">Observe que você não pode usar uma solicitação de PATCH para alterar o status de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="1f322-111">Note that you can't use a PATCH request to change the status of an assignment.</span></span> <span data-ttu-id="1f322-112">Use a ação [Publicar](../api/educationassignment-publish.md) para alterar o status da atribuição.</span><span class="sxs-lookup"><span data-stu-id="1f322-112">Use the [publish](../api/educationassignment-publish.md) action to change the assignment status.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f322-113">Permissions</span><span class="sxs-lookup"><span data-stu-id="1f322-113">Permissions</span></span>
<span data-ttu-id="1f322-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f322-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f322-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f322-116">Permission type</span></span>      | <span data-ttu-id="1f322-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1f322-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f322-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f322-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="1f322-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f322-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="1f322-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f322-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1f322-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f322-121">Not supported.</span></span>  |
|<span data-ttu-id="1f322-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f322-122">Application</span></span> | <span data-ttu-id="1f322-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f322-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1f322-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f322-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1f322-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f322-125">Request headers</span></span>
| <span data-ttu-id="1f322-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1f322-126">Header</span></span>       | <span data-ttu-id="1f322-127">Valor</span><span class="sxs-lookup"><span data-stu-id="1f322-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1f322-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f322-128">Authorization</span></span>  | <span data-ttu-id="1f322-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f322-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1f322-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1f322-131">Content-Type</span></span>  | <span data-ttu-id="1f322-132">application/json</span><span class="sxs-lookup"><span data-stu-id="1f322-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1f322-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f322-133">Request body</span></span>
<span data-ttu-id="1f322-134">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="1f322-134">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="1f322-135">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="1f322-135">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1f322-136">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="1f322-136">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1f322-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f322-137">Property</span></span>     | <span data-ttu-id="1f322-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f322-138">Type</span></span>   |<span data-ttu-id="1f322-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f322-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f322-140">allowLateSubmissions</span><span class="sxs-lookup"><span data-stu-id="1f322-140">allowLateSubmissions</span></span>|<span data-ttu-id="1f322-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="1f322-141">Boolean</span></span>| <span data-ttu-id="1f322-142">Se envios podem ser enviados após a data de vencimento.</span><span class="sxs-lookup"><span data-stu-id="1f322-142">Whether submissions can be submitted after the due date.</span></span>|
|<span data-ttu-id="1f322-143">allowStudentsToAddResourcesToSubmission</span><span class="sxs-lookup"><span data-stu-id="1f322-143">allowStudentsToAddResourcesToSubmission</span></span>|<span data-ttu-id="1f322-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="1f322-144">Boolean</span></span>| <span data-ttu-id="1f322-145">Se um estudante pode adicionar recursos para o envio de um.</span><span class="sxs-lookup"><span data-stu-id="1f322-145">Whether a student can add resources to a submission.</span></span> <span data-ttu-id="1f322-146">Indicado se os únicos itens no envio provém da lista de recursos de atribuição.</span><span class="sxs-lookup"><span data-stu-id="1f322-146">Indicated whether the only items on the submission came from the assignment resource list.</span></span> |
|<span data-ttu-id="1f322-147">assignDateTime</span><span class="sxs-lookup"><span data-stu-id="1f322-147">assignDateTime</span></span>|<span data-ttu-id="1f322-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f322-148">DateTimeOffset</span></span>| <span data-ttu-id="1f322-149">Data em que a atribuição deve ser publicada aos alunos.</span><span class="sxs-lookup"><span data-stu-id="1f322-149">Date the assignment should be published to students.</span></span> |
|<span data-ttu-id="1f322-150">assignTo</span><span class="sxs-lookup"><span data-stu-id="1f322-150">assignTo</span></span>|<span data-ttu-id="1f322-151">educationAssignmentRecipient</span><span class="sxs-lookup"><span data-stu-id="1f322-151">educationAssignmentRecipient</span></span>| <span data-ttu-id="1f322-152">Alunos que fazer a atribuição.</span><span class="sxs-lookup"><span data-stu-id="1f322-152">Students who get the assignment.</span></span>|
|<span data-ttu-id="1f322-153">displayName</span><span class="sxs-lookup"><span data-stu-id="1f322-153">displayName</span></span>|<span data-ttu-id="1f322-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f322-154">String</span></span>| <span data-ttu-id="1f322-155">Nome da atribuição.</span><span class="sxs-lookup"><span data-stu-id="1f322-155">Name of assignment.</span></span> |
|<span data-ttu-id="1f322-156">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="1f322-156">dueDateTime</span></span>|<span data-ttu-id="1f322-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f322-157">DateTimeOffset</span></span>| <span data-ttu-id="1f322-158">Atribuição de data deve ser concluída.</span><span class="sxs-lookup"><span data-stu-id="1f322-158">Date assignment is due.</span></span> |
|<span data-ttu-id="1f322-159">classificação</span><span class="sxs-lookup"><span data-stu-id="1f322-159">grading</span></span>|<span data-ttu-id="1f322-160">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="1f322-160">educationAssignmentGradeType</span></span>| <span data-ttu-id="1f322-161">Como a atribuição vai ser Graduada.</span><span class="sxs-lookup"><span data-stu-id="1f322-161">How the assignment will be graded.</span></span>|
|<span data-ttu-id="1f322-162">instruções</span><span class="sxs-lookup"><span data-stu-id="1f322-162">instructions</span></span>|<span data-ttu-id="1f322-163">itemBody</span><span class="sxs-lookup"><span data-stu-id="1f322-163">itemBody</span></span>| <span data-ttu-id="1f322-164">Instruções a ser dada aos alunos junto com a atribuição.</span><span class="sxs-lookup"><span data-stu-id="1f322-164">Instructions to be given to the students along with the assignment.</span></span> |

## <a name="response"></a><span data-ttu-id="1f322-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f322-165">Response</span></span>
<span data-ttu-id="1f322-166">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [educationAssignment](../resources/educationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f322-166">If successful, this method returns a `200 OK` response code and an updated [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1f322-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f322-167">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f322-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f322-168">Request</span></span>
<span data-ttu-id="1f322-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f322-169">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="1f322-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f322-170">Response</span></span>
<span data-ttu-id="1f322-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1f322-171">The following is an example of the response.</span></span> 

><span data-ttu-id="1f322-172">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1f322-172">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1f322-173">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1f322-173">All of the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Update educationassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
