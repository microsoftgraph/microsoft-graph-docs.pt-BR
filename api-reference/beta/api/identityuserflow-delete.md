---
title: Excluir userflow
description: Excluir userflow.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6f864005497b90111a499a2733c83c33142a39e1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953303"
---
# <a name="delete-userflow"></a><span data-ttu-id="3487e-103">Excluir userflow</span><span class="sxs-lookup"><span data-stu-id="3487e-103">Delete userFlow</span></span>

<span data-ttu-id="3487e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3487e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3487e-105">Excluir um objeto [userflow](../resources/identityuserflow.md) existente.</span><span class="sxs-lookup"><span data-stu-id="3487e-105">Delete an existing [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3487e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3487e-106">Permissions</span></span>

<span data-ttu-id="3487e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3487e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3487e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3487e-109">Permission type</span></span>                        | <span data-ttu-id="3487e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3487e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3487e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3487e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3487e-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3487e-112">IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="3487e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3487e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3487e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3487e-114">Not supported.</span></span> |
| <span data-ttu-id="3487e-115">Application</span><span class="sxs-lookup"><span data-stu-id="3487e-115">Application</span></span>                            | <span data-ttu-id="3487e-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3487e-116">IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3487e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3487e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/userFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3487e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3487e-118">Request headers</span></span>

| <span data-ttu-id="3487e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3487e-119">Name</span></span>          | <span data-ttu-id="3487e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3487e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3487e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3487e-121">Authorization</span></span> | <span data-ttu-id="3487e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3487e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3487e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3487e-124">Request body</span></span>

<span data-ttu-id="3487e-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3487e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3487e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="3487e-126">Response</span></span>

<span data-ttu-id="3487e-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3487e-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3487e-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3487e-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3487e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3487e-130">Request</span></span>

<span data-ttu-id="3487e-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3487e-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3487e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3487e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityuserflow"
}-->

```http
DELETE https://graph.microsoft.com/beta/identity/userFlows/{id}
```
# <a name="c"></a>[<span data-ttu-id="3487e-133">C#</span><span class="sxs-lookup"><span data-stu-id="3487e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3487e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3487e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3487e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3487e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3487e-136">Java</span><span class="sxs-lookup"><span data-stu-id="3487e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-identityuserflow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3487e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3487e-137">Response</span></span>

<span data-ttu-id="3487e-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3487e-138">The following is an example of the response.</span></span>

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


