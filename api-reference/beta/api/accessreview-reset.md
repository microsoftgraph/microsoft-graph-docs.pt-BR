---
title: Redefinir accessReview
description: No recurso de revisões do Azure AD Access, redefina as decisões de um accessReview ativo no momento.  O objeto de destino pode ser uma revisão de acesso única ou uma instância de uma revisão de acesso recorrente.  As decisões anteriores não são mais registradas, mas os revisores podem continuar a atualizar as decisões.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ac04f5b63a12147a926aa0dcd1c3aaae462a0852
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408780"
---
# <a name="reset-accessreview"></a><span data-ttu-id="dccc2-105">Redefinir accessReview</span><span class="sxs-lookup"><span data-stu-id="dccc2-105">Reset accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dccc2-106">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , redefina as decisões de um [accessReview](../resources/accessreview.md)ativo no momento.</span><span class="sxs-lookup"><span data-stu-id="dccc2-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, reset the decisions of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="dccc2-107">O objeto de destino pode ser uma revisão de acesso única ou uma instância de uma revisão de acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="dccc2-107">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="dccc2-108">As decisões anteriores não são mais registradas, mas os revisores podem continuar a atualizar as decisões.</span><span class="sxs-lookup"><span data-stu-id="dccc2-108">Previous decisions are no longer recorded, but reviewers can continue to update decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="dccc2-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="dccc2-109">Permissions</span></span>
<span data-ttu-id="dccc2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dccc2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dccc2-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dccc2-112">Permission type</span></span>                        | <span data-ttu-id="dccc2-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dccc2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="dccc2-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dccc2-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="dccc2-115">AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="dccc2-115">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="dccc2-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dccc2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dccc2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dccc2-117">Not supported.</span></span> |
|<span data-ttu-id="dccc2-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dccc2-118">Application</span></span>                            | <span data-ttu-id="dccc2-119">AccessReview. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="dccc2-119">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="dccc2-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dccc2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/resetDecisions
```
## <a name="request-headers"></a><span data-ttu-id="dccc2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dccc2-121">Request headers</span></span>
| <span data-ttu-id="dccc2-122">Nome</span><span class="sxs-lookup"><span data-stu-id="dccc2-122">Name</span></span>         | <span data-ttu-id="dccc2-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="dccc2-123">Type</span></span>        | <span data-ttu-id="dccc2-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="dccc2-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="dccc2-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="dccc2-125">Authorization</span></span> | <span data-ttu-id="dccc2-126">string</span><span class="sxs-lookup"><span data-stu-id="dccc2-126">string</span></span> | <span data-ttu-id="dccc2-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dccc2-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dccc2-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dccc2-129">Request body</span></span>
<span data-ttu-id="dccc2-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dccc2-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="dccc2-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="dccc2-131">Response</span></span>
<span data-ttu-id="dccc2-p105">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dccc2-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dccc2-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dccc2-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dccc2-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dccc2-135">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dccc2-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="dccc2-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reset_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/resetDecisions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dccc2-137">C#</span><span class="sxs-lookup"><span data-stu-id="dccc2-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reset-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dccc2-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dccc2-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reset-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dccc2-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="dccc2-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reset-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dccc2-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="dccc2-140">Response</span></span>
><span data-ttu-id="dccc2-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dccc2-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
