---
title: SendReminder accessReview
description: 'No recurso de revisões do Azure AD Access, envie um lembrete para os revisores de um accessReview ativo no momento.  O objeto de destino pode ser uma revisão de acesso única ou uma instância de uma revisão de acesso recorrente. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 565ae1a8916686069ad8950d7be4a346fef751d8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258811"
---
# <a name="sendreminder-accessreview"></a><span data-ttu-id="0ee9a-104">SendReminder accessReview</span><span class="sxs-lookup"><span data-stu-id="0ee9a-104">SendReminder accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ee9a-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , envie um lembrete para os revisores de um [accessReview](../resources/accessreview.md)ativo no momento.</span><span class="sxs-lookup"><span data-stu-id="0ee9a-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, send a reminder to the reviewers of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="0ee9a-106">O objeto de destino pode ser uma revisão de acesso única ou uma instância de uma revisão de acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="0ee9a-106">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span> 

## <a name="permissions"></a><span data-ttu-id="0ee9a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0ee9a-107">Permissions</span></span>
<span data-ttu-id="0ee9a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ee9a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ee9a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ee9a-110">Permission type</span></span>                        | <span data-ttu-id="0ee9a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0ee9a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ee9a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ee9a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0ee9a-113">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ee9a-113">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="0ee9a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ee9a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ee9a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ee9a-115">Not supported.</span></span> |
|<span data-ttu-id="0ee9a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ee9a-116">Application</span></span>                            | <span data-ttu-id="0ee9a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ee9a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ee9a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ee9a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/sendReminder()
```
## <a name="request-headers"></a><span data-ttu-id="0ee9a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ee9a-119">Request headers</span></span>
| <span data-ttu-id="0ee9a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="0ee9a-120">Name</span></span>         | <span data-ttu-id="0ee9a-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ee9a-121">Type</span></span>        | <span data-ttu-id="0ee9a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ee9a-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="0ee9a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ee9a-123">Authorization</span></span> | <span data-ttu-id="0ee9a-124">string</span><span class="sxs-lookup"><span data-stu-id="0ee9a-124">string</span></span> | <span data-ttu-id="0ee9a-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ee9a-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ee9a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ee9a-127">Request body</span></span>
<span data-ttu-id="0ee9a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0ee9a-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="0ee9a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ee9a-129">Response</span></span>
<span data-ttu-id="0ee9a-p105">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ee9a-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ee9a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ee9a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ee9a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ee9a-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/sendReminder
```
##### <a name="response"></a><span data-ttu-id="0ee9a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ee9a-134">Response</span></span>
><span data-ttu-id="0ee9a-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ee9a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0ee9a-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="0ee9a-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0ee9a-138">C#</span><span class="sxs-lookup"><span data-stu-id="0ee9a-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/sendReminder_accessReview-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0ee9a-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="0ee9a-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/sendReminder_accessReview-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0ee9a-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0ee9a-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/sendReminder_accessReview-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "SendReminder accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-sendreminder.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/accessreview-sendreminder.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-sendreminder.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
