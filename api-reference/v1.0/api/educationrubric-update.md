---
title: Atualizar educationRubric
description: Atualize as propriedades do objeto educationRubric.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 57a1565cb699f4d0c1a997cbf8563c6d8e32f210
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912152"
---
# <a name="update-educationrubric"></a><span data-ttu-id="f334f-103">Atualizar educationRubric</span><span class="sxs-lookup"><span data-stu-id="f334f-103">Update educationRubric</span></span>

<span data-ttu-id="f334f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f334f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f334f-105">Atualize as propriedades de um [objeto educationRubric.](../resources/educationrubric.md)</span><span class="sxs-lookup"><span data-stu-id="f334f-105">Update the properties of an [educationRubric](../resources/educationrubric.md) object.</span></span>

<span data-ttu-id="f334f-106">A atualização de uma rubrica anexada a uma atribuição ( ) só é possível antes da atribuição ser publicada, e o que é atualizado na verdade é a rubrica original que existe `PATCH /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/rubric` em `/education/users/{id}/rubrics` .</span><span class="sxs-lookup"><span data-stu-id="f334f-106">Updating a rubric attached to an assignment (`PATCH /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/rubric`) is only possible before the assignment is published, and what is updated is actually the original rubric that exists under `/education/users/{id}/rubrics`.</span></span> <span data-ttu-id="f334f-107">Depois que a atribuição for publicada, será feita uma cópia imutável da rubrica anexada a essa atribuição específica.</span><span class="sxs-lookup"><span data-stu-id="f334f-107">After the assignment is published, an immutable copy of the rubric is made that is attached to that specific assignment.</span></span> <span data-ttu-id="f334f-108">Essa rubrica pode ser recuperada usando [GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/rubric](educationrubric-get.md), mas não pode ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="f334f-108">That rubric can be retrieved using [GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/rubric](educationrubric-get.md), but it cannot be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="f334f-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="f334f-109">Permissions</span></span>

<span data-ttu-id="f334f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f334f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f334f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f334f-112">Permission type</span></span>                        | <span data-ttu-id="f334f-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f334f-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f334f-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f334f-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="f334f-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f334f-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="f334f-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f334f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f334f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f334f-117">Not supported.</span></span> |
| <span data-ttu-id="f334f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f334f-118">Application</span></span>                            | <span data-ttu-id="f334f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f334f-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f334f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f334f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /education/me/rubrics/ceb3863e-6912-4ea9-ac41-3c2bb7b6672d
PATCH /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/rubric
```

## <a name="request-headers"></a><span data-ttu-id="f334f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f334f-121">Request headers</span></span>

| <span data-ttu-id="f334f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f334f-122">Name</span></span>       | <span data-ttu-id="f334f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f334f-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f334f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f334f-124">Authorization</span></span> | <span data-ttu-id="f334f-125">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="f334f-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f334f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f334f-126">Request body</span></span>

<span data-ttu-id="f334f-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="f334f-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f334f-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="f334f-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f334f-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f334f-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f334f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f334f-130">Property</span></span>     | <span data-ttu-id="f334f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f334f-131">Type</span></span>        | <span data-ttu-id="f334f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f334f-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f334f-133">description</span><span class="sxs-lookup"><span data-stu-id="f334f-133">description</span></span>|<span data-ttu-id="f334f-134">itemBody</span><span class="sxs-lookup"><span data-stu-id="f334f-134">itemBody</span></span>|<span data-ttu-id="f334f-135">A descrição dessa rubrica.</span><span class="sxs-lookup"><span data-stu-id="f334f-135">The description of this rubric.</span></span>|
|<span data-ttu-id="f334f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f334f-136">displayName</span></span>|<span data-ttu-id="f334f-137">String</span><span class="sxs-lookup"><span data-stu-id="f334f-137">String</span></span>|<span data-ttu-id="f334f-138">O nome dessa rubrica.</span><span class="sxs-lookup"><span data-stu-id="f334f-138">The name of this rubric.</span></span>|
|<span data-ttu-id="f334f-139">grading</span><span class="sxs-lookup"><span data-stu-id="f334f-139">grading</span></span>|<span data-ttu-id="f334f-140">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="f334f-140">educationAssignmentGradeType</span></span>|<span data-ttu-id="f334f-141">Se essa rubrica tem pontos ou não.</span><span class="sxs-lookup"><span data-stu-id="f334f-141">Whether this rubric has points or not.</span></span>|
|<span data-ttu-id="f334f-142">levels</span><span class="sxs-lookup"><span data-stu-id="f334f-142">levels</span></span>|<span data-ttu-id="f334f-143">Coleção rubricLevel</span><span class="sxs-lookup"><span data-stu-id="f334f-143">rubricLevel collection</span></span>|<span data-ttu-id="f334f-144">A coleção de níveis que comem essa rubrica.</span><span class="sxs-lookup"><span data-stu-id="f334f-144">The collection of levels making up this rubric.</span></span>|
|<span data-ttu-id="f334f-145">qualidades</span><span class="sxs-lookup"><span data-stu-id="f334f-145">qualities</span></span>|<span data-ttu-id="f334f-146">Coleção rubricQuality</span><span class="sxs-lookup"><span data-stu-id="f334f-146">rubricQuality collection</span></span>|<span data-ttu-id="f334f-147">A coleção de qualidades que com isso é rubrica.</span><span class="sxs-lookup"><span data-stu-id="f334f-147">The collection of qualities making up this rubric.</span></span>|

## <a name="response"></a><span data-ttu-id="f334f-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="f334f-148">Response</span></span>

<span data-ttu-id="f334f-149">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationRubric](../resources/educationrubric.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f334f-149">If successful, this method returns a `200 OK` response code and an updated [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f334f-150">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f334f-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f334f-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f334f-151">Request</span></span>

<span data-ttu-id="f334f-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f334f-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_educationrubric"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/education/me/rubrics/ceb3863e-6912-4ea9-ac41-3c2bb7b6672d
Content-type: application/json

{
  "displayName": "Example Credit Rubric after display name patch"
}
```

### <a name="response"></a><span data-ttu-id="f334f-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="f334f-153">Response</span></span>

<span data-ttu-id="f334f-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f334f-154">The following is an example of the response.</span></span>

> <span data-ttu-id="f334f-155">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f334f-155">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "displayName": "Example Credit Rubric after display name patch",
    "id": "c4459fcb-a761-4f70-ac5b-e9466cb77c2a",
    "description": {
        "content": "This is an example of a credit rubric (no points)",
        "contentType": "text"
    },
    "levels": [
        {
            "levelId": "dec665d4-cf1b-4481-ac61-1d5b6188f4f5",
            "displayName": "Good",
            "description": {
                "content": "",
                "contentType": "text"
            }
        },
        {
            "levelId": "3f2e4b0f-508e-4005-984b-17e061bc5377",
            "displayName": "Poor",
            "description": {
                "content": "",
                "contentType": "text"
            }
        }
    ],
    "qualities": [
        {
            "qualityId": "dc79dcbf-b536-4797-9c5b-902f28129fd0",
            "description": {
                "content": "Argument",
                "contentType": "text"
            },
            "criteria": [
                {
                    "id": "8937fa15-4a7c-4f27-bd01-ca3471d2d1d5",
                    "description": {
                        "content": "The essay's argument is persuasive.",
                        "contentType": "text"
                    }
                },
                {
                    "id": "4dfb5263-1d3f-4f0a-93ef-d24d800d0f69",
                    "description": {
                        "content": "The essay's argument does not make sense.",
                        "contentType": "text"
                    }
                }
            ]
        },
        {
            "qualityId": "7e087062-ac25-4629-8386-a946350936db",
            "description": {
                "content": "Spelling and Grammar",
                "contentType": "text"
            },
            "criteria": [
                {
                    "id": "12276eb2-122c-4ad2-ba92-335ea798c88e",
                    "description": {
                        "content": "The essay uses proper spelling and grammar with few or no errors.",
                        "contentType": "text"
                    }
                },
                {
                    "id": "3db7e6b2-2b1b-4f8e-9fca-bea701159145",
                    "description": {
                        "content": "The essay has numerous errors in spelling and/or grammar.",
                        "contentType": "text"
                    }
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
  "description": "Update educationrubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


