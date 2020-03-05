---
title: Atualizar educationOutcome
description: Atualize as propriedades do objeto educationOutcome.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a02098f65bdf9357bcc944d667d7657871895e1e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42426189"
---
# <a name="update-educationoutcome"></a><span data-ttu-id="8f91e-103">Atualizar educationoutcome</span><span class="sxs-lookup"><span data-stu-id="8f91e-103">Update educationoutcome</span></span>

<span data-ttu-id="8f91e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8f91e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f91e-105">Atualiza as propriedades de um objeto [educationOutcome](../resources/educationoutcome.md) .</span><span class="sxs-lookup"><span data-stu-id="8f91e-105">Update the properties of an [educationOutcome](../resources/educationoutcome.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f91e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8f91e-106">Permissions</span></span>

<span data-ttu-id="8f91e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f91e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f91e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f91e-109">Permission type</span></span>                        | <span data-ttu-id="8f91e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8f91e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8f91e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f91e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f91e-112">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f91e-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="8f91e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f91e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f91e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f91e-114">Not supported.</span></span> |
| <span data-ttu-id="8f91e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f91e-115">Application</span></span>                            | <span data-ttu-id="8f91e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f91e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f91e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f91e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /education/classes/{id}/assignments/{id}/submissions/{id}/outcomes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8f91e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f91e-118">Request headers</span></span>

| <span data-ttu-id="8f91e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8f91e-119">Name</span></span>       | <span data-ttu-id="8f91e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f91e-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8f91e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f91e-121">Authorization</span></span> | <span data-ttu-id="8f91e-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="8f91e-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f91e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f91e-123">Request body</span></span>

<span data-ttu-id="8f91e-124">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="8f91e-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8f91e-125">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="8f91e-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8f91e-126">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="8f91e-126">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="8f91e-127">O objeto educationOutcome será um dos seguintes tipos derivados: **educationPointsOutcome**, **educationFeedbackOutcome**ou **educationRubricOutcome**.</span><span class="sxs-lookup"><span data-stu-id="8f91e-127">The educationOutcome object will be one of the following derived types: **educationPointsOutcome**, **educationFeedbackOutcome**, or **educationRubricOutcome**.</span></span> <span data-ttu-id="8f91e-128">Forneça as propriedades específicas relevantes ao tipo de resultado que está sendo corrigido.</span><span class="sxs-lookup"><span data-stu-id="8f91e-128">Supply the specific properties relevant to the type of outcome being patched.</span></span>

<span data-ttu-id="8f91e-129">Todos os tipos de resultados derivados têm uma propriedade regular e "publicada" apropriada para esse tipo de resultado; por exemplo, **pontos** e **publishedPoints**, **feedback** e **publishedFeedback**.</span><span class="sxs-lookup"><span data-stu-id="8f91e-129">All derived outcome types have a regular and a "published" property appropriate to that type of outcome; for example, **points** and **publishedPoints**, **feedback** and **publishedFeedback**.</span></span> <span data-ttu-id="8f91e-130">Não atualiza a propriedade "published"; é para uso interno.</span><span class="sxs-lookup"><span data-stu-id="8f91e-130">Do not update the "published" property; it is for internal use.</span></span> <span data-ttu-id="8f91e-131">Por exemplo, para atribuir pontos a um **educationPointsOutcome**, atualize a propriedade **Points** , mas não atualize o **publishedPoints**.</span><span class="sxs-lookup"><span data-stu-id="8f91e-131">For example, to assign points to an **educationPointsOutcome**, update the **points** property, but do not update **publishedPoints**.</span></span>

## <a name="response"></a><span data-ttu-id="8f91e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f91e-132">Response</span></span>

<span data-ttu-id="8f91e-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [educationOutcome](../resources/educationoutcome.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f91e-133">If successful, this method returns a `200 OK` response code and an updated [educationOutcome](../resources/educationoutcome.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8f91e-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8f91e-134">Examples</span></span>

### <a name="example-1-update-a-feedback-outcome"></a><span data-ttu-id="8f91e-135">Exemplo 1: atualizar um resultado de comentários</span><span class="sxs-lookup"><span data-stu-id="8f91e-135">Example 1: Update a Feedback Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="8f91e-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f91e-136">Request</span></span>

<span data-ttu-id="8f91e-137">Veja a seguir um exemplo da solicitação para atualizar um resultado de comentários.</span><span class="sxs-lookup"><span data-stu-id="8f91e-137">The following is an example of the request for updating a feedback outcome.</span></span>

# <a name="http"></a>[<span data-ttu-id="8f91e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f91e-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationfeedbackoutcome"
}-->

```http
PATCH https://graph.microsoft.com/beta/education/me/assignments/{id}/submissions/{id}/outcomes/{id}
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.educationFeedbackOutcome",
    "feedback":{
        "text":{
            "content":"This is feedback for the assignment as a whole.",
            "contentType":"text"
        }
    }
}
```
# <a name="javascript"></a>[<span data-ttu-id="8f91e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f91e-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationfeedbackoutcome-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8f91e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f91e-140">Response</span></span>

<span data-ttu-id="8f91e-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8f91e-141">The following is an example of the response.</span></span>

> <span data-ttu-id="8f91e-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f91e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationFeedbackOutcome"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.educationFeedbackOutcome",
    "id": "ca05367a-b292-42d5-aff7-5d279feeace8",
    "lastModifiedBy": {
        "user": {
            "id": "9391878d-903c-406c-bb1c-0f17d00fd878"
        }
    },
    "feedback": {
        "feedbackDateTime": "2019-07-31T21:10:30.3231461Z",
        "text": {
            "content": "This is feedback for the assignment as a whole.",
            "contentType": "text"
        },
        "feedbackBy": {
            "user": {
                "id": "9391878d-903c-406c-bb1c-0f17d00fd878",
            }
        }
    }
}
```

### <a name="example-2-update-a-points-outcome"></a><span data-ttu-id="8f91e-144">Exemplo 2: atualizar um resultado de pontos</span><span class="sxs-lookup"><span data-stu-id="8f91e-144">Example 2: Update a Points Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="8f91e-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f91e-145">Request</span></span>

<span data-ttu-id="8f91e-146">Veja a seguir um exemplo da solicitação para atualizar um resultado de pontos.</span><span class="sxs-lookup"><span data-stu-id="8f91e-146">The following is an example of the request for updating a points outcome.</span></span>

# <a name="http"></a>[<span data-ttu-id="8f91e-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f91e-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationpointsoutcome"
}-->

```http
PATCH https://graph.microsoft.com/beta/education/me/assignments/{id}/submissions/{id}/outcomes/{id}
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.educationPointsOutcome",
    "points":{
        "@odata.type":"#microsoft.graph.educationAssignmentPointsGrade",
        "points":85.0
    }
}
```
# <a name="javascript"></a>[<span data-ttu-id="8f91e-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f91e-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationpointsoutcome-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8f91e-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f91e-149">Response</span></span>

<span data-ttu-id="8f91e-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8f91e-150">The following is an example of the response.</span></span>

> <span data-ttu-id="8f91e-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f91e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationPointsOutcome"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.educationPointsOutcome",
    "id":"ea1351f6-ba33-4940-b2cb-6a7254af2dc8",
    "lastModifiedBy":{
        "user":{
            "id":"9391878d-903c-406c-bb1c-0f17d00fd878"
        }
    },
    "points":{
        "gradedDateTime":"2019-07-15T22:35:48.2429387Z",
        "points":85.0,
        "gradedBy":{
            "user":{
                "id":"9391878d-903c-406c-bb1c-0f17d00fd878"
            }
        }
    }
}
```

### <a name="example-3-update-a-rubric-outcome"></a><span data-ttu-id="8f91e-153">Exemplo 3: atualizar um resultado de amostra rubric</span><span class="sxs-lookup"><span data-stu-id="8f91e-153">Example 3: Update a Rubric Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="8f91e-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f91e-154">Request</span></span>

<span data-ttu-id="8f91e-155">Veja a seguir um exemplo da solicitação para atualizar um resultado amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="8f91e-155">The following is an example of the request for updating a rubric outcome.</span></span>

# <a name="http"></a>[<span data-ttu-id="8f91e-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f91e-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationoutcome"
}-->

```http
PATCH https://graph.microsoft.com/beta/education/me/assignments/{id}/submissions/{id}/outcomes/{id}
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.educationRubricOutcome",
    "rubricQualityFeedback":[
        {
            "qualityId":"9a145aa8-f3d9-43a1-8f77-5387ff0693f2",
            "feedback":{
                "content":"This is feedback specific to the first quality of the rubric.",
                "contentType":"text"
            }
        },
        {
            "qualityId":"d2331fb2-2761-402e-8de6-93e0afaa076e",
            "feedback":{
                "content":"This is feedback specific to the second quality of the rubric.",
                "contentType":"text"
            }
        }
    ],
    "rubricQualitySelectedLevels":[
        {
            "qualityId":"9a145aa8-f3d9-43a1-8f77-5387ff0693f2",
            "columnId":"4fb17a1d-5681-46c2-a295-4e305c3eae23"
        },
        {
            "qualityId":"d2331fb2-2761-402e-8de6-93e0afaa076e",
            "columnId":"aac076bf-51ba-48c5-a2e0-ee235b0b9740"
        }
    ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="8f91e-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f91e-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationoutcome-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8f91e-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f91e-158">Response</span></span>

<span data-ttu-id="8f91e-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8f91e-159">The following is an example of the response.</span></span>

> <span data-ttu-id="8f91e-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f91e-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationPointsOutcome"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.type": "#microsoft.graph.educationRubricOutcome",
    "id": "65a46d78-1a2b-4a7e-bcf8-78a22ac2611b",
    "rubricQualityFeedback": [
        {
            "qualityId": "9a145aa8-f3d9-43a1-8f77-5387ff0693f2",
            "feedback": {
                "content": "This is feedback specific to the first quality of the rubric.",
                "contentType": "text"
            }
        },
        {
            "qualityId": "d2331fb2-2761-402e-8de6-93e0afaa076e",
            "feedback": {
                "content": "This is feedback specific to the second quality of the rubric.",
                "contentType": "text"
            }
        }
    ],
    "rubricQualitySelectedLevels": [
        {
            "qualityId": "9a145aa8-f3d9-43a1-8f77-5387ff0693f2",
            "columnId": "4fb17a1d-5681-46c2-a295-4e305c3eae23"
        },
        {
            "qualityId": "d2331fb2-2761-402e-8de6-93e0afaa076e",
            "columnId": "aac076bf-51ba-48c5-a2e0-ee235b0b9740"
        }
    ]
}
```



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationoutcome",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
