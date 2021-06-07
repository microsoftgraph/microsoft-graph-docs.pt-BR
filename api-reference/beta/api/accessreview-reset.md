---
title: Redefinir accessReview
description: No recurso de revisões de acesso do Azure AD, redefinir as decisões de um accessReview ativo no momento.  O objeto de destino pode ser uma revisão de acesso único ou uma instância de uma revisão de acesso recorrente.  As decisões anteriores não são mais registradas, mas os revisadores podem continuar a atualizar decisões.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 3005c6b8c3fbed81e89de62ff1e3e756cce6bd4a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751026"
---
# <a name="reset-accessreview"></a><span data-ttu-id="03e5b-105">Redefinir accessReview</span><span class="sxs-lookup"><span data-stu-id="03e5b-105">Reset accessReview</span></span>

<span data-ttu-id="03e5b-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03e5b-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03e5b-107">No recurso de revisões de acesso do Azure [AD,](../resources/accessreviews-root.md) redefinir as decisões de um [accessReview ativo no momento.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="03e5b-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, reset the decisions of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="03e5b-108">O objeto de destino pode ser uma revisão de acesso único ou uma instância de uma revisão de acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="03e5b-108">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="03e5b-109">As decisões anteriores não são mais registradas, mas os revisadores podem continuar a atualizar decisões.</span><span class="sxs-lookup"><span data-stu-id="03e5b-109">Previous decisions are no longer recorded, but reviewers can continue to update decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="03e5b-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="03e5b-110">Permissions</span></span>
<span data-ttu-id="03e5b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03e5b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03e5b-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03e5b-113">Permission type</span></span>                        | <span data-ttu-id="03e5b-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="03e5b-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="03e5b-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03e5b-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="03e5b-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03e5b-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="03e5b-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03e5b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03e5b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03e5b-118">Not supported.</span></span> |
|<span data-ttu-id="03e5b-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03e5b-119">Application</span></span>                            | <span data-ttu-id="03e5b-120">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="03e5b-120">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="03e5b-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03e5b-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/resetDecisions
```
## <a name="request-headers"></a><span data-ttu-id="03e5b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03e5b-122">Request headers</span></span>
| <span data-ttu-id="03e5b-123">Nome</span><span class="sxs-lookup"><span data-stu-id="03e5b-123">Name</span></span>         | <span data-ttu-id="03e5b-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="03e5b-124">Type</span></span>        | <span data-ttu-id="03e5b-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="03e5b-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="03e5b-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="03e5b-126">Authorization</span></span> | <span data-ttu-id="03e5b-127">string</span><span class="sxs-lookup"><span data-stu-id="03e5b-127">string</span></span> | <span data-ttu-id="03e5b-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03e5b-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="03e5b-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03e5b-130">Request body</span></span>
<span data-ttu-id="03e5b-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="03e5b-131">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="03e5b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="03e5b-132">Response</span></span>
<span data-ttu-id="03e5b-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03e5b-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03e5b-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03e5b-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03e5b-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03e5b-136">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="03e5b-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="03e5b-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reset_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/resetDecisions
```
# <a name="c"></a>[<span data-ttu-id="03e5b-138">C#</span><span class="sxs-lookup"><span data-stu-id="03e5b-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reset-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03e5b-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03e5b-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reset-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03e5b-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03e5b-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reset-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="03e5b-141">Java</span><span class="sxs-lookup"><span data-stu-id="03e5b-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reset-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="03e5b-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="03e5b-142">Response</span></span>
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


