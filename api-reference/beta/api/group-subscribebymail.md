---
title: 'group: subscribeByMail'
description: Chamar esse método permitirá que o usuário atual receba notificações por email para este grupo, sobre novas postagens, eventos e arquivos do grupo. Suporte apenas para Grupos do Office 365.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 1ac29aa08035563db9f05c3b8c5db3be0806eb45
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262829"
---
# <a name="group-subscribebymail"></a><span data-ttu-id="f5aff-104">group: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="f5aff-104">group: subscribeByMail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5aff-105">Chamar esse método permitirá que o usuário atual receba notificações por email para este grupo, sobre novas postagens, eventos e arquivos do grupo.</span><span class="sxs-lookup"><span data-stu-id="f5aff-105">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group.</span></span> <span data-ttu-id="f5aff-106">Suporte apenas para Grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="f5aff-106">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5aff-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5aff-107">Permissions</span></span>
<span data-ttu-id="f5aff-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5aff-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5aff-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5aff-110">Permission type</span></span>      | <span data-ttu-id="f5aff-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5aff-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5aff-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5aff-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f5aff-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5aff-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f5aff-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5aff-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5aff-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5aff-115">Not supported.</span></span>    |
|<span data-ttu-id="f5aff-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5aff-116">Application</span></span> | <span data-ttu-id="f5aff-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5aff-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5aff-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5aff-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="f5aff-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5aff-119">Request headers</span></span>
| <span data-ttu-id="f5aff-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f5aff-120">Header</span></span>       | <span data-ttu-id="f5aff-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f5aff-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f5aff-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5aff-122">Authorization</span></span>  | <span data-ttu-id="f5aff-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5aff-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f5aff-125">Preferir</span><span class="sxs-lookup"><span data-stu-id="f5aff-125">Prefer</span></span> | <span data-ttu-id="f5aff-126">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="f5aff-126">return=minimal.</span></span> <span data-ttu-id="f5aff-127">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f5aff-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="f5aff-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f5aff-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="f5aff-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5aff-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="f5aff-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5aff-130">Response</span></span>
<span data-ttu-id="f5aff-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5aff-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5aff-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5aff-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f5aff-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5aff-134">Request</span></span>
<span data-ttu-id="f5aff-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5aff-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/subscribeByMail
```

#### <a name="response"></a><span data-ttu-id="f5aff-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5aff-136">Response</span></span>
<span data-ttu-id="f5aff-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f5aff-137">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f5aff-138">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="f5aff-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f5aff-139">C#</span><span class="sxs-lookup"><span data-stu-id="f5aff-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group_subscribebymail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f5aff-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="f5aff-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group_subscribebymail-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f5aff-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f5aff-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/group_subscribebymail-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: subscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-subscribebymail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-subscribebymail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-subscribebymail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
