---
title: Remover rejectedSender
description: Remover um usuário ou grupo da lista de remetentes rejeitados.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 1999e2351cc5e535d97a64c4c84c0bced1bdf12d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449607"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="c0adc-103">Remover rejectedSender</span><span class="sxs-lookup"><span data-stu-id="c0adc-103">Remove rejectedSender</span></span>
<span data-ttu-id="c0adc-104">Remover um usuário ou grupo da lista de remetentes rejeitados.</span><span class="sxs-lookup"><span data-stu-id="c0adc-104">Remove a user or group from the rejected-senders list.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0adc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0adc-105">Permissions</span></span>
<span data-ttu-id="c0adc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0adc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c0adc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0adc-108">Permission type</span></span>                        | <span data-ttu-id="c0adc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0adc-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="c0adc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0adc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c0adc-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0adc-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="c0adc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0adc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0adc-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0adc-113">Not supported.</span></span> |
| <span data-ttu-id="c0adc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0adc-114">Application</span></span>                            | <span data-ttu-id="c0adc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0adc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0adc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0adc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
DELETE /groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/v1.0/groups/{other-group-id}
```

## <a name="request-headers"></a><span data-ttu-id="c0adc-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0adc-117">Request headers</span></span>

| <span data-ttu-id="c0adc-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c0adc-118">Header</span></span>         | <span data-ttu-id="c0adc-119">Valor</span><span class="sxs-lookup"><span data-stu-id="c0adc-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="c0adc-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0adc-120">Authorization</span></span>  | <span data-ttu-id="c0adc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0adc-p102">Bearer {token}. Required.</span></span> 

## <a name="request-body"></a><span data-ttu-id="c0adc-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0adc-123">Request body</span></span>
<span data-ttu-id="c0adc-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0adc-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0adc-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0adc-125">Response</span></span>
<span data-ttu-id="c0adc-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0adc-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0adc-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0adc-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c0adc-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0adc-129">Request</span></span>
<span data-ttu-id="c0adc-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0adc-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c0adc-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0adc-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_rejectedSender_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c0adc-132">C#</span><span class="sxs-lookup"><span data-stu-id="c0adc-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-rejectedsender-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c0adc-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="c0adc-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-rejectedsender-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c0adc-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c0adc-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-rejectedsender-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c0adc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0adc-135">Response</span></span>
<span data-ttu-id="c0adc-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c0adc-136">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
