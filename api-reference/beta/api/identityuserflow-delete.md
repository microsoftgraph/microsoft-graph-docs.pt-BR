---
title: Excluir userflow
description: Excluir userflow.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8750ecc9770d0b067704c271b7b7bc898d57d542
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938033"
---
# <a name="delete-userflow"></a><span data-ttu-id="b3014-103">Excluir userflow</span><span class="sxs-lookup"><span data-stu-id="b3014-103">Delete userFlow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3014-104">Excluir um objeto [userflow](../resources/identityuserflow.md) existente.</span><span class="sxs-lookup"><span data-stu-id="b3014-104">Delete an existing [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3014-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b3014-105">Permissions</span></span>

<span data-ttu-id="b3014-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3014-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b3014-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3014-108">Permission type</span></span>                        | <span data-ttu-id="b3014-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3014-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b3014-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3014-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b3014-111">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b3014-111">IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="b3014-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3014-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3014-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3014-113">Not supported.</span></span> |
| <span data-ttu-id="b3014-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3014-114">Application</span></span>                            | <span data-ttu-id="b3014-115">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b3014-115">IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3014-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3014-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/userFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b3014-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3014-117">Request headers</span></span>

| <span data-ttu-id="b3014-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b3014-118">Name</span></span>          | <span data-ttu-id="b3014-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3014-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b3014-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3014-120">Authorization</span></span> | <span data-ttu-id="b3014-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3014-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3014-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3014-123">Request body</span></span>

<span data-ttu-id="b3014-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b3014-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3014-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3014-125">Response</span></span>

<span data-ttu-id="b3014-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3014-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b3014-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b3014-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b3014-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3014-129">Request</span></span>

<span data-ttu-id="b3014-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3014-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b3014-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3014-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityuserflow"
}-->

```http
DELETE https://graph.microsoft.com/beta/identity/userFlows/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b3014-132">C#</span><span class="sxs-lookup"><span data-stu-id="b3014-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b3014-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3014-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b3014-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3014-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b3014-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3014-135">Response</span></span>

<span data-ttu-id="b3014-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b3014-136">The following is an example of the response.</span></span>

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
