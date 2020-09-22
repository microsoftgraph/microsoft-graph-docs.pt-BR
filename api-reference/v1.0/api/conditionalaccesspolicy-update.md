---
title: Atualizar conditionalaccesspolicy
description: Atualiza as propriedades de um objeto conditionalAccessPolicy.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bef688740af831900da7699f8d664b072f195a96
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067024"
---
# <a name="update-conditionalaccesspolicy"></a><span data-ttu-id="dff8d-103">Atualizar conditionalaccesspolicy</span><span class="sxs-lookup"><span data-stu-id="dff8d-103">Update conditionalaccesspolicy</span></span>

<span data-ttu-id="dff8d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dff8d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dff8d-105">Atualiza as propriedades de um objeto [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="dff8d-105">Update the properties of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dff8d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dff8d-106">Permissions</span></span>

<span data-ttu-id="dff8d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dff8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dff8d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dff8d-109">Permission type</span></span>                        | <span data-ttu-id="dff8d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dff8d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dff8d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dff8d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dff8d-112">Policy. Read. All, Policy. ReadWrite. ConditionalAccess e Application. Read. All</span><span class="sxs-lookup"><span data-stu-id="dff8d-112">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |
| <span data-ttu-id="dff8d-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dff8d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dff8d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dff8d-114">Not supported.</span></span> |
| <span data-ttu-id="dff8d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dff8d-115">Application</span></span>                            | <span data-ttu-id="dff8d-116">Policy. Read. All, Policy. ReadWrite. ConditionalAccess e Application. Read. All</span><span class="sxs-lookup"><span data-stu-id="dff8d-116">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |

> [!NOTE]
> <span data-ttu-id="dff8d-117">Essa API tem um [problema conhecido](/graph/known-issues#permissions) relacionado às permissões.</span><span class="sxs-lookup"><span data-stu-id="dff8d-117">This API has a [known issue](/graph/known-issues#permissions) related to permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="dff8d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dff8d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dff8d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dff8d-119">Request headers</span></span>

| <span data-ttu-id="dff8d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="dff8d-120">Name</span></span>          | <span data-ttu-id="dff8d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="dff8d-121">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="dff8d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dff8d-122">Authorization</span></span> | <span data-ttu-id="dff8d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dff8d-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="dff8d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dff8d-125">Content-Type</span></span>  | <span data-ttu-id="dff8d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dff8d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dff8d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dff8d-128">Request body</span></span>

<span data-ttu-id="dff8d-129">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="dff8d-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="dff8d-130">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="dff8d-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="dff8d-131">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="dff8d-131">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="dff8d-132">Para obter a lista de propriedades, consulte [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dff8d-132">For the list of properties, see [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md).</span></span>

## <a name="response"></a><span data-ttu-id="dff8d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="dff8d-133">Response</span></span>

<span data-ttu-id="dff8d-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dff8d-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dff8d-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dff8d-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="dff8d-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dff8d-137">Request</span></span>

<span data-ttu-id="dff8d-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dff8d-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dff8d-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="dff8d-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_conditionalaccesspolicy"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies/{id}
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
# <a name="c"></a>[<span data-ttu-id="dff8d-140">C#</span><span class="sxs-lookup"><span data-stu-id="dff8d-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-conditionalaccesspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dff8d-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dff8d-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-conditionalaccesspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dff8d-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dff8d-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-conditionalaccesspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dff8d-143">Java</span><span class="sxs-lookup"><span data-stu-id="dff8d-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-conditionalaccesspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="dff8d-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="dff8d-144">Response</span></span>

<span data-ttu-id="dff8d-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dff8d-145">The following is an example of the response.</span></span>

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

