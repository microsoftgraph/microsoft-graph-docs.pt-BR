---
title: Excluir mailFolder
description: Exclua o mailFolder especificado.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1effb7d8e0ba6a27ddbef979f85c6e1e81adcecd
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612619"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="15f4a-103">Excluir mailFolder</span><span class="sxs-lookup"><span data-stu-id="15f4a-103">Delete mailFolder</span></span>

<span data-ttu-id="15f4a-104">Exclua o [mailFolder](../resources/mailfolder.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="15f4a-104">Delete the specified [mailFolder](../resources/mailfolder.md).</span></span>

<span data-ttu-id="15f4a-105">Você pode especificar uma pasta de email por sua ID de pasta ou por seu [nome de pasta conhecido](../resources/mailfolder.md), se houver uma.</span><span class="sxs-lookup"><span data-stu-id="15f4a-105">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="15f4a-106">**Observação** Você pode não conseguir excluir itens da pasta exclusão de itens recuperáveis (representado pelo nome `recoverableitemsdeletions`de pasta conhecido).</span><span class="sxs-lookup"><span data-stu-id="15f4a-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="15f4a-107">Veja [retenção de item excluído](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) e [limpar itens excluídos](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="15f4a-107">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="15f4a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="15f4a-108">Permissions</span></span>
<span data-ttu-id="15f4a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15f4a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15f4a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15f4a-111">Permission type</span></span>      | <span data-ttu-id="15f4a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="15f4a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15f4a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15f4a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="15f4a-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15f4a-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="15f4a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15f4a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15f4a-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15f4a-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="15f4a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15f4a-117">Application</span></span> | <span data-ttu-id="15f4a-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15f4a-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="15f4a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15f4a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="15f4a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15f4a-120">Request headers</span></span>
| <span data-ttu-id="15f4a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="15f4a-121">Name</span></span>       | <span data-ttu-id="15f4a-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="15f4a-122">Type</span></span> | <span data-ttu-id="15f4a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="15f4a-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="15f4a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="15f4a-124">Authorization</span></span>  | <span data-ttu-id="15f4a-125">string</span><span class="sxs-lookup"><span data-stu-id="15f4a-125">string</span></span>  | <span data-ttu-id="15f4a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15f4a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15f4a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15f4a-128">Request body</span></span>
<span data-ttu-id="15f4a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="15f4a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15f4a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="15f4a-130">Response</span></span>

<span data-ttu-id="15f4a-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15f4a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15f4a-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15f4a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15f4a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15f4a-134">Request</span></span>
<span data-ttu-id="15f4a-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15f4a-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="15f4a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="15f4a-136">Response</span></span>
<span data-ttu-id="15f4a-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15f4a-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="15f4a-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="15f4a-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="15f4a-139">Basic</span><span class="sxs-lookup"><span data-stu-id="15f4a-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_mailfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="15f4a-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15f4a-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_mailfolder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/mailfolder-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/mailfolder-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
