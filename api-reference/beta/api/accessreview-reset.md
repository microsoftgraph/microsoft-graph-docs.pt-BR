---
title: Redefinir accessReview
description: No recurso de revisões do Azure AD Access, redefina as decisões de um accessReview ativo no momento.  O objeto de destino pode ser uma revisão de acesso única ou uma instância de uma revisão de acesso recorrente.  As decisões anteriores não são mais registradas, mas os revisores podem continuar a atualizar as decisões.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e3f848b2e1c9d648ed0888bb30b72e2533f07eda
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258832"
---
# <a name="reset-accessreview"></a><span data-ttu-id="2c2cf-105">Redefinir accessReview</span><span class="sxs-lookup"><span data-stu-id="2c2cf-105">Reset accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c2cf-106">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , redefina as decisões de um [accessReview](../resources/accessreview.md)ativo no momento.</span><span class="sxs-lookup"><span data-stu-id="2c2cf-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, reset the decisions of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="2c2cf-107">O objeto de destino pode ser uma revisão de acesso única ou uma instância de uma revisão de acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="2c2cf-107">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="2c2cf-108">As decisões anteriores não são mais registradas, mas os revisores podem continuar a atualizar as decisões.</span><span class="sxs-lookup"><span data-stu-id="2c2cf-108">Previous decisions are no longer recorded, but reviewers can continue to update decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c2cf-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="2c2cf-109">Permissions</span></span>
<span data-ttu-id="2c2cf-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c2cf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c2cf-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c2cf-112">Permission type</span></span>                        | <span data-ttu-id="2c2cf-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2c2cf-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c2cf-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c2cf-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="2c2cf-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c2cf-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="2c2cf-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c2cf-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c2cf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c2cf-117">Not supported.</span></span> |
|<span data-ttu-id="2c2cf-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c2cf-118">Application</span></span>                            | <span data-ttu-id="2c2cf-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c2cf-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c2cf-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c2cf-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/resetDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="2c2cf-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c2cf-121">Request headers</span></span>
| <span data-ttu-id="2c2cf-122">Nome</span><span class="sxs-lookup"><span data-stu-id="2c2cf-122">Name</span></span>         | <span data-ttu-id="2c2cf-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c2cf-123">Type</span></span>        | <span data-ttu-id="2c2cf-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c2cf-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="2c2cf-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c2cf-125">Authorization</span></span> | <span data-ttu-id="2c2cf-126">string</span><span class="sxs-lookup"><span data-stu-id="2c2cf-126">string</span></span> | <span data-ttu-id="2c2cf-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c2cf-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c2cf-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c2cf-129">Request body</span></span>
<span data-ttu-id="2c2cf-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2c2cf-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="2c2cf-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c2cf-131">Response</span></span>
<span data-ttu-id="2c2cf-p105">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c2cf-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c2cf-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2c2cf-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2c2cf-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c2cf-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "reset_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/resetDecisions
```
##### <a name="response"></a><span data-ttu-id="2c2cf-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c2cf-136">Response</span></span>
><span data-ttu-id="2c2cf-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2c2cf-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="2c2cf-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="2c2cf-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2c2cf-140">C#</span><span class="sxs-lookup"><span data-stu-id="2c2cf-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reset_accessReview-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2c2cf-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="2c2cf-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reset_accessReview-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2c2cf-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2c2cf-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reset_accessReview-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/accessreview-reset.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/accessreview-reset.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-reset.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
