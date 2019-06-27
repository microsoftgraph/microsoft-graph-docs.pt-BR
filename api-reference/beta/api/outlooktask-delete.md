---
title: Excluir outlookTask
description: Excluir a tarefa especificada do Outlook na caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 1a3cde57422d3955718aa2e58fb431de5db465d8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266798"
---
# <a name="delete-outlooktask"></a><span data-ttu-id="3258c-103">Excluir outlookTask</span><span class="sxs-lookup"><span data-stu-id="3258c-103">Delete outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3258c-104">Excluir a tarefa especificada do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="3258c-104">Delete the specified Outlook task in the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="3258c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3258c-105">Permissions</span></span>

<span data-ttu-id="3258c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3258c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3258c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3258c-108">Permission type</span></span>      | <span data-ttu-id="3258c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3258c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3258c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3258c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3258c-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3258c-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="3258c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3258c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3258c-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3258c-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="3258c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3258c-114">Application</span></span> | <span data-ttu-id="3258c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3258c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3258c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3258c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/{id}
DELETE /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3258c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3258c-117">Request headers</span></span>

| <span data-ttu-id="3258c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="3258c-118">Name</span></span>       | <span data-ttu-id="3258c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="3258c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3258c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="3258c-120">Authorization</span></span>  | <span data-ttu-id="3258c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3258c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3258c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3258c-123">Request body</span></span>

<span data-ttu-id="3258c-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3258c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3258c-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="3258c-125">Response</span></span>

<span data-ttu-id="3258c-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3258c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3258c-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3258c-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="3258c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3258c-129">Request</span></span>

<span data-ttu-id="3258c-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3258c-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlooktask"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADIyAAAhrb_QAAA=
```

### <a name="response"></a><span data-ttu-id="3258c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3258c-131">Response</span></span>

<span data-ttu-id="3258c-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3258c-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3258c-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="3258c-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3258c-134">C#</span><span class="sxs-lookup"><span data-stu-id="3258c-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_outlooktask-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3258c-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="3258c-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_outlooktask-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3258c-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3258c-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_outlooktask-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktask-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/outlooktask-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlooktask-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
