---
title: Excluir conditionalAccessPolicy
description: Excluir um conditionalAccessPolicy.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f49e0b6a7817fffa1773b6793acf2759187b90e6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43387195"
---
# <a name="delete-conditionalaccesspolicy"></a><span data-ttu-id="e42de-103">Excluir conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="e42de-103">Delete conditionalAccessPolicy</span></span>

<span data-ttu-id="e42de-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e42de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e42de-105">Excluir um objeto [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="e42de-105">Delete a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e42de-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e42de-106">Permissions</span></span>

<span data-ttu-id="e42de-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e42de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e42de-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e42de-109">Permission type</span></span>                        | <span data-ttu-id="e42de-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e42de-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="e42de-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e42de-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e42de-112">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="e42de-112">Policy.ReadWrite.ConditionalAccess</span></span> |
|<span data-ttu-id="e42de-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e42de-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e42de-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e42de-114">Not supported.</span></span> |
|<span data-ttu-id="e42de-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e42de-115">Application</span></span>                            | <span data-ttu-id="e42de-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e42de-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e42de-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e42de-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e42de-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e42de-118">Request headers</span></span>

| <span data-ttu-id="e42de-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e42de-119">Name</span></span>          | <span data-ttu-id="e42de-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e42de-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e42de-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e42de-121">Authorization</span></span> | <span data-ttu-id="e42de-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e42de-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e42de-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e42de-124">Request body</span></span>

<span data-ttu-id="e42de-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e42de-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e42de-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="e42de-126">Response</span></span>

<span data-ttu-id="e42de-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e42de-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e42de-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e42de-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e42de-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e42de-130">Request</span></span>

<span data-ttu-id="e42de-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e42de-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e42de-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e42de-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conditionalaccesspolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/identity/conditionalAccess/policies/{id}
```
# <a name="c"></a>[<span data-ttu-id="e42de-133">C#</span><span class="sxs-lookup"><span data-stu-id="e42de-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conditionalaccesspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e42de-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e42de-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conditionalaccesspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e42de-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e42de-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conditionalaccesspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e42de-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e42de-136">Response</span></span>

<span data-ttu-id="e42de-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e42de-137">The following is an example of the response.</span></span>

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
