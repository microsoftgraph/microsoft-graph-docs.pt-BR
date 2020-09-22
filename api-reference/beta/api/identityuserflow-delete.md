---
title: Excluir userflow
description: Excluir userflow.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 29452ee5750be5d1a52965dd52caa264bbfbc804
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006675"
---
# <a name="delete-userflow"></a><span data-ttu-id="949a8-103">Excluir userflow</span><span class="sxs-lookup"><span data-stu-id="949a8-103">Delete userFlow</span></span>

<span data-ttu-id="949a8-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="949a8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="949a8-105">Excluir um objeto [userflow](../resources/identityuserflow.md) existente.</span><span class="sxs-lookup"><span data-stu-id="949a8-105">Delete an existing [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="949a8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="949a8-106">Permissions</span></span>

<span data-ttu-id="949a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="949a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="949a8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="949a8-109">Permission type</span></span>                        | <span data-ttu-id="949a8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="949a8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="949a8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="949a8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="949a8-112">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="949a8-112">IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="949a8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="949a8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="949a8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="949a8-114">Not supported.</span></span> |
| <span data-ttu-id="949a8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="949a8-115">Application</span></span>                            | <span data-ttu-id="949a8-116">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="949a8-116">IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="949a8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="949a8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/userFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="949a8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="949a8-118">Request headers</span></span>

| <span data-ttu-id="949a8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="949a8-119">Name</span></span>          | <span data-ttu-id="949a8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="949a8-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="949a8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="949a8-121">Authorization</span></span> | <span data-ttu-id="949a8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="949a8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="949a8-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="949a8-124">Request body</span></span>

<span data-ttu-id="949a8-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="949a8-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="949a8-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="949a8-126">Response</span></span>

<span data-ttu-id="949a8-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="949a8-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="949a8-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="949a8-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="949a8-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="949a8-130">Request</span></span>

<span data-ttu-id="949a8-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="949a8-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="949a8-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="949a8-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityuserflow"
}-->

```http
DELETE https://graph.microsoft.com/beta/identity/userFlows/{id}
```
# <a name="c"></a>[<span data-ttu-id="949a8-133">C#</span><span class="sxs-lookup"><span data-stu-id="949a8-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="949a8-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="949a8-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="949a8-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="949a8-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="949a8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="949a8-136">Response</span></span>

<span data-ttu-id="949a8-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="949a8-137">The following is an example of the response.</span></span>

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


