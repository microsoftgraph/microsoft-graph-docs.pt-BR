---
title: Anexar educationRubric a educationAssignment
description: Anexar um objeto educationRubric existente a um educationAssignment.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 84a0f60edfa292776291e823538c45ae7e7d5898
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461137"
---
# <a name="create-educationrubric"></a><span data-ttu-id="885fc-103">Criar educationRubric</span><span class="sxs-lookup"><span data-stu-id="885fc-103">Create educationRubric</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="885fc-104">Anexar um objeto [educationRubric](../resources/educationrubric.md) existente a um [educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="885fc-104">Attach an existing [educationRubric](../resources/educationrubric.md) object to an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="885fc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="885fc-105">Permissions</span></span>

<span data-ttu-id="885fc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="885fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="885fc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="885fc-108">Permission type</span></span>                        | <span data-ttu-id="885fc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="885fc-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="885fc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="885fc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="885fc-111">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="885fc-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="885fc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="885fc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="885fc-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="885fc-113">Not supported.</span></span> |
| <span data-ttu-id="885fc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="885fc-114">Application</span></span>                            | <span data-ttu-id="885fc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="885fc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="885fc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="885fc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /education/classes/{id}/assignments/{id}/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="885fc-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="885fc-117">Request headers</span></span>

| <span data-ttu-id="885fc-118">Nome</span><span class="sxs-lookup"><span data-stu-id="885fc-118">Name</span></span>          | <span data-ttu-id="885fc-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="885fc-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="885fc-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="885fc-120">Authorization</span></span> | <span data-ttu-id="885fc-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="885fc-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="885fc-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="885fc-122">Request body</span></span>

<span data-ttu-id="885fc-123">No corpo da solicitação, forneça a ID de OData de um objeto [educationRubric](../resources/educationrubric.md) existente.</span><span class="sxs-lookup"><span data-stu-id="885fc-123">In the request body, supply the OData ID of an existing [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="885fc-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="885fc-124">Response</span></span>

<span data-ttu-id="885fc-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="885fc-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="885fc-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="885fc-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="885fc-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="885fc-128">Request</span></span>

<span data-ttu-id="885fc-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="885fc-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="885fc-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="885fc-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationrubric_from_educationassignment"
}-->

```http
PUT https://graph.microsoft.com/beta/education/classes/{id}/assignments/{id}/rubric/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/education/me/rubrics/{id}"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="885fc-131">C#</span><span class="sxs-lookup"><span data-stu-id="885fc-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationrubric-from-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="885fc-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="885fc-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationrubric-from-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="885fc-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="885fc-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationrubric-from-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="885fc-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="885fc-134">Response</span></span>

<span data-ttu-id="885fc-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="885fc-135">The following is an example of the response.</span></span>

> <span data-ttu-id="885fc-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="885fc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric"
} -->

```http
HTTP/1.1 204 No Content
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
