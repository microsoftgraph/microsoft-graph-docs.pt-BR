---
title: Criar educationRubric
description: Criar um novo objeto educationRubric.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b36bbf9d8f463cef1fa56cc91d2f03862bc83379
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981104"
---
# <a name="create-educationrubric"></a><span data-ttu-id="32f00-103">Criar educationRubric</span><span class="sxs-lookup"><span data-stu-id="32f00-103">Create educationRubric</span></span>

<span data-ttu-id="32f00-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32f00-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32f00-105">Criar um novo objeto [educationRubric](../resources/educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="32f00-105">Create a new [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="32f00-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="32f00-106">Permissions</span></span>

<span data-ttu-id="32f00-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32f00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="32f00-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32f00-109">Permission type</span></span>                        | <span data-ttu-id="32f00-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="32f00-110">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="32f00-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32f00-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="32f00-112">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32f00-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="32f00-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32f00-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32f00-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32f00-114">Not supported.</span></span>                                          |
| <span data-ttu-id="32f00-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32f00-115">Application</span></span>                            | <span data-ttu-id="32f00-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32f00-116">Not supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="32f00-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32f00-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /education/me/rubrics
```

## <a name="request-headers"></a><span data-ttu-id="32f00-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32f00-118">Request headers</span></span>

| <span data-ttu-id="32f00-119">Nome</span><span class="sxs-lookup"><span data-stu-id="32f00-119">Name</span></span>          | <span data-ttu-id="32f00-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="32f00-120">Description</span></span>    |
| :------------ | :------------- |
| <span data-ttu-id="32f00-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="32f00-121">Authorization</span></span> | <span data-ttu-id="32f00-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="32f00-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="32f00-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32f00-123">Request body</span></span>

<span data-ttu-id="32f00-124">No corpo da solicitação, forneça uma representação JSON de um objeto [educationRubric](../resources/educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="32f00-124">In the request body, supply a JSON representation of an [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="32f00-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="32f00-125">Response</span></span>

<span data-ttu-id="32f00-126">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um novo objeto [educationRubric](../resources/educationrubric.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32f00-126">If successful, this method returns `201 Created` response code and a new [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="32f00-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="32f00-127">Examples</span></span>

### <a name="example-1-posting-a-credit-rubric"></a><span data-ttu-id="32f00-128">Exemplo 1: postando um amostra rubric de crédito</span><span class="sxs-lookup"><span data-stu-id="32f00-128">Example 1: Posting a Credit Rubric</span></span>

#### <a name="request"></a><span data-ttu-id="32f00-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32f00-129">Request</span></span>

<span data-ttu-id="32f00-130">Veja a seguir um exemplo da solicitação para postar um amostra rubric de crédito (um amostra rubric sem pontos).</span><span class="sxs-lookup"><span data-stu-id="32f00-130">The following is an example of the request to post a credit rubric (a rubric with no points).</span></span>

# <a name="http"></a>[<span data-ttu-id="32f00-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="32f00-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationrubric_from_educationuser"
}-->

```http
POST https://graph.microsoft.com/beta/education/me/rubrics
Content-type: application/json

{
    "displayName":"Example Credit Rubric",
    "description":{
        "content":"This is an example of a credit rubric (no points)",
        "contentType":"text"
    },
    "levels":[
        {
            "displayName":"Good",
            "description":{
                "content":"",
                "contentType":"text"
            }
        },
        {
            "displayName":"Poor",
            "description":{
                "content":"",
                "contentType":"text"
            }
        }
    ],
    "qualities":[
        {
            "description":{
                "content":"Argument",
                "contentType":"text"
            },
            "criteria":[
                {
                    "description":{
                        "content":"The essay's argument is persuasive.",
                        "contentType":"text"
                    }
                },
                {
                    "description":{
                        "content":"The essay's argument does not make sense.",
                        "contentType":"text"
                    }
                }
            ]
        },
        {
            "description":{
                "content":"Spelling and Grammar",
                "contentType":"text"
            },
            "criteria":[
                {
                    "description":{
                        "content":"The essay uses proper spelling and grammar with few or no errors.",
                        "contentType":"text"
                    }
                },
                {
                    "description":{
                        "content":"The essay has numerous errors in spelling and/or grammar.",
                        "contentType":"text"
                    }
                }
            ]
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="32f00-132">C#</span><span class="sxs-lookup"><span data-stu-id="32f00-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationrubric-from-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32f00-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32f00-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationrubric-from-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32f00-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32f00-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationrubric-from-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="32f00-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="32f00-135">Response</span></span>

<span data-ttu-id="32f00-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="32f00-136">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="32f00-137">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="32f00-137">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="32f00-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32f00-138">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "displayName": "Example Credit Rubric",
    "id": "63618139-2e8d-4f56-a762-dd734736816f",
    "description": {
        "content": "This is an example of a credit rubric (no points)",
        "contentType": "text"
    },
    "qualities": [
        {
            "qualityId": "461e866a-4844-4a3f-9a3c-e5464a32acf1",
            "description": {
                "content": "Argument",
                "contentType": "text"
            },
            "criteria": [
                {
                    "description": {
                        "content": "The essay's argument is persuasive.",
                        "contentType": "text"
                    }
                },
                {
                    "description": {
                        "content": "The essay's argument does not make sense.",
                        "contentType": "text"
                    }
                }
            ]
        },
        {
            "qualityId": "ccb47c1c-1a01-4027-93d7-f14b9fe86fdd",
            "description": {
                "content": "Spelling and Grammar",
                "contentType": "text"
            },
            "criteria": [
                {
                    "description": {
                        "content": "The essay uses proper spelling and grammar with few or no errors.",
                        "contentType": "text"
                    }
                },
                {
                    "description": {
                        "content": "The essay has numerous errors in spelling and/or grammar.",
                        "contentType": "text"
                    }
                }
            ]
        }
    ],
    "levels": [
        {
            "levelId": "564e68f6-984b-4574-bea7-ffae3c92633f",
            "displayName": "Good",
            "description": {
                "content": "",
                "contentType": "text"
            }
        },
        {
            "levelId": "3f082e35-46e3-4944-baea-ea6c7e36ef37",
            "displayName": "Poor",
            "description": {
                "content": "",
                "contentType": "text"
            }
        }
    ]
}
```

### <a name="example-2-posting-a-points-rubric"></a><span data-ttu-id="32f00-139">Exemplo 2: lançamento de pontos amostra rubric</span><span class="sxs-lookup"><span data-stu-id="32f00-139">Example 2: Posting a Points Rubric</span></span>

<span data-ttu-id="32f00-140">Veja a seguir um exemplo da solicitação para postar um amostra rubric com pontos.</span><span class="sxs-lookup"><span data-stu-id="32f00-140">The following is an example of the request to post a rubric with points.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationrubric_from_educationuser"
}-->

```http
POST https://graph.microsoft.com/beta/education/me/rubrics
Content-type: application/json

{
    "displayName":"Example Points Rubric",
    "description":{
        "content":"This is an example of a rubric with points",
        "contentType":"text"
    },
    "levels":[
        {
            "displayName":"Good",
            "description":{
                "content":"",
                "contentType":"text"
            },
            "grading":{
                "@odata.type":"#microsoft.graph.educationAssignmentPointsGradeType",
                "maxPoints":2
            }
        },
        {
            "displayName":"Poor",
            "description":{
                "content":"",
                "contentType":"text"
            },
            "grading":{
                "@odata.type":"#microsoft.graph.educationAssignmentPointsGradeType",
                "maxPoints":1
            }
        }
    ],
    "qualities":[
        {
            "description":{
                "content":"Argument",
                "contentType":"text"
            },
            "criteria":[
                {
                    "description":{
                        "content":"The essay's argument is persuasive.",
                        "contentType":"text"
                    }
                },
                {
                    "description":{
                        "content":"The essay's argument does not make sense.",
                        "contentType":"text"
                    }
                }
            ],
            "weight":50.0
        },
        {
            "description":{
                "content":"Spelling and Grammar",
                "contentType":"text"
            },
            "criteria":[
                {
                    "description":{
                        "content":"The essay uses proper spelling and grammar with few or no errors.",
                        "contentType":"text"
                    }
                },
                {
                    "description":{
                        "content":"The essay has numerous errors in spelling and/or grammar.",
                        "contentType":"text"
                    }
                }
            ],
            "weight":50.0
        }
    ],
    "grading":{
        "@odata.type":"#microsoft.graph.educationAssignmentPointsGradeType"
    }
}
```

#### <a name="response"></a><span data-ttu-id="32f00-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="32f00-141">Response</span></span>

<span data-ttu-id="32f00-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="32f00-142">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="32f00-143">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="32f00-143">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="32f00-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32f00-144">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "displayName": "Example Points Rubric",
    "id": "bf040af7-a5ff-4abe-a8c8-1bdc532344c2",
    "description": {
        "content": "This is an example of a rubric with points",
        "contentType": "text"
    },
    "levels": [
        {
            "levelId": "519cd134-c513-40b9-aa71-fdb0d063c084",
            "displayName": "Good",
            "description": {
                "content": "",
                "contentType": "text"
            },
            "grading": {
                "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
                "maxPoints": 2
            }
        },
        {
            "levelId": "db2a0c91-abef-44cb-b8b1-ef1f85ef4a77",
            "displayName": "Poor",
            "description": {
                "content": "",
                "contentType": "text"
            },
            "grading": {
                "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
                "maxPoints": 1
            }
        }
    ],
    "qualities": [
        {
            "qualityId": "bbf3fb4a-a794-4b51-a1ad-c22fb891c5d8",
            "weight": 50.0,
            "description": {
                "content": "Argument",
                "contentType": "text"
            },
            "criteria": [
                {
                    "id": "5e637d79-f26b-4ea6-acd7-73824f0c0967",
                    "description": {
                        "content": "The essay's argument is persuasive.",
                        "contentType": "text"
                    }
                },
                {
                    "id": "ebdcc27f-d1ec-4aa3-9da7-bd8d7842e3d3",
                    "description": {
                        "content": "The essay's argument does not make sense.",
                        "contentType": "text"
                    }
                }
            ]
        },
        {
            "qualityId": "ebe97fd7-47f7-4e9a-b31b-221ad731fc5a",
            "weight": 50.0,
            "description": {
                "content": "Spelling and Grammar",
                "contentType": "text"
            },
            "criteria": [
                {
                    "id": "5417252a-f810-41eb-9a83-09276a258a08",
                    "description": {
                        "content": "The essay uses proper spelling and grammar with few or no errors.",
                        "contentType": "text"
                    }
                },
                {
                    "id": "5de220bd-74b9-41a7-85d5-9be7c6cb7933",
                    "description": {
                        "content": "The essay has numerous errors in spelling and/or grammar.",
                        "contentType": "text"
                    }
                }
            ]
        }
    ],
    "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 100
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


