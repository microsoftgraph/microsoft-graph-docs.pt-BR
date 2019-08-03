---
title: Atualizar educationRubric
description: Atualize as propriedades do objeto educationRubric.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c1c900084c0410f583621b43b145ccd9934c820b
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173136"
---
# <a name="update-educationrubric"></a><span data-ttu-id="8aa4a-103">Atualizar educationRubric</span><span class="sxs-lookup"><span data-stu-id="8aa4a-103">Update educationRubric</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8aa4a-104">Atualiza as propriedades de um objeto [educationRubric](../resources/educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="8aa4a-104">Update the properties of an [educationRubric](../resources/educationrubric.md) object.</span></span>

<span data-ttu-id="8aa4a-105">A atualização de um amostra rubric anexado a uma`PATCH /education/me/assignments/{id}/rubric`atribuição () só é possível antes da atribuição ser publicada e o que é atualizado na verdade, o amostra rubric original `/education/users/{id}/rubrics`que existe em.</span><span class="sxs-lookup"><span data-stu-id="8aa4a-105">Updating a rubric attached to an assignment (`PATCH /education/me/assignments/{id}/rubric`) is only possible before the assignment is published, and what is updated is actually the original rubric that exists under `/education/users/{id}/rubrics`.</span></span> <span data-ttu-id="8aa4a-106">Depois que a atribuição é publicada, uma cópia imutável do amostra rubric é feita anexada a essa atribuição específica.</span><span class="sxs-lookup"><span data-stu-id="8aa4a-106">After the assignment is published, an immutable copy of the rubric is made that is attached to that specific assignment.</span></span> <span data-ttu-id="8aa4a-107">Esse amostra rubric pode ser recuperado usando [Get/Education/me/assignments/{ID}/rubric](educationrubric-get.md), mas não pode ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="8aa4a-107">That rubric can be retrieved using [GET /education/me/assignments/{id}/rubric](educationrubric-get.md), but it cannot be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="8aa4a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="8aa4a-108">Permissions</span></span>

<span data-ttu-id="8aa4a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8aa4a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8aa4a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8aa4a-111">Permission type</span></span>                        | <span data-ttu-id="8aa4a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8aa4a-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8aa4a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8aa4a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8aa4a-114">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8aa4a-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="8aa4a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8aa4a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8aa4a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8aa4a-116">Not supported.</span></span> |
| <span data-ttu-id="8aa4a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8aa4a-117">Application</span></span>                            | <span data-ttu-id="8aa4a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8aa4a-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8aa4a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8aa4a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /education/me/rubrics/{id}
PATCH /education/me/assignments/{id}/rubric
```

## <a name="request-headers"></a><span data-ttu-id="8aa4a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8aa4a-120">Request headers</span></span>

| <span data-ttu-id="8aa4a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8aa4a-121">Name</span></span>       | <span data-ttu-id="8aa4a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8aa4a-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8aa4a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8aa4a-123">Authorization</span></span> | <span data-ttu-id="8aa4a-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="8aa4a-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8aa4a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8aa4a-125">Request body</span></span>

<span data-ttu-id="8aa4a-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="8aa4a-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8aa4a-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="8aa4a-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8aa4a-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="8aa4a-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8aa4a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8aa4a-129">Property</span></span>     | <span data-ttu-id="8aa4a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8aa4a-130">Type</span></span>        | <span data-ttu-id="8aa4a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8aa4a-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8aa4a-132">description</span><span class="sxs-lookup"><span data-stu-id="8aa4a-132">description</span></span>|<span data-ttu-id="8aa4a-133">dobody</span><span class="sxs-lookup"><span data-stu-id="8aa4a-133">itemBody</span></span>|<span data-ttu-id="8aa4a-134">A descrição desse amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="8aa4a-134">The description of this rubric.</span></span>|
|<span data-ttu-id="8aa4a-135">displayName</span><span class="sxs-lookup"><span data-stu-id="8aa4a-135">displayName</span></span>|<span data-ttu-id="8aa4a-136">String</span><span class="sxs-lookup"><span data-stu-id="8aa4a-136">String</span></span>|<span data-ttu-id="8aa4a-137">O nome deste amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="8aa4a-137">The name of this rubric.</span></span>|
|<span data-ttu-id="8aa4a-138">notas</span><span class="sxs-lookup"><span data-stu-id="8aa4a-138">grading</span></span>|<span data-ttu-id="8aa4a-139">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="8aa4a-139">educationAssignmentGradeType</span></span>|<span data-ttu-id="8aa4a-140">Se este amostra rubric tem pontos ou não.</span><span class="sxs-lookup"><span data-stu-id="8aa4a-140">Whether this rubric has points or not.</span></span>|
|<span data-ttu-id="8aa4a-141">alcançar</span><span class="sxs-lookup"><span data-stu-id="8aa4a-141">levels</span></span>|<span data-ttu-id="8aa4a-142">coleção rubricLevel</span><span class="sxs-lookup"><span data-stu-id="8aa4a-142">rubricLevel collection</span></span>|<span data-ttu-id="8aa4a-143">A coleção de níveis que compõem este amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="8aa4a-143">The collection of levels making up this rubric.</span></span>|
|<span data-ttu-id="8aa4a-144">qualidades</span><span class="sxs-lookup"><span data-stu-id="8aa4a-144">qualities</span></span>|<span data-ttu-id="8aa4a-145">coleção rubricQuality</span><span class="sxs-lookup"><span data-stu-id="8aa4a-145">rubricQuality collection</span></span>|<span data-ttu-id="8aa4a-146">O conjunto de qualidades que compõem este amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="8aa4a-146">The collection of qualities making up this rubric.</span></span>|

## <a name="response"></a><span data-ttu-id="8aa4a-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="8aa4a-147">Response</span></span>

<span data-ttu-id="8aa4a-148">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [educationRubric](../resources/educationrubric.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8aa4a-148">If successful, this method returns a `200 OK` response code and an updated [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8aa4a-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8aa4a-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8aa4a-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8aa4a-150">Request</span></span>

<span data-ttu-id="8aa4a-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8aa4a-151">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationrubric"
}-->

```http
PATCH https://graph.microsoft.com/beta/education/me/rubrics/{id}
Content-type: application/json

{
  "displayName": "Example Credit Rubric after display name patch"
}
```

### <a name="response"></a><span data-ttu-id="8aa4a-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="8aa4a-152">Response</span></span>

<span data-ttu-id="8aa4a-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8aa4a-153">The following is an example of the response.</span></span>

> <span data-ttu-id="8aa4a-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8aa4a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
