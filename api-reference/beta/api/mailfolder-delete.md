---
title: Excluir mailFolder
description: Exclua o mailFolder ou o mailSearchFolder especificado.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: d219d9c410573b932c7022b2aea50826d0a016c1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266133"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="b694d-103">Excluir mailFolder</span><span class="sxs-lookup"><span data-stu-id="b694d-103">Delete mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b694d-104">Exclua o [mailFolder](../resources/mailfolder.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="b694d-104">Delete the specified [mailFolder](../resources/mailfolder.md).</span></span> <span data-ttu-id="b694d-105">A pasta pode ser uma [mailSearchFolder](../resources/mailsearchfolder.md).</span><span class="sxs-lookup"><span data-stu-id="b694d-105">The folder can be a [mailSearchFolder](../resources/mailsearchfolder.md).</span></span>

<span data-ttu-id="b694d-106">Você pode especificar uma pasta de email por sua ID de pasta ou por seu [nome de pasta conhecido](../resources/mailfolder.md), se houver uma.</span><span class="sxs-lookup"><span data-stu-id="b694d-106">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="b694d-107">**Observação** Você pode não conseguir excluir itens da pasta exclusão de itens recuperáveis (representado pelo nome `recoverableitemsdeletions`de pasta conhecido).</span><span class="sxs-lookup"><span data-stu-id="b694d-107">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="b694d-108">Veja [retenção de item excluído](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) e [limpar itens excluídos](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="b694d-108">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="b694d-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="b694d-109">Permissions</span></span>
<span data-ttu-id="b694d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b694d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b694d-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b694d-112">Permission type</span></span>      | <span data-ttu-id="b694d-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b694d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b694d-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b694d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b694d-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b694d-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b694d-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b694d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b694d-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b694d-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b694d-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b694d-118">Application</span></span> | <span data-ttu-id="b694d-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b694d-119">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b694d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b694d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b694d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b694d-121">Request headers</span></span>
| <span data-ttu-id="b694d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="b694d-122">Name</span></span>       | <span data-ttu-id="b694d-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="b694d-123">Type</span></span> | <span data-ttu-id="b694d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b694d-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b694d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b694d-125">Authorization</span></span>  | <span data-ttu-id="b694d-126">string</span><span class="sxs-lookup"><span data-stu-id="b694d-126">string</span></span>  | <span data-ttu-id="b694d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b694d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b694d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b694d-129">Request body</span></span>
<span data-ttu-id="b694d-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b694d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b694d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b694d-131">Response</span></span>
<span data-ttu-id="b694d-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b694d-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b694d-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b694d-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b694d-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b694d-135">Request</span></span>
<span data-ttu-id="b694d-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b694d-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/
```

#### <a name="response"></a><span data-ttu-id="b694d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b694d-137">Response</span></span>
<span data-ttu-id="b694d-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b694d-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b694d-139">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="b694d-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b694d-140">C#</span><span class="sxs-lookup"><span data-stu-id="b694d-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_mailfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b694d-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="b694d-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_mailfolder-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b694d-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b694d-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_mailfolder-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/mailfolder-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
