---
title: Excluir educationRubric
description: Excluir um objeto educationRubric.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2d9d3b67ec4ef0ef8bdd6684489630228355e3d1
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461042"
---
# <a name="delete-educationrubric"></a><span data-ttu-id="27153-103">Excluir educationRubric</span><span class="sxs-lookup"><span data-stu-id="27153-103">Delete educationRubric</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27153-104">Excluir um objeto [educationRubric](../resources/educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="27153-104">Delete an [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="27153-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="27153-105">Permissions</span></span>

<span data-ttu-id="27153-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27153-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="27153-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27153-108">Permission type</span></span>                        | <span data-ttu-id="27153-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27153-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="27153-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27153-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="27153-111">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27153-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="27153-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27153-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27153-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27153-113">Not supported.</span></span> |
| <span data-ttu-id="27153-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27153-114">Application</span></span>                            | <span data-ttu-id="27153-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27153-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="27153-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27153-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/me/rubrics/{id}
```

## <a name="request-headers"></a><span data-ttu-id="27153-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27153-117">Request headers</span></span>

| <span data-ttu-id="27153-118">Nome</span><span class="sxs-lookup"><span data-stu-id="27153-118">Name</span></span>          | <span data-ttu-id="27153-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="27153-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="27153-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="27153-120">Authorization</span></span> | <span data-ttu-id="27153-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="27153-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="27153-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27153-122">Request body</span></span>

<span data-ttu-id="27153-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="27153-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27153-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="27153-124">Response</span></span>

<span data-ttu-id="27153-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27153-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="27153-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="27153-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="27153-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27153-128">Request</span></span>

<span data-ttu-id="27153-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="27153-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="27153-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="27153-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationrubric"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/me/rubrics/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="27153-131">C#</span><span class="sxs-lookup"><span data-stu-id="27153-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationrubric-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="27153-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27153-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationrubric-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="27153-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="27153-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationrubric-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="27153-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="27153-134">Response</span></span>

<span data-ttu-id="27153-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="27153-135">The following is an example of the response.</span></span>

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
