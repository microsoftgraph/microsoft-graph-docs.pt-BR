---
title: Excluir userflow
description: Excluir userflow.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b9caa40d37cc04f9b248fc273c9c75488b8e63bd
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218833"
---
# <a name="delete-userflow"></a><span data-ttu-id="3c8fa-103">Excluir userflow</span><span class="sxs-lookup"><span data-stu-id="3c8fa-103">Delete userFlow</span></span>

<span data-ttu-id="3c8fa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c8fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c8fa-105">Excluir um objeto [userflow](../resources/identityuserflow.md) existente.</span><span class="sxs-lookup"><span data-stu-id="3c8fa-105">Delete an existing [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c8fa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3c8fa-106">Permissions</span></span>

<span data-ttu-id="3c8fa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c8fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3c8fa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c8fa-109">Permission type</span></span>                        | <span data-ttu-id="3c8fa-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3c8fa-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3c8fa-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c8fa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3c8fa-112">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3c8fa-112">IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="3c8fa-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c8fa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c8fa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c8fa-114">Not supported.</span></span> |
| <span data-ttu-id="3c8fa-115">Application</span><span class="sxs-lookup"><span data-stu-id="3c8fa-115">Application</span></span>                            | <span data-ttu-id="3c8fa-116">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3c8fa-116">IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c8fa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c8fa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/userFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3c8fa-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c8fa-118">Request headers</span></span>

| <span data-ttu-id="3c8fa-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3c8fa-119">Name</span></span>          | <span data-ttu-id="3c8fa-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c8fa-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3c8fa-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c8fa-121">Authorization</span></span> | <span data-ttu-id="3c8fa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c8fa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c8fa-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c8fa-124">Request body</span></span>

<span data-ttu-id="3c8fa-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3c8fa-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c8fa-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c8fa-126">Response</span></span>

<span data-ttu-id="3c8fa-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c8fa-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3c8fa-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3c8fa-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3c8fa-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c8fa-130">Request</span></span>

<span data-ttu-id="3c8fa-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c8fa-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3c8fa-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c8fa-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityuserflow"
}-->

```http
DELETE https://graph.microsoft.com/beta/identity/userFlows/{id}
```
# <a name="c"></a>[<span data-ttu-id="3c8fa-133">C#</span><span class="sxs-lookup"><span data-stu-id="3c8fa-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c8fa-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c8fa-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c8fa-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c8fa-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3c8fa-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c8fa-136">Response</span></span>

<span data-ttu-id="3c8fa-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3c8fa-137">The following is an example of the response.</span></span>

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
  "description": "Delete userFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
