---
title: 'group: resetUnseenCount'
description: Redefina a unseenCount de todas as postagens que o usuário atual não viu desde sua última visita. Suporte apenas para Grupos do Office 365.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 4a3c344101f27dab7a9b5d036ed69b73a2f41b43
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592571"
---
# <a name="group-resetunseencount"></a><span data-ttu-id="5b1a1-104">group: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="5b1a1-104">group: resetUnseenCount</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b1a1-105">Redefina a unseenCount de todas as postagens que o usuário atual não viu desde sua última visita.</span><span class="sxs-lookup"><span data-stu-id="5b1a1-105">Reset the unseenCount of all the posts that the current user has not seen since their last visit.</span></span> <span data-ttu-id="5b1a1-106">Suporte apenas para Grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="5b1a1-106">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b1a1-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5b1a1-107">Permissions</span></span>
<span data-ttu-id="5b1a1-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b1a1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b1a1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b1a1-110">Permission type</span></span>      | <span data-ttu-id="5b1a1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5b1a1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b1a1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b1a1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5b1a1-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b1a1-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5b1a1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b1a1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b1a1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b1a1-115">Not supported.</span></span>    |
|<span data-ttu-id="5b1a1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b1a1-116">Application</span></span> | <span data-ttu-id="5b1a1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b1a1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b1a1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b1a1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="5b1a1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b1a1-119">Request headers</span></span>
| <span data-ttu-id="5b1a1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5b1a1-120">Header</span></span>       | <span data-ttu-id="5b1a1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5b1a1-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5b1a1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b1a1-122">Authorization</span></span>  | <span data-ttu-id="5b1a1-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b1a1-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5b1a1-125">Preferir</span><span class="sxs-lookup"><span data-stu-id="5b1a1-125">Prefer</span></span> | <span data-ttu-id="5b1a1-126">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="5b1a1-126">return=minimal.</span></span> <span data-ttu-id="5b1a1-127">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5b1a1-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="5b1a1-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5b1a1-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="5b1a1-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b1a1-129">Request body</span></span>
<span data-ttu-id="5b1a1-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5b1a1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b1a1-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b1a1-131">Response</span></span>
<span data-ttu-id="5b1a1-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b1a1-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b1a1-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b1a1-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5b1a1-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b1a1-135">Request</span></span>
<span data-ttu-id="5b1a1-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b1a1-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/resetUnseenCount
```

#### <a name="response"></a><span data-ttu-id="5b1a1-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b1a1-137">Response</span></span>
<span data-ttu-id="5b1a1-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5b1a1-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5b1a1-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="5b1a1-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5b1a1-140">Basic</span><span class="sxs-lookup"><span data-stu-id="5b1a1-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group_resetunseencount-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5b1a1-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b1a1-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group_resetunseencount-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: resetUnseenCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-resetunseencount.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-resetunseencount.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
