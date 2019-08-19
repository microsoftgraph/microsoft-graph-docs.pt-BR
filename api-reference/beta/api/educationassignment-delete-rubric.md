---
title: Remover o educationRubric do educationAssignment
description: Remover um educationRubric de um educationAssignment
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 19b35c7684e3b1886d5479ed9e3d9011683bf06e
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461163"
---
# <a name="remove-educationrubric-from-educationassignment"></a><span data-ttu-id="9dc31-103">Remover o educationRubric do educationAssignment</span><span class="sxs-lookup"><span data-stu-id="9dc31-103">Remove educationRubric from educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9dc31-104">Remover um [educationRubric](../resources/educationrubric.md) de um [educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9dc31-104">Remove an [educationRubric](../resources/educationrubric.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>  <span data-ttu-id="9dc31-105">Isso não exclui o próprio amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="9dc31-105">This does not delete the rubric itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="9dc31-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9dc31-106">Permissions</span></span>

<span data-ttu-id="9dc31-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9dc31-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9dc31-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9dc31-109">Permission type</span></span>                        | <span data-ttu-id="9dc31-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9dc31-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9dc31-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9dc31-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9dc31-112">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9dc31-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="9dc31-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9dc31-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9dc31-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9dc31-114">Not supported.</span></span> |
| <span data-ttu-id="9dc31-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9dc31-115">Application</span></span>                            | <span data-ttu-id="9dc31-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9dc31-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9dc31-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9dc31-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignments/{id}/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="9dc31-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9dc31-118">Request headers</span></span>

| <span data-ttu-id="9dc31-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9dc31-119">Name</span></span>          | <span data-ttu-id="9dc31-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9dc31-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9dc31-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9dc31-121">Authorization</span></span> | <span data-ttu-id="9dc31-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="9dc31-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9dc31-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9dc31-123">Request body</span></span>

<span data-ttu-id="9dc31-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9dc31-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9dc31-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="9dc31-125">Response</span></span>

<span data-ttu-id="9dc31-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9dc31-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9dc31-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9dc31-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9dc31-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9dc31-129">Request</span></span>

<span data-ttu-id="9dc31-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9dc31-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9dc31-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="9dc31-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationrubric_from_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/me/assignments/{id}/rubric/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9dc31-132">C#</span><span class="sxs-lookup"><span data-stu-id="9dc31-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationrubric-from-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9dc31-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9dc31-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationrubric-from-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9dc31-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9dc31-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationrubric-from-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9dc31-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9dc31-135">Response</span></span>

<span data-ttu-id="9dc31-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9dc31-136">The following is an example of the response.</span></span>

> <span data-ttu-id="9dc31-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9dc31-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
