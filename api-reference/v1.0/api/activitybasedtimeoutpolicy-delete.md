---
title: Excluir activityBasedTimeoutPolicy
description: Excluir activityBasedTimeoutPolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a541d32fe57a2734b9e744c6c306a656c3a9fe46
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442632"
---
# <a name="delete-activitybasedtimeoutpolicy"></a><span data-ttu-id="804ef-103">Excluir activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="804ef-103">Delete activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="804ef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="804ef-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="804ef-105">[Exclua um objeto activityBasedTimeoutPolicy.](../resources/activitybasedtimeoutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="804ef-105">Delete an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="804ef-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="804ef-106">Permissions</span></span>

<span data-ttu-id="804ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="804ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="804ef-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="804ef-109">Permission type</span></span>                        | <span data-ttu-id="804ef-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="804ef-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="804ef-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="804ef-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="804ef-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="804ef-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="804ef-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="804ef-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="804ef-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="804ef-114">Not supported.</span></span> |
| <span data-ttu-id="804ef-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="804ef-115">Application</span></span>                            | <span data-ttu-id="804ef-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="804ef-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="804ef-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="804ef-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="804ef-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="804ef-118">Request headers</span></span>

| <span data-ttu-id="804ef-119">Nome</span><span class="sxs-lookup"><span data-stu-id="804ef-119">Name</span></span>          | <span data-ttu-id="804ef-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="804ef-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="804ef-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="804ef-121">Authorization</span></span> | <span data-ttu-id="804ef-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="804ef-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="804ef-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="804ef-124">Request body</span></span>

<span data-ttu-id="804ef-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="804ef-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="804ef-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="804ef-126">Response</span></span>

<span data-ttu-id="804ef-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="804ef-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="804ef-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="804ef-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="804ef-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="804ef-129">Request</span></span>

<span data-ttu-id="804ef-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="804ef-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="804ef-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="804ef-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_activitybasedtimeoutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/activityBasedTimeoutPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="804ef-132">C#</span><span class="sxs-lookup"><span data-stu-id="804ef-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-activitybasedtimeoutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="804ef-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="804ef-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-activitybasedtimeoutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="804ef-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="804ef-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-activitybasedtimeoutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="804ef-135">Java</span><span class="sxs-lookup"><span data-stu-id="804ef-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-activitybasedtimeoutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="804ef-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="804ef-136">Response</span></span>

<span data-ttu-id="804ef-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="804ef-137">The following is an example of the response.</span></span>

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

