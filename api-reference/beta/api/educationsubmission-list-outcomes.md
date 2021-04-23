---
title: Listar resultados
description: Recupere uma lista de objetos educationoutcome.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 623fd7562dcfc925553996eda139377f623fa4a3
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961223"
---
# <a name="list-outcomes"></a><span data-ttu-id="c9a2e-103">Listar resultados</span><span class="sxs-lookup"><span data-stu-id="c9a2e-103">List outcomes</span></span>

<span data-ttu-id="c9a2e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9a2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9a2e-105">Recupere uma lista de [objetos educationOutcome.](../resources/educationoutcome.md)</span><span class="sxs-lookup"><span data-stu-id="c9a2e-105">Retrieve a list of [educationOutcome](../resources/educationoutcome.md) objects.</span></span>  <span data-ttu-id="c9a2e-106">Há três tipos de resultados: **educationPointsOutcome**, **educationFeedbackOutcome** e **educationRubricOutcome**.</span><span class="sxs-lookup"><span data-stu-id="c9a2e-106">There are three types of outcomes: **educationPointsOutcome**, **educationFeedbackOutcome**, and **educationRubricOutcome**.</span></span>

<span data-ttu-id="c9a2e-107">Um envio para uma atribuição de crédito (aquele que não tem valor de ponto e nenhuma rubrica) terá [um educationFeedbackOutcome](../resources/educationpointsoutcome.md).</span><span class="sxs-lookup"><span data-stu-id="c9a2e-107">A submission for a credit assignment (one that has no point value and no rubric) will have an [educationFeedbackOutcome](../resources/educationpointsoutcome.md).</span></span> <span data-ttu-id="c9a2e-108">(Também pode retornar [um educationPointsOutcome](../resources/educationpointsoutcome.md), mas esse resultado é ignorado.)</span><span class="sxs-lookup"><span data-stu-id="c9a2e-108">(It might also return an [educationPointsOutcome](../resources/educationpointsoutcome.md), but that outcome is ignored.)</span></span>

<span data-ttu-id="c9a2e-109">Um envio para uma atribuição de pontos (um que tenha um valor de ponto atribuído) terá um [educationFeedbackOutcome](../resources/educationpointsoutcome.md) e [um educationPointsOutcome](../resources/educationpointsoutcome.md).</span><span class="sxs-lookup"><span data-stu-id="c9a2e-109">A submission for a points assignment (one that has a point value assigned) will have both an [educationFeedbackOutcome](../resources/educationpointsoutcome.md) and an [educationPointsOutcome](../resources/educationpointsoutcome.md).</span></span>

<span data-ttu-id="c9a2e-110">Um envio para uma atribuição com uma rubrica anexada, se a rubrica for uma rubrica de crédito (sem pontos), terá [um educationFeedbackOutcome](../resources/educationpointsoutcome.md) e [um educationRubricOutcome](../resources/educationrubricoutcome.md).</span><span class="sxs-lookup"><span data-stu-id="c9a2e-110">A submission for an assignment with an attached rubric, if the rubric is a credit rubric (no points), will have an [educationFeedbackOutcome](../resources/educationpointsoutcome.md) and an [educationRubricOutcome](../resources/educationrubricoutcome.md).</span></span> <span data-ttu-id="c9a2e-111">(Também pode retornar [um educationPointsOutcome](../resources/educationpointsoutcome.md), mas esse resultado é ignorado.)</span><span class="sxs-lookup"><span data-stu-id="c9a2e-111">(It might also return an [educationPointsOutcome](../resources/educationpointsoutcome.md), but that outcome is ignored.)</span></span>

<span data-ttu-id="c9a2e-112">Um envio para uma atribuição com uma rubrica anexada, se a rubrica for uma rubrica de pontos, terá [um educationFeedbackOutcome](../resources/educationpointsoutcome.md), um [educationPointsOutcome](.. /resources/educationpointsoutcome.md e [educationRubricOutcome](../resources/educationrubricoutcome.md).</span><span class="sxs-lookup"><span data-stu-id="c9a2e-112">A submission for an assignment with an attached rubric, if the rubric is a points rubric, will have an [educationFeedbackOutcome](../resources/educationpointsoutcome.md), an [educationPointsOutcome](../resources/educationpointsoutcome.md, and an [educationRubricOutcome](../resources/educationrubricoutcome.md).</span></span>

<span data-ttu-id="c9a2e-113">Todos os tipos de resultados têm uma propriedade regular e publicada apropriada a esse tipo de resultado; por exemplo, **pontos e** **publishedPoints**, **comentários** e **publishedFeedback**.</span><span class="sxs-lookup"><span data-stu-id="c9a2e-113">All outcome types have a regular and a published property appropriate to that type of outcome; for example, **points** and **publishedPoints**, **feedback** and **publishedFeedback**.</span></span>  <span data-ttu-id="c9a2e-114">A propriedade regular é o valor mais recente atualizado pelo professor; a propriedade publicada é o valor mais recente retornado ao aluno.</span><span class="sxs-lookup"><span data-stu-id="c9a2e-114">The regular property is the most recent value updated by the teacher; the published property is the most recent value returned to the student.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9a2e-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="c9a2e-115">Permissions</span></span>

<span data-ttu-id="c9a2e-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9a2e-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c9a2e-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9a2e-118">Permission type</span></span>                        | <span data-ttu-id="c9a2e-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c9a2e-119">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c9a2e-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9a2e-120">Delegated (work or school account)</span></span>     | <span data-ttu-id="c9a2e-121">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9a2e-121">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="c9a2e-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9a2e-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9a2e-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9a2e-123">Not supported.</span></span> |
| <span data-ttu-id="c9a2e-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9a2e-124">Application</span></span>                            | <span data-ttu-id="c9a2e-125">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9a2e-125">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9a2e-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9a2e-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/outcomes
```

## <a name="request-headers"></a><span data-ttu-id="c9a2e-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9a2e-127">Request headers</span></span>

| <span data-ttu-id="c9a2e-128">Nome</span><span class="sxs-lookup"><span data-stu-id="c9a2e-128">Name</span></span>      |<span data-ttu-id="c9a2e-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9a2e-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c9a2e-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9a2e-130">Authorization</span></span> | <span data-ttu-id="c9a2e-131">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="c9a2e-131">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9a2e-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9a2e-132">Request body</span></span>

<span data-ttu-id="c9a2e-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c9a2e-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9a2e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9a2e-134">Response</span></span>

<span data-ttu-id="c9a2e-135">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos educationOutcome](../resources/educationoutcome.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9a2e-135">If successful, this method returns a `200 OK` response code and a collection of [educationOutcome](../resources/educationoutcome.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c9a2e-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c9a2e-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c9a2e-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9a2e-137">Request</span></span>

<span data-ttu-id="c9a2e-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9a2e-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c9a2e-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9a2e-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outcomes"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/assignments/{id}/submissions/{id}/outcomes
```
# <a name="c"></a>[<span data-ttu-id="c9a2e-140">C#</span><span class="sxs-lookup"><span data-stu-id="c9a2e-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outcomes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c9a2e-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9a2e-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outcomes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9a2e-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9a2e-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outcomes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c9a2e-143">Java</span><span class="sxs-lookup"><span data-stu-id="c9a2e-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-outcomes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c9a2e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9a2e-144">Response</span></span>

<span data-ttu-id="c9a2e-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c9a2e-145">The following is an example of the response.</span></span>

> <span data-ttu-id="c9a2e-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c9a2e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationOutcome",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "@odata.type": "#microsoft.graph.educationFeedbackOutcome",
            "id": "ca05367a-b292-42d5-aff7-5d279feeace8",
            "feedback": {
                "feedbackDateTime": "2019-07-15T22:35:46.4847754Z",
                "text": {
                    "content": "This is feedback for the assignment as a whole.",
                    "contentType": "text"
                },
                "feedbackBy": {
                    "user": {
                        "id": "9391878d-903c-406c-bb1c-0f17d00fd878"
                    }
                }
            },
            "publishedFeedback": {
                "feedbackDateTime": "2019-07-15T22:35:46.4847754Z",
                "text": {
                    "content": "This is feedback for the assignment as a whole.",
                    "contentType": "text"
                },
                "feedbackBy": {
                    "user": {
                        "id": "9391878d-903c-406c-bb1c-0f17d00fd878"
                    }
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.educationPointsOutcome",
            "id": "ea1351f6-ba33-4940-b2cb-6a7254af2dc8",
            "points": {
                "gradedDateTime": "2019-07-15T22:36:02.2592364Z",
                "points": 75,
                "gradedBy": {
                    "user": {
                        "id": "9391878d-903c-406c-bb1c-0f17d00fd878"
                    }
                }
            },
            "publishedPoints": {
                "gradedDateTime": "2019-07-15T22:36:02.2592364Z",
                "points": 75,
                "gradedBy": {
                    "user": {
                        "id": "9391878d-903c-406c-bb1c-0f17d00fd878"
                    }
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.educationRubricOutcome",
            "id": "65a46d78-1a2b-4a7e-bcf8-78a22ac2611b",
            "rubricQualityFeedback": [
                {
                    "qualityId": "ebe97fd7-47f7-4e9a-b31b-221ad731fc5a",
                    "feedback": {
                        "content": "This is feedback specific to this quality of the rubric.",
                        "contentType": "text"
                    }
                },
                {
                    "qualityId": "bbf3fb4a-a794-4b51-a1ad-c22fb891c5d8",
                    "feedback": {
                        "content": "This is feedback specific to this quality of the rubric.",
                        "contentType": "text"
                    }
                }
            ],
            "rubricQualitySelectedLevels": [
                {
                    "qualityId": "ebe97fd7-47f7-4e9a-b31b-221ad731fc5a",
                    "columnId": "db2a0c91-abef-44cb-b8b1-ef1f85ef4a77"
                },
                {
                    "qualityId": "bbf3fb4a-a794-4b51-a1ad-c22fb891c5d8",
                    "columnId": "519cd134-c513-40b9-aa71-fdb0d063c084"
                }
            ],
            "publishedRubricQualityFeedback": [
                {
                    "qualityId": "ebe97fd7-47f7-4e9a-b31b-221ad731fc5a",
                    "feedback": {
                        "content": "This is feedback specific to this quality of the rubric.",
                        "contentType": "text"
                    }
                },
                {
                    "qualityId": "bbf3fb4a-a794-4b51-a1ad-c22fb891c5d8",
                    "feedback": {
                        "content": "This is feedback specific to this quality of the rubric.",
                        "contentType": "text"
                    }
                }
            ],
            "publishedRubricQualitySelectedLevels": [
                {
                    "qualityId": "ebe97fd7-47f7-4e9a-b31b-221ad731fc5a",
                    "columnId": "db2a0c91-abef-44cb-b8b1-ef1f85ef4a77"
                },
                {
                    "qualityId": "bbf3fb4a-a794-4b51-a1ad-c22fb891c5d8",
                    "columnId": "519cd134-c513-40b9-aa71-fdb0d063c084"
                }
            ]
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List outcomes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


