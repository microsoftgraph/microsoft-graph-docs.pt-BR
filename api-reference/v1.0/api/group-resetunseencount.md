---
title: 'group: resetUnseenCount'
description: Redefina a unseenCount de todas as postagens que o usuário atual não viu desde sua última visita. Suporte apenas para grupos do Office 365.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 035d53537587fde0c6ab0b33fd08fbe7987e1fbd
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613925"
---
# <a name="group-resetunseencount"></a><span data-ttu-id="ad596-104">group: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="ad596-104">group: resetUnseenCount</span></span>
<span data-ttu-id="ad596-p102">Redefina a unseenCount de todas as postagens que o usuário atual não viu desde sua última visita. Suporte apenas para grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="ad596-p102">Reset the unseenCount of all the posts that the current user has not seen since their last visit. Supported for Office 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad596-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ad596-107">Permissions</span></span>
<span data-ttu-id="ad596-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad596-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad596-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad596-110">Permission type</span></span>      | <span data-ttu-id="ad596-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ad596-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad596-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad596-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ad596-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad596-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ad596-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad596-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad596-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad596-115">Not supported.</span></span>    |
|<span data-ttu-id="ad596-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad596-116">Application</span></span> | <span data-ttu-id="ad596-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad596-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad596-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad596-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="ad596-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad596-119">Request headers</span></span>
| <span data-ttu-id="ad596-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ad596-120">Header</span></span>       | <span data-ttu-id="ad596-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ad596-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ad596-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad596-122">Authorization</span></span>  | <span data-ttu-id="ad596-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad596-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ad596-125">Preferir</span><span class="sxs-lookup"><span data-stu-id="ad596-125">Prefer</span></span> | <span data-ttu-id="ad596-126">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="ad596-126">return=minimal.</span></span> <span data-ttu-id="ad596-127">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ad596-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="ad596-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ad596-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="ad596-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad596-129">Request body</span></span>
<span data-ttu-id="ad596-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ad596-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad596-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad596-131">Response</span></span>
<span data-ttu-id="ad596-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad596-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad596-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad596-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ad596-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad596-135">Request</span></span>
<span data-ttu-id="ad596-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad596-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/resetUnseenCount
```

#### <a name="response"></a><span data-ttu-id="ad596-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad596-137">Response</span></span>
<span data-ttu-id="ad596-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ad596-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ad596-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="ad596-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ad596-140">Basic</span><span class="sxs-lookup"><span data-stu-id="ad596-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group_resetunseencount-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ad596-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad596-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group_resetunseencount-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: resetUnseenCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-resetunseencount.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-resetunseencount.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
