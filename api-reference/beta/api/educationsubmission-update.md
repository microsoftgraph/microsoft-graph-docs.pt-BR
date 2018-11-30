---
title: Atualizar educationsubmission
description: Adicione um nível e os comentários para o envio de um. Professores só podem executar essa operação. Observe que a permissão básica não tem acesso às propriedades do nível e, portanto, não é possível gravar em nível ou comentários. Essa ação não libera o nível e comentários ao aluno. Um professor deve executar uma ação de versão explícita para os dados de nível a ser retornado ao aluno.
ms.openlocfilehash: 64e9313c30ce97c2bdbfdb9d3b7fb3077208ab1d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037791"
---
# <a name="update-educationsubmission"></a><span data-ttu-id="f3949-107">Atualizar educationsubmission</span><span class="sxs-lookup"><span data-stu-id="f3949-107">Update educationsubmission</span></span>

> <span data-ttu-id="f3949-108">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f3949-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3949-109">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f3949-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f3949-110">Adicione um nível e os comentários para o envio de um.</span><span class="sxs-lookup"><span data-stu-id="f3949-110">Add a grade and feedback to a submission.</span></span> <span data-ttu-id="f3949-111">Professores só podem executar essa operação.</span><span class="sxs-lookup"><span data-stu-id="f3949-111">Only teachers can perform this operation.</span></span> <span data-ttu-id="f3949-112">Observe que a permissão básica não tem acesso às propriedades do nível e, portanto, não é possível gravar em nível ou comentários.</span><span class="sxs-lookup"><span data-stu-id="f3949-112">Note that the Basic permission does not have access to the grade properties, and therefore cannot write to grade or feedback.</span></span> <span data-ttu-id="f3949-113">Essa ação não libera o nível e comentários ao aluno.</span><span class="sxs-lookup"><span data-stu-id="f3949-113">This action does not release the grade and feedback to the student.</span></span> <span data-ttu-id="f3949-114">Um professor deve executar uma ação de versão explícita para os dados de nível a ser retornado ao aluno.</span><span class="sxs-lookup"><span data-stu-id="f3949-114">A teacher must take an explicit release action for the grade data to be returned to the student.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3949-115">Permissions</span><span class="sxs-lookup"><span data-stu-id="f3949-115">Permissions</span></span>
<span data-ttu-id="f3949-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3949-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3949-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3949-118">Permission type</span></span>      | <span data-ttu-id="f3949-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f3949-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3949-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3949-120">Delegated (work or school account)</span></span> |  <span data-ttu-id="f3949-121">EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3949-121">EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="f3949-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3949-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3949-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3949-123">Not supported.</span></span>   |
|<span data-ttu-id="f3949-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3949-124">Application</span></span> | <span data-ttu-id="f3949-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3949-125">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f3949-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3949-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f3949-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3949-127">Request headers</span></span>
| <span data-ttu-id="f3949-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f3949-128">Header</span></span>       | <span data-ttu-id="f3949-129">Valor</span><span class="sxs-lookup"><span data-stu-id="f3949-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f3949-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3949-130">Authorization</span></span>  | <span data-ttu-id="f3949-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3949-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f3949-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3949-133">Request body</span></span>
<span data-ttu-id="f3949-134">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="f3949-134">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f3949-135">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="f3949-135">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f3949-136">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f3949-136">For best performance, don't include existing values that haven't changed.</span></span>

<!-- Provide the property descriptions. -->

| <span data-ttu-id="f3949-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3949-137">Property</span></span>     | <span data-ttu-id="f3949-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3949-138">Type</span></span>   |<span data-ttu-id="f3949-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3949-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3949-140">comentários</span><span class="sxs-lookup"><span data-stu-id="f3949-140">feedback</span></span>|<span data-ttu-id="f3949-141">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="f3949-141">educationFeedback</span></span>||
|<span data-ttu-id="f3949-142">grade</span><span class="sxs-lookup"><span data-stu-id="f3949-142">grade</span></span>|<span data-ttu-id="f3949-143">educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="f3949-143">educationAssignmentGrade</span></span>||

## <a name="response"></a><span data-ttu-id="f3949-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3949-144">Response</span></span>
<span data-ttu-id="f3949-145">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [educationSubmission](../resources/educationsubmission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3949-145">If successful, this method returns a `200 OK` response code and an updated [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f3949-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3949-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f3949-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3949-147">Request</span></span>
<span data-ttu-id="f3949-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3949-148">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="f3949-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3949-149">Response</span></span>
<span data-ttu-id="f3949-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f3949-150">The following is an example of the response.</span></span> 

><span data-ttu-id="f3949-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f3949-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update educationsubmission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
