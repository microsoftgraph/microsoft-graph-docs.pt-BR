---
title: Atualizar conditionalAccessPolicy
description: Atualiza as propriedades de um objeto conditionalAccessPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b55e492f7fae576c9026588205eae2bafa99c178
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636761"
---
# <a name="update-conditionalaccesspolicy"></a><span data-ttu-id="8ab84-103">Atualizar conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="8ab84-103">Update conditionalAccessPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ab84-104">Atualiza as propriedades de um objeto [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="8ab84-104">Update the properties of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ab84-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8ab84-105">Permissions</span></span>

<span data-ttu-id="8ab84-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ab84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ab84-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ab84-108">Permission type</span></span>                        | <span data-ttu-id="8ab84-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ab84-109">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="8ab84-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ab84-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8ab84-111">Policy. ReadWrite. ConditionalAccess e Application. Read. All</span><span class="sxs-lookup"><span data-stu-id="8ab84-111">Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |
|<span data-ttu-id="8ab84-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ab84-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ab84-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ab84-113">Not supported.</span></span> |
|<span data-ttu-id="8ab84-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ab84-114">Application</span></span>                            | <span data-ttu-id="8ab84-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ab84-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ab84-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ab84-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8ab84-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ab84-117">Request headers</span></span>

| <span data-ttu-id="8ab84-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8ab84-118">Name</span></span>          | <span data-ttu-id="8ab84-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ab84-119">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="8ab84-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ab84-120">Authorization</span></span> | <span data-ttu-id="8ab84-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ab84-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="8ab84-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8ab84-123">Content-Type</span></span>  | <span data-ttu-id="8ab84-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ab84-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ab84-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ab84-126">Request body</span></span>

<span data-ttu-id="8ab84-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="8ab84-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8ab84-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="8ab84-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8ab84-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="8ab84-129">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="8ab84-130">Para obter a lista de propriedades, consulte [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8ab84-130">For the list of properties, see [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md).</span></span>

## <a name="response"></a><span data-ttu-id="8ab84-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ab84-131">Response</span></span>

<span data-ttu-id="8ab84-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ab84-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8ab84-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8ab84-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8ab84-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ab84-135">Request</span></span>

<span data-ttu-id="8ab84-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ab84-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8ab84-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ab84-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_conditionalaccesspolicy"
}-->

```http
PATCH https://graph.microsoft.com/beta/conditionalAccess/policies/{id}
Content-type: application/json

{
    "conditions": {
        "signInRiskLevels": [
            "high",
            "medium",
            "low",
        ]
    }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8ab84-138">C#</span><span class="sxs-lookup"><span data-stu-id="8ab84-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-conditionalaccesspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8ab84-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ab84-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-conditionalaccesspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8ab84-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8ab84-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-conditionalaccesspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8ab84-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ab84-141">Response</span></span>

<span data-ttu-id="8ab84-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8ab84-142">The following is an example of the response.</span></span>

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
  "description": "Update conditionalaccesspolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
