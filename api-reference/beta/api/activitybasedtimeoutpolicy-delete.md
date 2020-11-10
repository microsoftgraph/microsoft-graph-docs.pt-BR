---
title: Excluir activityBasedTimeoutPolicy
description: Exclua activityBasedTimeoutPolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4b874e5e7625df1e61ef0e289624bfe441094ee0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952567"
---
# <a name="delete-activitybasedtimeoutpolicy"></a><span data-ttu-id="84a80-103">Excluir activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="84a80-103">Delete activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="84a80-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84a80-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84a80-105">Excluir um objeto [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="84a80-105">Delete an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="84a80-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="84a80-106">Permissions</span></span>

<span data-ttu-id="84a80-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84a80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="84a80-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84a80-109">Permission type</span></span>                        | <span data-ttu-id="84a80-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="84a80-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="84a80-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84a80-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="84a80-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="84a80-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="84a80-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84a80-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84a80-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84a80-114">Not supported.</span></span> |
| <span data-ttu-id="84a80-115">Application</span><span class="sxs-lookup"><span data-stu-id="84a80-115">Application</span></span>                            | <span data-ttu-id="84a80-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="84a80-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="84a80-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84a80-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="84a80-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84a80-118">Request headers</span></span>

| <span data-ttu-id="84a80-119">Nome</span><span class="sxs-lookup"><span data-stu-id="84a80-119">Name</span></span>          | <span data-ttu-id="84a80-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="84a80-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="84a80-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="84a80-121">Authorization</span></span> | <span data-ttu-id="84a80-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="84a80-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="84a80-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84a80-123">Request body</span></span>

<span data-ttu-id="84a80-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="84a80-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84a80-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="84a80-125">Response</span></span>

<span data-ttu-id="84a80-126">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="84a80-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="84a80-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="84a80-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="84a80-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84a80-128">Request</span></span>

<span data-ttu-id="84a80-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="84a80-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="84a80-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="84a80-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_activitybasedtimeoutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="84a80-131">C#</span><span class="sxs-lookup"><span data-stu-id="84a80-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-activitybasedtimeoutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84a80-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84a80-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-activitybasedtimeoutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84a80-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84a80-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-activitybasedtimeoutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84a80-134">Java</span><span class="sxs-lookup"><span data-stu-id="84a80-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-activitybasedtimeoutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="84a80-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="84a80-135">Response</span></span>

<span data-ttu-id="84a80-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="84a80-136">The following is an example of the response.</span></span>

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
  "description": "Delete activityBasedTimeoutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


