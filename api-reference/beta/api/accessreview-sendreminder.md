---
title: SendReminder accessReview
description: 'No recurso de revisões do Azure AD Access, envie um lembrete para os revisores de um accessReview ativo no momento.  O objeto de destino pode ser uma revisão de acesso única ou uma instância de uma revisão de acesso recorrente. '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8de9b05873ec1f28172568ce242494db0db6e3cd
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636769"
---
# <a name="sendreminder-accessreview"></a><span data-ttu-id="52e25-104">SendReminder accessReview</span><span class="sxs-lookup"><span data-stu-id="52e25-104">SendReminder accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52e25-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , envie um lembrete para os revisores de um [accessReview](../resources/accessreview.md)ativo no momento.</span><span class="sxs-lookup"><span data-stu-id="52e25-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, send a reminder to the reviewers of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="52e25-106">O objeto de destino pode ser uma revisão de acesso única ou uma instância de uma revisão de acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="52e25-106">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span> 

## <a name="permissions"></a><span data-ttu-id="52e25-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="52e25-107">Permissions</span></span>
<span data-ttu-id="52e25-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52e25-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52e25-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52e25-110">Permission type</span></span>                        | <span data-ttu-id="52e25-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52e25-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="52e25-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52e25-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="52e25-113">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52e25-113">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="52e25-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52e25-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52e25-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52e25-115">Not supported.</span></span> |
|<span data-ttu-id="52e25-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52e25-116">Application</span></span>                            | <span data-ttu-id="52e25-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52e25-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="52e25-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52e25-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/sendReminder()
```
## <a name="request-headers"></a><span data-ttu-id="52e25-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52e25-119">Request headers</span></span>
| <span data-ttu-id="52e25-120">Nome</span><span class="sxs-lookup"><span data-stu-id="52e25-120">Name</span></span>         | <span data-ttu-id="52e25-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="52e25-121">Type</span></span>        | <span data-ttu-id="52e25-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="52e25-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="52e25-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="52e25-123">Authorization</span></span> | <span data-ttu-id="52e25-124">string</span><span class="sxs-lookup"><span data-stu-id="52e25-124">string</span></span> | <span data-ttu-id="52e25-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52e25-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52e25-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52e25-127">Request body</span></span>
<span data-ttu-id="52e25-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="52e25-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="52e25-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="52e25-129">Response</span></span>
<span data-ttu-id="52e25-p105">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52e25-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52e25-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52e25-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="52e25-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52e25-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/sendReminder
```
##### <a name="response"></a><span data-ttu-id="52e25-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="52e25-134">Response</span></span>
><span data-ttu-id="52e25-p106">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52e25-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="52e25-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="52e25-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="52e25-138">Basic</span><span class="sxs-lookup"><span data-stu-id="52e25-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/sendReminder_accessReview-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="52e25-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52e25-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/sendReminder_accessReview-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/accessreview-sendreminder.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-sendreminder.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
