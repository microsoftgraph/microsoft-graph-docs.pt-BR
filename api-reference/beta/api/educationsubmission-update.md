---
title: Atualizar educationsubmission
description: Adicione uma classificação e comentários a um envio. Somente os professores podem executar essa operação. Observe que a permissão básica não tem acesso às propriedades da graduação e, portanto, não pode gravar no meio ou nos comentários. Esta ação não libera o conceito e o feedback para o aluno. Um professor deve executar uma ação de liberação explícita para que os dados da grade sejam retornados ao aluno.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3ad2c4663eb2d93d36a370762a650f4a38f48c03
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954946"
---
# <a name="update-educationsubmission"></a><span data-ttu-id="6f565-107">Atualizar educationsubmission</span><span class="sxs-lookup"><span data-stu-id="6f565-107">Update educationsubmission</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f565-108">Adicione uma classificação e comentários a um envio.</span><span class="sxs-lookup"><span data-stu-id="6f565-108">Add a grade and feedback to a submission.</span></span> <span data-ttu-id="6f565-109">Somente os professores podem executar essa operação.</span><span class="sxs-lookup"><span data-stu-id="6f565-109">Only teachers can perform this operation.</span></span> <span data-ttu-id="6f565-110">Observe que a permissão básica não tem acesso às propriedades da graduação e, portanto, não pode gravar no meio ou nos comentários.</span><span class="sxs-lookup"><span data-stu-id="6f565-110">Note that the Basic permission does not have access to the grade properties, and therefore cannot write to grade or feedback.</span></span> <span data-ttu-id="6f565-111">Esta ação não libera o conceito e o feedback para o aluno.</span><span class="sxs-lookup"><span data-stu-id="6f565-111">This action does not release the grade and feedback to the student.</span></span> <span data-ttu-id="6f565-112">Um professor deve executar uma ação de liberação explícita para que os dados da grade sejam retornados ao aluno.</span><span class="sxs-lookup"><span data-stu-id="6f565-112">A teacher must take an explicit release action for the grade data to be returned to the student.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f565-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="6f565-113">Permissions</span></span>
<span data-ttu-id="6f565-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f565-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f565-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f565-116">Permission type</span></span>      | <span data-ttu-id="6f565-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6f565-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f565-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f565-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="6f565-119">EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6f565-119">EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="6f565-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f565-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f565-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f565-121">Not supported.</span></span>   |
|<span data-ttu-id="6f565-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f565-122">Application</span></span> | <span data-ttu-id="6f565-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f565-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6f565-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f565-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6f565-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f565-125">Request headers</span></span>
| <span data-ttu-id="6f565-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6f565-126">Header</span></span>       | <span data-ttu-id="6f565-127">Valor</span><span class="sxs-lookup"><span data-stu-id="6f565-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6f565-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f565-128">Authorization</span></span>  | <span data-ttu-id="6f565-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f565-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6f565-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f565-131">Request body</span></span>
<span data-ttu-id="6f565-132">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="6f565-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6f565-133">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="6f565-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6f565-134">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="6f565-134">For best performance, don't include existing values that haven't changed.</span></span>

<!-- Provide the property descriptions. -->

| <span data-ttu-id="6f565-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f565-135">Property</span></span>     | <span data-ttu-id="6f565-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f565-136">Type</span></span>   |<span data-ttu-id="6f565-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f565-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f565-138">comentários</span><span class="sxs-lookup"><span data-stu-id="6f565-138">feedback</span></span>|<span data-ttu-id="6f565-139">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="6f565-139">educationFeedback</span></span>||
|<span data-ttu-id="6f565-140">grade</span><span class="sxs-lookup"><span data-stu-id="6f565-140">grade</span></span>|<span data-ttu-id="6f565-141">educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="6f565-141">educationAssignmentGrade</span></span>||

## <a name="response"></a><span data-ttu-id="6f565-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f565-142">Response</span></span>
<span data-ttu-id="6f565-143">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [educationSubmission](../resources/educationsubmission.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f565-143">If successful, this method returns a `200 OK` response code and an updated [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6f565-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f565-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6f565-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f565-145">Request</span></span>
<span data-ttu-id="6f565-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f565-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_educationsubmission"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7
Content-type: application/json
Content-length: 658

{
  "feedback": {
    "text": {
      "content": "Good work!",
      "contentType": "Text"
    },
    "feedbackDateTime": "2014-01-01T00:00:00Z",
    "feedbackBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      },
      "@odata.type": "microsoft.graph.identitySet"
    },
    "@odata.type": "microsoft.graph.educationFeedback"
  },
  "grade": {
      "gradedBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      },
      "@odata.type": "microsoft.graph.identitySet"
    },
    "gradedDateTime": "2014-01-01T00:00:00Z",
    "@odata.type": "microsoft.graph.educationAssignmentGrade"
  }
}
```
##### <a name="response"></a><span data-ttu-id="6f565-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f565-147">Response</span></span>
<span data-ttu-id="6f565-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6f565-148">The following is an example of the response.</span></span> 

><span data-ttu-id="6f565-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6f565-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1217

{
  "feedback": {
    "text": {
      "content": "Good work!",
      "contentType": "Text"
    },
    "feedbackDateTime": "2014-01-01T00:00:00Z",
    "feedbackBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      }
    },
    "@odata.type": "microsoft.graph.educationFeedback"
  },
  "grade": {
         "gradedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
          "@odata.type": "microsoft.graph.identitySet"
        },
        "gradedDateTime": "2014-01-01T00:00:00Z",
        "@odata.type": "microsoft.graph.educationAssignmentGrade"
  },
  "id": "850f51b7",
  "recipient": {
    userId:"dsfewsddf",
    "@odata.type": "#microsoft.graph.educationSubmissionRecipient"
  },
  "releasedBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012"
    },
  },
  "releasedDateTime": "2014-01-01T00:00:00Z",
  "resourcesFolderUrl": "String",
  "status": "completed",
  "submittedBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012"
    },
  },
  "submittedDateTime": "2014-01-01T00:00:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update educationsubmission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
