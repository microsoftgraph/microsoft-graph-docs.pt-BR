---
title: 'group: subscribeByMail'
description: Chamar esse método permitirá que o usuário atual receba notificações por email para este grupo, sobre novas postagens, eventos e arquivos do grupo. Suporte apenas para Grupos do Office 365.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5fc66ab5e80d939a742db0e70eb527a79249ea44
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592488"
---
# <a name="group-subscribebymail"></a><span data-ttu-id="2c3bb-104">group: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="2c3bb-104">group: subscribeByMail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c3bb-105">Chamar esse método permitirá que o usuário atual receba notificações por email para este grupo, sobre novas postagens, eventos e arquivos do grupo.</span><span class="sxs-lookup"><span data-stu-id="2c3bb-105">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group.</span></span> <span data-ttu-id="2c3bb-106">Suporte apenas para Grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="2c3bb-106">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c3bb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2c3bb-107">Permissions</span></span>
<span data-ttu-id="2c3bb-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c3bb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c3bb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c3bb-110">Permission type</span></span>      | <span data-ttu-id="2c3bb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2c3bb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c3bb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c3bb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2c3bb-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c3bb-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2c3bb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c3bb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c3bb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c3bb-115">Not supported.</span></span>    |
|<span data-ttu-id="2c3bb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c3bb-116">Application</span></span> | <span data-ttu-id="2c3bb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c3bb-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c3bb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c3bb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="2c3bb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c3bb-119">Request headers</span></span>
| <span data-ttu-id="2c3bb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2c3bb-120">Header</span></span>       | <span data-ttu-id="2c3bb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2c3bb-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2c3bb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c3bb-122">Authorization</span></span>  | <span data-ttu-id="2c3bb-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c3bb-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2c3bb-125">Preferir</span><span class="sxs-lookup"><span data-stu-id="2c3bb-125">Prefer</span></span> | <span data-ttu-id="2c3bb-126">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="2c3bb-126">return=minimal.</span></span> <span data-ttu-id="2c3bb-127">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2c3bb-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="2c3bb-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="2c3bb-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="2c3bb-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c3bb-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="2c3bb-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c3bb-130">Response</span></span>
<span data-ttu-id="2c3bb-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c3bb-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c3bb-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2c3bb-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2c3bb-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c3bb-134">Request</span></span>
<span data-ttu-id="2c3bb-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c3bb-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/subscribeByMail
```

#### <a name="response"></a><span data-ttu-id="2c3bb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c3bb-136">Response</span></span>
<span data-ttu-id="2c3bb-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2c3bb-137">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="2c3bb-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="2c3bb-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2c3bb-139">Basic</span><span class="sxs-lookup"><span data-stu-id="2c3bb-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group_subscribebymail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2c3bb-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c3bb-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group_subscribebymail-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/group-subscribebymail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-subscribebymail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
