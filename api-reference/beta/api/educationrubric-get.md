---
title: Obter educationRubric
description: Recupere as propriedades e as relações de um objeto educationrubric.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 70f151e34c2768dc90526d0bd17ae476ffc7e459
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231417"
---
# <a name="get-educationrubric"></a><span data-ttu-id="b000c-103">Obter educationRubric</span><span class="sxs-lookup"><span data-stu-id="b000c-103">Get educationRubric</span></span>

<span data-ttu-id="b000c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b000c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b000c-105">Recupere as propriedades e as relações de um [objeto educationRubric.](../resources/educationrubric.md)</span><span class="sxs-lookup"><span data-stu-id="b000c-105">Retrieve the properties and relationships of an [educationRubric](../resources/educationrubric.md) object.</span></span>

<span data-ttu-id="b000c-106">Observe que, ao obter a rubrica de uma atribuição ( ), o que é retornado é uma cópia imutável da rubrica original que `GET /education/classes/{id}/assignments/{id}/rubric` existe em `/education/users/{id}/rubrics` .</span><span class="sxs-lookup"><span data-stu-id="b000c-106">Note that when getting the rubric of an assignment (`GET /education/classes/{id}/assignments/{id}/rubric`), what is returned is an immutable copy of the original rubric that exists under `/education/users/{id}/rubrics`.</span></span> <span data-ttu-id="b000c-107">A cópia está associada a essa atribuição específica.</span><span class="sxs-lookup"><span data-stu-id="b000c-107">The copy is associated with that specific assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="b000c-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="b000c-108">Permissions</span></span>

<span data-ttu-id="b000c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b000c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b000c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b000c-111">Permission type</span></span>                        | <span data-ttu-id="b000c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b000c-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b000c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b000c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b000c-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b000c-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="b000c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b000c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b000c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b000c-116">Not supported.</span></span> |
| <span data-ttu-id="b000c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b000c-117">Application</span></span>                            | <span data-ttu-id="b000c-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b000c-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b000c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b000c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me/rubrics/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b000c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b000c-120">Request headers</span></span>

| <span data-ttu-id="b000c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b000c-121">Name</span></span>      |<span data-ttu-id="b000c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b000c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b000c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b000c-123">Authorization</span></span> | <span data-ttu-id="b000c-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="b000c-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b000c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b000c-125">Request body</span></span>

<span data-ttu-id="b000c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b000c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b000c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b000c-127">Response</span></span>

<span data-ttu-id="b000c-128">Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [educationRubric](../resources/educationrubric.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b000c-128">If successful, this method returns a `200 OK` response code and the requested [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b000c-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b000c-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b000c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b000c-130">Request</span></span>

<span data-ttu-id="b000c-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b000c-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b000c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b000c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationrubric"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/rubrics/{id}
```
# <a name="c"></a>[<span data-ttu-id="b000c-133">C#</span><span class="sxs-lookup"><span data-stu-id="b000c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationrubric-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b000c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b000c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationrubric-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b000c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b000c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationrubric-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b000c-136">Java</span><span class="sxs-lookup"><span data-stu-id="b000c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationrubric-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b000c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b000c-137">Response</span></span>

<span data-ttu-id="b000c-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b000c-138">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="b000c-139">O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="b000c-139">The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric"
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
  "description": "Get educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


