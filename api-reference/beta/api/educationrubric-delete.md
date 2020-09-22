---
title: Excluir educationRubric
description: Excluir um objeto educationRubric.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 277429b3b784ddb4607c3483c88375d401f457b3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002402"
---
# <a name="delete-educationrubric"></a><span data-ttu-id="a1174-103">Excluir educationRubric</span><span class="sxs-lookup"><span data-stu-id="a1174-103">Delete educationRubric</span></span>

<span data-ttu-id="a1174-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1174-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1174-105">Excluir um objeto [educationRubric](../resources/educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="a1174-105">Delete an [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1174-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a1174-106">Permissions</span></span>

<span data-ttu-id="a1174-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1174-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a1174-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1174-109">Permission type</span></span>                        | <span data-ttu-id="a1174-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a1174-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a1174-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1174-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a1174-112">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1174-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="a1174-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1174-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1174-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1174-114">Not supported.</span></span> |
| <span data-ttu-id="a1174-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1174-115">Application</span></span>                            | <span data-ttu-id="a1174-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1174-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1174-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1174-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/me/rubrics/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a1174-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1174-118">Request headers</span></span>

| <span data-ttu-id="a1174-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a1174-119">Name</span></span>          | <span data-ttu-id="a1174-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1174-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a1174-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1174-121">Authorization</span></span> | <span data-ttu-id="a1174-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="a1174-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1174-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1174-123">Request body</span></span>

<span data-ttu-id="a1174-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a1174-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1174-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1174-125">Response</span></span>

<span data-ttu-id="a1174-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1174-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a1174-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a1174-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a1174-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1174-129">Request</span></span>

<span data-ttu-id="a1174-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1174-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a1174-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1174-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationrubric"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/me/rubrics/{id}
```
# <a name="c"></a>[<span data-ttu-id="a1174-132">C#</span><span class="sxs-lookup"><span data-stu-id="a1174-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationrubric-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1174-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1174-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationrubric-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1174-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1174-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationrubric-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a1174-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1174-135">Response</span></span>

<span data-ttu-id="a1174-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a1174-136">The following is an example of the response.</span></span>

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


