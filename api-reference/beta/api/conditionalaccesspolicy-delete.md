---
title: Excluir conditionalAccessPolicy
description: Excluir um conditionalAccessPolicy.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 29e8bc18b4608f08a8285c6b575e2ce96c204fc4
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916506"
---
# <a name="delete-conditionalaccesspolicy"></a><span data-ttu-id="b7f32-103">Excluir conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="b7f32-103">Delete conditionalAccessPolicy</span></span>

<span data-ttu-id="b7f32-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7f32-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7f32-105">Excluir um objeto [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="b7f32-105">Delete a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7f32-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b7f32-106">Permissions</span></span>

<span data-ttu-id="b7f32-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7f32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7f32-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7f32-109">Permission type</span></span>                        | <span data-ttu-id="b7f32-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b7f32-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="b7f32-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7f32-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b7f32-112">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="b7f32-112">Policy.ReadWrite.ConditionalAccess</span></span> |
|<span data-ttu-id="b7f32-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7f32-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7f32-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7f32-114">Not supported.</span></span> |
|<span data-ttu-id="b7f32-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7f32-115">Application</span></span>                            | <span data-ttu-id="b7f32-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7f32-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7f32-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7f32-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b7f32-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7f32-118">Request headers</span></span>

| <span data-ttu-id="b7f32-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b7f32-119">Name</span></span>          | <span data-ttu-id="b7f32-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7f32-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b7f32-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7f32-121">Authorization</span></span> | <span data-ttu-id="b7f32-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7f32-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7f32-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7f32-124">Request body</span></span>

<span data-ttu-id="b7f32-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b7f32-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7f32-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7f32-126">Response</span></span>

<span data-ttu-id="b7f32-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7f32-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b7f32-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b7f32-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b7f32-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7f32-130">Request</span></span>

<span data-ttu-id="b7f32-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7f32-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b7f32-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b7f32-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conditionalaccesspolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/identity/conditionalAccess/policies/{id}
```
# <a name="c"></a>[<span data-ttu-id="b7f32-133">C#</span><span class="sxs-lookup"><span data-stu-id="b7f32-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conditionalaccesspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b7f32-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b7f32-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conditionalaccesspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b7f32-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b7f32-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conditionalaccesspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b7f32-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7f32-136">Response</span></span>

<span data-ttu-id="b7f32-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b7f32-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete conditionalAccessPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
