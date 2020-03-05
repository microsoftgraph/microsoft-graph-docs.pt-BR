---
title: Obter educationRubric anexados a educationAssignment
description: Obtenha o educaitonRubric anexado a um educationAssignment, se houver um.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ad4e72c2d638e1b07aa1ef363f8d0c406ef9b4bd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42427652"
---
# <a name="get-educationrubric-attached-to-educationassignment"></a><span data-ttu-id="8bb2b-103">Obter educationRubric anexados a educationAssignment</span><span class="sxs-lookup"><span data-stu-id="8bb2b-103">Get educationRubric attached to educationAssignment</span></span>

<span data-ttu-id="8bb2b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8bb2b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bb2b-105">Obtenha o objeto [educationRubric](../resources/educationrubric.md) anexado a um [educationAssignment](../resources/educationassignment.md), se houver um.</span><span class="sxs-lookup"><span data-stu-id="8bb2b-105">Get the [educationRubric](../resources/educationrubric.md) object attached to an [educationAssignment](../resources/educationassignment.md), if one exists.</span></span>

## <a name="permissions"></a><span data-ttu-id="8bb2b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8bb2b-106">Permissions</span></span>

<span data-ttu-id="8bb2b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bb2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8bb2b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8bb2b-109">Permission type</span></span>                        | <span data-ttu-id="8bb2b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8bb2b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8bb2b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8bb2b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8bb2b-112">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8bb2b-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="8bb2b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8bb2b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bb2b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8bb2b-114">Not supported.</span></span> |
| <span data-ttu-id="8bb2b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8bb2b-115">Application</span></span>                            | <span data-ttu-id="8bb2b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8bb2b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bb2b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8bb2b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/classes/{id}/assignments/{id}/rubric
```

## <a name="request-headers"></a><span data-ttu-id="8bb2b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8bb2b-118">Request headers</span></span>

| <span data-ttu-id="8bb2b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8bb2b-119">Name</span></span>      |<span data-ttu-id="8bb2b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8bb2b-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8bb2b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8bb2b-121">Authorization</span></span> | <span data-ttu-id="8bb2b-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="8bb2b-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8bb2b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8bb2b-123">Request body</span></span>

<span data-ttu-id="8bb2b-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8bb2b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8bb2b-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bb2b-125">Response</span></span>

<span data-ttu-id="8bb2b-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [educationRubric](../resources/educationrubric.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8bb2b-126">If successful, this method returns a `200 OK` response code and an [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8bb2b-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8bb2b-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8bb2b-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8bb2b-128">Request</span></span>

<span data-ttu-id="8bb2b-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8bb2b-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8bb2b-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="8bb2b-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rubric"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/assignments/{id}/rubric
```
# <a name="c"></a>[<span data-ttu-id="8bb2b-131">C#</span><span class="sxs-lookup"><span data-stu-id="8bb2b-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rubric-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8bb2b-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8bb2b-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rubric-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8bb2b-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8bb2b-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rubric-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8bb2b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bb2b-134">Response</span></span>

<span data-ttu-id="8bb2b-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8bb2b-135">The following is an example of the response.</span></span>

> <span data-ttu-id="8bb2b-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8bb2b-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
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
  "description": "List rubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
