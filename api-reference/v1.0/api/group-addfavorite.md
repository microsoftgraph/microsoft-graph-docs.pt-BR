---
title: 'group: addFavorite'
description: Adicionar o grupo à lista de grupos de favoritos do usuário atual. Com suporte apenas para grupos do Office 365.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 451cc5adf5a943eda99912ddae1179ca785fcf7a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33614679"
---
# <a name="group-addfavorite"></a><span data-ttu-id="4fb59-104">group: addFavorite</span><span class="sxs-lookup"><span data-stu-id="4fb59-104">group: addFavorite</span></span>
<span data-ttu-id="4fb59-p102">Adicionar o grupo à lista de grupos de favoritos do usuário atual. Com suporte apenas para grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="4fb59-p102">Add the group to the list of the current user's favorite groups. Supported for Office 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="4fb59-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4fb59-107">Permissions</span></span>
<span data-ttu-id="4fb59-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fb59-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fb59-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4fb59-110">Permission type</span></span>      | <span data-ttu-id="4fb59-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4fb59-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4fb59-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4fb59-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4fb59-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fb59-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4fb59-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4fb59-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4fb59-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4fb59-115">Not supported.</span></span>    |
|<span data-ttu-id="4fb59-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4fb59-116">Application</span></span> | <span data-ttu-id="4fb59-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4fb59-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4fb59-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4fb59-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/addFavorite
```

## <a name="request-headers"></a><span data-ttu-id="4fb59-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4fb59-119">Request headers</span></span>
| <span data-ttu-id="4fb59-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4fb59-120">Header</span></span>       | <span data-ttu-id="4fb59-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4fb59-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4fb59-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4fb59-122">Authorization</span></span>  | <span data-ttu-id="4fb59-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4fb59-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4fb59-125">Preferir</span><span class="sxs-lookup"><span data-stu-id="4fb59-125">Prefer</span></span> | <span data-ttu-id="4fb59-126">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="4fb59-126">return=minimal.</span></span> <span data-ttu-id="4fb59-127">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4fb59-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="4fb59-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="4fb59-128">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4fb59-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4fb59-129">Request body</span></span>
<span data-ttu-id="4fb59-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4fb59-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4fb59-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fb59-131">Response</span></span>
<span data-ttu-id="4fb59-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4fb59-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fb59-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4fb59-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4fb59-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4fb59-135">Request</span></span>
<span data-ttu-id="4fb59-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4fb59-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_addfavorite"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/addFavorite
```

#### <a name="response"></a><span data-ttu-id="4fb59-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fb59-137">Response</span></span>
<span data-ttu-id="4fb59-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4fb59-138">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4fb59-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="4fb59-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4fb59-140">Basic</span><span class="sxs-lookup"><span data-stu-id="4fb59-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group_addfavorite-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4fb59-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4fb59-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group_addfavorite-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: addFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-addfavorite.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-addfavorite.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
