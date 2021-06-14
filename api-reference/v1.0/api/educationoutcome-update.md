---
title: Atualizar educationOutcome
description: Atualize as propriedades do objeto educationOutcome.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b6b3fba4f87f17528c1e4774b34ba4faeae43bfb
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912154"
---
# <a name="update-educationoutcome"></a><span data-ttu-id="182bb-103">Atualizar educationoutcome</span><span class="sxs-lookup"><span data-stu-id="182bb-103">Update educationoutcome</span></span>

<span data-ttu-id="182bb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="182bb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="182bb-105">Atualize as propriedades de um [objeto educationOutcome.](../resources/educationoutcome.md)</span><span class="sxs-lookup"><span data-stu-id="182bb-105">Update the properties of an [educationOutcome](../resources/educationoutcome.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="182bb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="182bb-106">Permissions</span></span>

<span data-ttu-id="182bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="182bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="182bb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="182bb-109">Permission type</span></span>                        | <span data-ttu-id="182bb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="182bb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="182bb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="182bb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="182bb-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="182bb-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="182bb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="182bb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="182bb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="182bb-114">Not supported.</span></span> |
| <span data-ttu-id="182bb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="182bb-115">Application</span></span>                            | <span data-ttu-id="182bb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="182bb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="182bb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="182bb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/outcomes/9c0f2850-ff8f-4fd6-b3ac-e23077b59141
```

## <a name="request-headers"></a><span data-ttu-id="182bb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="182bb-118">Request headers</span></span>

| <span data-ttu-id="182bb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="182bb-119">Name</span></span>       | <span data-ttu-id="182bb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="182bb-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="182bb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="182bb-121">Authorization</span></span> | <span data-ttu-id="182bb-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="182bb-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="182bb-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="182bb-123">Request body</span></span>

<span data-ttu-id="182bb-124">No corpo da solicitação, fornece apenas os valores dos campos que você deseja atualizar.</span><span class="sxs-lookup"><span data-stu-id="182bb-124">In the request body, supply only the values of the fields you want to update.</span></span>

<span data-ttu-id="182bb-125">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="182bb-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="182bb-126">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="182bb-126">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="182bb-127">O objeto educationOutcome será um dos seguintes tipos **derivados: educationPointsOutcome**, **educationFeedbackOutcome** ou **educationRubricOutcome**.</span><span class="sxs-lookup"><span data-stu-id="182bb-127">The educationOutcome object will be one of the following derived types: **educationPointsOutcome**, **educationFeedbackOutcome**, or **educationRubricOutcome**.</span></span> <span data-ttu-id="182bb-128">Fornecer as propriedades específicas relevantes para o tipo de resultado que está sendo remendado.</span><span class="sxs-lookup"><span data-stu-id="182bb-128">Supply the specific properties relevant to the type of outcome being patched.</span></span>

<span data-ttu-id="182bb-129">Todos os tipos de resultado derivados têm uma propriedade regular e "publicada" apropriada para esse tipo de resultado; por exemplo, **pontos e** **publishedPoints**, **comentários** e **publishedFeedback**.</span><span class="sxs-lookup"><span data-stu-id="182bb-129">All derived outcome types have a regular and a "published" property appropriate to that type of outcome; for example, **points** and **publishedPoints**, **feedback** and **publishedFeedback**.</span></span> <span data-ttu-id="182bb-130">Não atualize a propriedade "publicado"; é para uso interno.</span><span class="sxs-lookup"><span data-stu-id="182bb-130">Don't update the "published" property; it is for internal use.</span></span> <span data-ttu-id="182bb-131">Por exemplo, para atribuir pontos a **um educationPointsOutcome**, atualize a propriedade **points,** mas Não atualize **publishedPoints**.</span><span class="sxs-lookup"><span data-stu-id="182bb-131">For example, to assign points to an **educationPointsOutcome**, update the **points** property, but Don't update **publishedPoints**.</span></span>

## <a name="response"></a><span data-ttu-id="182bb-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="182bb-132">Response</span></span>

<span data-ttu-id="182bb-133">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationOutcome](../resources/educationoutcome.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="182bb-133">If successful, this method returns a `200 OK` response code and an updated [educationOutcome](../resources/educationoutcome.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="182bb-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="182bb-134">Examples</span></span>

### <a name="example-1-update-a-feedback-outcome"></a><span data-ttu-id="182bb-135">Exemplo 1: Atualizar um resultado de feedback</span><span class="sxs-lookup"><span data-stu-id="182bb-135">Example 1: Update a Feedback Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="182bb-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="182bb-136">Request</span></span>

<span data-ttu-id="182bb-137">A seguir, um exemplo da solicitação de atualização de um resultado de feedback.</span><span class="sxs-lookup"><span data-stu-id="182bb-137">The following is an example of the request for updating a feedback outcome.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_educationfeedbackoutcome"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/outcomes/9c0f2850-ff8f-4fd6-b3ac-e23077b59141
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

#### <a name="response"></a><span data-ttu-id="182bb-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="182bb-138">Response</span></span>

<span data-ttu-id="182bb-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="182bb-139">The following is an example of the response.</span></span>

> <span data-ttu-id="182bb-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="182bb-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-update-a-points-outcome"></a><span data-ttu-id="182bb-141">Exemplo 2: Atualizar um resultado de pontos</span><span class="sxs-lookup"><span data-stu-id="182bb-141">Example 2: Update a Points Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="182bb-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="182bb-142">Request</span></span>

<span data-ttu-id="182bb-143">A seguir, um exemplo da solicitação de atualização de um resultado de pontos.</span><span class="sxs-lookup"><span data-stu-id="182bb-143">The following is an example of the request for updating a points outcome.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_educationpointsoutcome"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/outcomes/9c0f2850-ff8f-4fd6-b3ac-e23077b59141
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.educationPointsOutcome",
    "points":{
        "@odata.type":"#microsoft.graph.educationAssignmentPointsGrade",
        "points":85.0
    }
}
```

#### <a name="response"></a><span data-ttu-id="182bb-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="182bb-144">Response</span></span>

<span data-ttu-id="182bb-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="182bb-145">The following is an example of the response.</span></span>

> <span data-ttu-id="182bb-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="182bb-146">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-update-a-rubric-outcome"></a><span data-ttu-id="182bb-147">Exemplo 3: atualizar um resultado rubrico</span><span class="sxs-lookup"><span data-stu-id="182bb-147">Example 3: Update a Rubric Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="182bb-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="182bb-148">Request</span></span>

<span data-ttu-id="182bb-149">A seguir, um exemplo da solicitação de atualização de um resultado rubrico.</span><span class="sxs-lookup"><span data-stu-id="182bb-149">The following is an example of the request for updating a rubric outcome.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_educationoutcome"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/outcomes/9c0f2850-ff8f-4fd6-b3ac-e23077b59141
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

#### <a name="response"></a><span data-ttu-id="182bb-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="182bb-150">Response</span></span>

<span data-ttu-id="182bb-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="182bb-151">The following is an example of the response.</span></span>

> <span data-ttu-id="182bb-152">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="182bb-152">**Note:** The response object shown here might be shortened for readability.</span></span>

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


