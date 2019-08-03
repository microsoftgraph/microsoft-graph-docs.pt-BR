---
title: Obter educationRubric
description: Recupere as propriedades e os relacionamentos de um objeto educationrubric.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6306caf95dc4de199cb2f056c28469c1da5274c1
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173143"
---
# <a name="get-educationrubric"></a><span data-ttu-id="db914-103">Obter educationRubric</span><span class="sxs-lookup"><span data-stu-id="db914-103">Get educationRubric</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db914-104">Recupere as propriedades e os relacionamentos de um objeto [educationRubric](../resources/educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="db914-104">Retrieve the properties and relationships of an [educationRubric](../resources/educationrubric.md) object.</span></span>

<span data-ttu-id="db914-105">Observe que ao obter o amostra rubric de uma atribuição (`GET /education/me/assignments/{id}/rubric`), o que é retornado é uma cópia imutável do amostra rubric original existente em `/education/users/{id}/rubrics`.</span><span class="sxs-lookup"><span data-stu-id="db914-105">Note that when getting the rubric of an assignment (`GET /education/me/assignments/{id}/rubric`), what is returned is an immutable copy of the original rubric that exists under `/education/users/{id}/rubrics`.</span></span> <span data-ttu-id="db914-106">A cópia é associada a essa atribuição específica.</span><span class="sxs-lookup"><span data-stu-id="db914-106">The copy is associated with that specific assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="db914-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="db914-107">Permissions</span></span>

<span data-ttu-id="db914-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db914-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db914-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db914-110">Permission type</span></span>                        | <span data-ttu-id="db914-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="db914-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="db914-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db914-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="db914-113">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db914-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="db914-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db914-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db914-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db914-115">Not supported.</span></span> |
| <span data-ttu-id="db914-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db914-116">Application</span></span>                            | <span data-ttu-id="db914-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db914-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="db914-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db914-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me/rubrics/{id}
```

## <a name="request-headers"></a><span data-ttu-id="db914-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db914-119">Request headers</span></span>

| <span data-ttu-id="db914-120">Nome</span><span class="sxs-lookup"><span data-stu-id="db914-120">Name</span></span>      |<span data-ttu-id="db914-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="db914-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="db914-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="db914-122">Authorization</span></span> | <span data-ttu-id="db914-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="db914-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="db914-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db914-124">Request body</span></span>

<span data-ttu-id="db914-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="db914-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db914-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="db914-126">Response</span></span>

<span data-ttu-id="db914-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [educationRubric](../resources/educationrubric.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db914-127">If successful, this method returns a `200 OK` response code and the requested [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="db914-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="db914-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="db914-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db914-129">Request</span></span>

<span data-ttu-id="db914-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="db914-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationrubric"
}-->

```http
GET https://graph.microsoft.com/beta/education/me/rubrics/{id}
```

### <a name="response"></a><span data-ttu-id="db914-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="db914-131">Response</span></span>

<span data-ttu-id="db914-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="db914-132">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="db914-133">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="db914-133">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="db914-134">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db914-134">All the properties will be returned from an actual call.</span></span>

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
