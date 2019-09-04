---
title: Obter educationRubric anexados a educationAssignment
description: Obtenha o educaitonRubric anexado a um educationAssignment, se houver um.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7fd0524affaec2da6a9e21ef679dce539113d8b2
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36717990"
---
# <a name="get-educationrubric-attached-to-educationassignment"></a><span data-ttu-id="85776-103">Obter educationRubric anexados a educationAssignment</span><span class="sxs-lookup"><span data-stu-id="85776-103">Get educationRubric attached to educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85776-104">Obtenha o objeto [educationRubric](../resources/educationrubric.md) anexado a um [educationAssignment](../resources/educationassignment.md), se houver um.</span><span class="sxs-lookup"><span data-stu-id="85776-104">Get the [educationRubric](../resources/educationrubric.md) object attached to an [educationAssignment](../resources/educationassignment.md), if one exists.</span></span>

## <a name="permissions"></a><span data-ttu-id="85776-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="85776-105">Permissions</span></span>

<span data-ttu-id="85776-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85776-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="85776-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85776-108">Permission type</span></span>                        | <span data-ttu-id="85776-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="85776-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="85776-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85776-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="85776-111">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85776-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="85776-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85776-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85776-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85776-113">Not supported.</span></span> |
| <span data-ttu-id="85776-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85776-114">Application</span></span>                            | <span data-ttu-id="85776-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85776-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="85776-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85776-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/classes/{id}/assignments/{id}/rubric
```

## <a name="request-headers"></a><span data-ttu-id="85776-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85776-117">Request headers</span></span>

| <span data-ttu-id="85776-118">Nome</span><span class="sxs-lookup"><span data-stu-id="85776-118">Name</span></span>      |<span data-ttu-id="85776-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="85776-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="85776-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="85776-120">Authorization</span></span> | <span data-ttu-id="85776-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="85776-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="85776-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85776-122">Request body</span></span>

<span data-ttu-id="85776-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="85776-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85776-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="85776-124">Response</span></span>

<span data-ttu-id="85776-125">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [educationRubric](../resources/educationrubric.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85776-125">If successful, this method returns a `200 OK` response code and an [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="85776-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="85776-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="85776-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85776-127">Request</span></span>

<span data-ttu-id="85776-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="85776-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="85776-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="85776-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rubric"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/assignments/{id}/rubric
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="85776-130">C#</span><span class="sxs-lookup"><span data-stu-id="85776-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rubric-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="85776-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85776-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rubric-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="85776-132">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="85776-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rubric-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="85776-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="85776-133">Response</span></span>

<span data-ttu-id="85776-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="85776-134">The following is an example of the response.</span></span>

> <span data-ttu-id="85776-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="85776-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
