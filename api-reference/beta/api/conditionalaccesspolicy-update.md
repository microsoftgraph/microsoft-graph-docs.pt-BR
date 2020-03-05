---
title: Atualizar conditionalAccessPolicy
description: Atualiza as propriedades de um objeto conditionalAccessPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7716697d6dd5cdb852c0851c301dba00b28f3fe8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437956"
---
# <a name="update-conditionalaccesspolicy"></a><span data-ttu-id="11555-103">Atualizar conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="11555-103">Update conditionalAccessPolicy</span></span>

<span data-ttu-id="11555-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="11555-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11555-105">Atualiza as propriedades de um objeto [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="11555-105">Update the properties of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="11555-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="11555-106">Permissions</span></span>

<span data-ttu-id="11555-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11555-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11555-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11555-109">Permission type</span></span>                        | <span data-ttu-id="11555-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11555-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="11555-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11555-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="11555-112">Policy. ReadWrite. ConditionalAccess e Application. Read. All</span><span class="sxs-lookup"><span data-stu-id="11555-112">Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |
|<span data-ttu-id="11555-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11555-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11555-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11555-114">Not supported.</span></span> |
|<span data-ttu-id="11555-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11555-115">Application</span></span>                            | <span data-ttu-id="11555-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11555-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="11555-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11555-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="11555-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11555-118">Request headers</span></span>

| <span data-ttu-id="11555-119">Nome</span><span class="sxs-lookup"><span data-stu-id="11555-119">Name</span></span>          | <span data-ttu-id="11555-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="11555-120">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="11555-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="11555-121">Authorization</span></span> | <span data-ttu-id="11555-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11555-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="11555-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="11555-124">Content-Type</span></span>  | <span data-ttu-id="11555-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11555-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11555-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11555-127">Request body</span></span>

<span data-ttu-id="11555-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="11555-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="11555-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="11555-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="11555-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="11555-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="11555-131">Para obter a lista de propriedades, consulte [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="11555-131">For the list of properties, see [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md).</span></span>

## <a name="response"></a><span data-ttu-id="11555-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="11555-132">Response</span></span>

<span data-ttu-id="11555-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11555-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="11555-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="11555-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="11555-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11555-136">Request</span></span>

<span data-ttu-id="11555-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="11555-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="11555-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="11555-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="11555-139">C#</span><span class="sxs-lookup"><span data-stu-id="11555-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-conditionalaccesspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11555-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11555-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-conditionalaccesspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11555-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11555-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-conditionalaccesspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="11555-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="11555-142">Response</span></span>

<span data-ttu-id="11555-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="11555-143">The following is an example of the response.</span></span>

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
