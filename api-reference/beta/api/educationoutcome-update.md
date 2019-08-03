---
title: Atualizar educationOutcome
description: Atualize as propriedades do objeto educationOutcome.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2c7b85d3456927e6a63f61f11722dfe8eccf270e
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173178"
---
# <a name="update-educationoutcome"></a><span data-ttu-id="5663e-103">Atualizar educationoutcome</span><span class="sxs-lookup"><span data-stu-id="5663e-103">Update educationoutcome</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5663e-104">Atualiza as propriedades de um objeto [educationOutcome](../resources/educationoutcome.md) .</span><span class="sxs-lookup"><span data-stu-id="5663e-104">Update the properties of an [educationOutcome](../resources/educationoutcome.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5663e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5663e-105">Permissions</span></span>

<span data-ttu-id="5663e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5663e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5663e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5663e-108">Permission type</span></span>                        | <span data-ttu-id="5663e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5663e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5663e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5663e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5663e-111">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5663e-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="5663e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5663e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5663e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5663e-113">Not supported.</span></span> |
| <span data-ttu-id="5663e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5663e-114">Application</span></span>                            | <span data-ttu-id="5663e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5663e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5663e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5663e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /education/classes/{id}/assignments/{id}/submissions/{id}/outcomes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5663e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5663e-117">Request headers</span></span>

| <span data-ttu-id="5663e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="5663e-118">Name</span></span>       | <span data-ttu-id="5663e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="5663e-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5663e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="5663e-120">Authorization</span></span> | <span data-ttu-id="5663e-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="5663e-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5663e-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5663e-122">Request body</span></span>

<span data-ttu-id="5663e-123">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="5663e-123">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5663e-124">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="5663e-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5663e-125">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="5663e-125">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="5663e-126">O objeto educationOutcome será um dos seguintes tipos derivados: **educationPointsOutcome**, **educationFeedbackOutcome**ou **educationRubricOutcome**.</span><span class="sxs-lookup"><span data-stu-id="5663e-126">The educationOutcome object will be one of the following derived types: **educationPointsOutcome**, **educationFeedbackOutcome**, or **educationRubricOutcome**.</span></span> <span data-ttu-id="5663e-127">Forneça as propriedades específicas relevantes ao tipo de resultado que está sendo corrigido.</span><span class="sxs-lookup"><span data-stu-id="5663e-127">Supply the specific properties relevant to the type of outcome being patched.</span></span>

<span data-ttu-id="5663e-128">Todos os tipos de resultados derivados têm uma propriedade regular e "publicada" apropriada para esse tipo de resultado; por exemplo, **pontos** e **publishedPoints**, **feedback** e **publishedFeedback**.</span><span class="sxs-lookup"><span data-stu-id="5663e-128">All derived outcome types have a regular and a "published" property appropriate to that type of outcome; for example, **points** and **publishedPoints**, **feedback** and **publishedFeedback**.</span></span> <span data-ttu-id="5663e-129">Não atualiza a propriedade "published"; é para uso interno.</span><span class="sxs-lookup"><span data-stu-id="5663e-129">Do not update the "published" property; it is for internal use.</span></span> <span data-ttu-id="5663e-130">Por exemplo, para atribuir pontos a um **educationPointsOutcome**, atualize a \*\*\*\* propriedade Points, mas não atualize o **publishedPoints**.</span><span class="sxs-lookup"><span data-stu-id="5663e-130">For example, to assign points to an **educationPointsOutcome**, update the **points** property, but do not update **publishedPoints**.</span></span>

## <a name="response"></a><span data-ttu-id="5663e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5663e-131">Response</span></span>

<span data-ttu-id="5663e-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [educationOutcome](../resources/educationoutcome.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5663e-132">If successful, this method returns a `200 OK` response code and an updated [educationOutcome](../resources/educationoutcome.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5663e-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5663e-133">Examples</span></span>

### <a name="example-1-update-a-feedback-outcome"></a><span data-ttu-id="5663e-134">Exemplo 1: atualizar um resultado de comentários</span><span class="sxs-lookup"><span data-stu-id="5663e-134">Example 1: Update a Feedback Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="5663e-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5663e-135">Request</span></span>

<span data-ttu-id="5663e-136">Veja a seguir um exemplo da solicitação para atualizar um resultado de comentários.</span><span class="sxs-lookup"><span data-stu-id="5663e-136">The following is an example of the request for updating a feedback outcome.</span></span>
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

#### <a name="response"></a><span data-ttu-id="5663e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5663e-137">Response</span></span>

<span data-ttu-id="5663e-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5663e-138">The following is an example of the response.</span></span>

> <span data-ttu-id="5663e-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5663e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-update-a-points-outcome"></a><span data-ttu-id="5663e-141">Exemplo 2: atualizar um resultado de pontos</span><span class="sxs-lookup"><span data-stu-id="5663e-141">Example 2: Update a Points Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="5663e-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5663e-142">Request</span></span>

<span data-ttu-id="5663e-143">Veja a seguir um exemplo da solicitação para atualizar um resultado de pontos.</span><span class="sxs-lookup"><span data-stu-id="5663e-143">The following is an example of the request for updating a points outcome.</span></span>
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

#### <a name="response"></a><span data-ttu-id="5663e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="5663e-144">Response</span></span>

<span data-ttu-id="5663e-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5663e-145">The following is an example of the response.</span></span>

> <span data-ttu-id="5663e-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5663e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-update-a-rubric-outcome"></a><span data-ttu-id="5663e-148">Exemplo 3: atualizar um resultado de amostra rubric</span><span class="sxs-lookup"><span data-stu-id="5663e-148">Example 3: Update a Rubric Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="5663e-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5663e-149">Request</span></span>

<span data-ttu-id="5663e-150">Veja a seguir um exemplo da solicitação para atualizar um resultado amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="5663e-150">The following is an example of the request for updating a rubric outcome.</span></span>
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

#### <a name="response"></a><span data-ttu-id="5663e-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="5663e-151">Response</span></span>

<span data-ttu-id="5663e-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5663e-152">The following is an example of the response.</span></span>

> <span data-ttu-id="5663e-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5663e-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
