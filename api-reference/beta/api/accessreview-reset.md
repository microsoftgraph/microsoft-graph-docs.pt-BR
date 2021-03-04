---
title: Redefinir accessReview
description: No recurso de revisões de acesso do Azure AD, redefinir as decisões de um accessReview ativo no momento.  O objeto de destino pode ser uma revisão de acesso único ou uma instância de uma revisão de acesso recorrente.  As decisões anteriores não são mais registradas, mas os revisadores podem continuar a atualizar decisões.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d4dd539e4809a8914b74700fd550917cab164145
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439293"
---
# <a name="reset-accessreview"></a><span data-ttu-id="cddf8-105">Redefinir accessReview</span><span class="sxs-lookup"><span data-stu-id="cddf8-105">Reset accessReview</span></span>

<span data-ttu-id="cddf8-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cddf8-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cddf8-107">No recurso de revisões de acesso do Azure [AD,](../resources/accessreviews-root.md) redefinir as decisões de um [accessReview ativo no momento.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="cddf8-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, reset the decisions of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="cddf8-108">O objeto de destino pode ser uma revisão de acesso único ou uma instância de uma revisão de acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="cddf8-108">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="cddf8-109">As decisões anteriores não são mais registradas, mas os revisadores podem continuar a atualizar decisões.</span><span class="sxs-lookup"><span data-stu-id="cddf8-109">Previous decisions are no longer recorded, but reviewers can continue to update decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="cddf8-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="cddf8-110">Permissions</span></span>
<span data-ttu-id="cddf8-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cddf8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cddf8-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cddf8-113">Permission type</span></span>                        | <span data-ttu-id="cddf8-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cddf8-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="cddf8-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cddf8-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="cddf8-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cddf8-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="cddf8-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cddf8-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cddf8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cddf8-118">Not supported.</span></span> |
|<span data-ttu-id="cddf8-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cddf8-119">Application</span></span>                            | <span data-ttu-id="cddf8-120">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="cddf8-120">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="cddf8-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cddf8-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/resetDecisions
```
## <a name="request-headers"></a><span data-ttu-id="cddf8-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cddf8-122">Request headers</span></span>
| <span data-ttu-id="cddf8-123">Nome</span><span class="sxs-lookup"><span data-stu-id="cddf8-123">Name</span></span>         | <span data-ttu-id="cddf8-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="cddf8-124">Type</span></span>        | <span data-ttu-id="cddf8-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="cddf8-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="cddf8-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="cddf8-126">Authorization</span></span> | <span data-ttu-id="cddf8-127">string</span><span class="sxs-lookup"><span data-stu-id="cddf8-127">string</span></span> | <span data-ttu-id="cddf8-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cddf8-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cddf8-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cddf8-130">Request body</span></span>
<span data-ttu-id="cddf8-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cddf8-131">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="cddf8-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="cddf8-132">Response</span></span>
<span data-ttu-id="cddf8-p105">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cddf8-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cddf8-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cddf8-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cddf8-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cddf8-136">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="cddf8-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="cddf8-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reset_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/resetDecisions
```
# <a name="c"></a>[<span data-ttu-id="cddf8-138">C#</span><span class="sxs-lookup"><span data-stu-id="cddf8-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reset-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cddf8-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cddf8-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reset-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cddf8-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cddf8-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reset-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cddf8-141">Java</span><span class="sxs-lookup"><span data-stu-id="cddf8-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reset-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cddf8-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="cddf8-142">Response</span></span>
><span data-ttu-id="cddf8-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cddf8-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Reset accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


