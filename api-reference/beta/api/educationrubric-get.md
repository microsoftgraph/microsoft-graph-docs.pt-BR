---
title: Obter educationRubric
description: Recupere as propriedades e os relacionamentos de um objeto educationrubric.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c5454d52d30b6174cfbb5a387fea0d115d4981a4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002399"
---
# <a name="get-educationrubric"></a><span data-ttu-id="1c5cb-103">Obter educationRubric</span><span class="sxs-lookup"><span data-stu-id="1c5cb-103">Get educationRubric</span></span>

<span data-ttu-id="1c5cb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c5cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c5cb-105">Recupere as propriedades e os relacionamentos de um objeto [educationRubric](../resources/educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="1c5cb-105">Retrieve the properties and relationships of an [educationRubric](../resources/educationrubric.md) object.</span></span>

<span data-ttu-id="1c5cb-106">Observe que ao obter o amostra rubric de uma atribuição ( `GET /education/me/assignments/{id}/rubric` ), o que é retornado é uma cópia imutável do amostra rubric original existente em `/education/users/{id}/rubrics` .</span><span class="sxs-lookup"><span data-stu-id="1c5cb-106">Note that when getting the rubric of an assignment (`GET /education/me/assignments/{id}/rubric`), what is returned is an immutable copy of the original rubric that exists under `/education/users/{id}/rubrics`.</span></span> <span data-ttu-id="1c5cb-107">A cópia é associada a essa atribuição específica.</span><span class="sxs-lookup"><span data-stu-id="1c5cb-107">The copy is associated with that specific assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c5cb-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c5cb-108">Permissions</span></span>

<span data-ttu-id="1c5cb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c5cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1c5cb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c5cb-111">Permission type</span></span>                        | <span data-ttu-id="1c5cb-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1c5cb-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1c5cb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c5cb-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c5cb-114">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c5cb-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="1c5cb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c5cb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c5cb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c5cb-116">Not supported.</span></span> |
| <span data-ttu-id="1c5cb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c5cb-117">Application</span></span>                            | <span data-ttu-id="1c5cb-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c5cb-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c5cb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c5cb-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me/rubrics/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1c5cb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c5cb-120">Request headers</span></span>

| <span data-ttu-id="1c5cb-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1c5cb-121">Name</span></span>      |<span data-ttu-id="1c5cb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c5cb-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1c5cb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c5cb-123">Authorization</span></span> | <span data-ttu-id="1c5cb-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="1c5cb-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c5cb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c5cb-125">Request body</span></span>

<span data-ttu-id="1c5cb-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c5cb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c5cb-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c5cb-127">Response</span></span>

<span data-ttu-id="1c5cb-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [educationRubric](../resources/educationrubric.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c5cb-128">If successful, this method returns a `200 OK` response code and the requested [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1c5cb-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1c5cb-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1c5cb-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c5cb-130">Request</span></span>

<span data-ttu-id="1c5cb-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c5cb-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1c5cb-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c5cb-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationrubric"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/rubrics/{id}
```
# <a name="c"></a>[<span data-ttu-id="1c5cb-133">C#</span><span class="sxs-lookup"><span data-stu-id="1c5cb-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationrubric-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c5cb-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c5cb-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationrubric-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c5cb-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c5cb-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationrubric-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1c5cb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c5cb-136">Response</span></span>

<span data-ttu-id="1c5cb-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1c5cb-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="1c5cb-138">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1c5cb-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1c5cb-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c5cb-139">All the properties will be returned from an actual call.</span></span>

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


