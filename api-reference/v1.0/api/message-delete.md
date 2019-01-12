---
title: Excluir mensagem
description: Excluir uma mensagem na caixa de correio do usuário especificado ou excluir uma relação da mensagem.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: cb9e6fd563688fc422bcaf748d931daf97c74985
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984924"
---
# <a name="delete-message"></a><span data-ttu-id="62bfa-103">Excluir mensagem</span><span class="sxs-lookup"><span data-stu-id="62bfa-103">Delete message</span></span>

<span data-ttu-id="62bfa-104">Excluir uma mensagem na caixa de correio do usuário especificado ou excluir uma relação da mensagem.</span><span class="sxs-lookup"><span data-stu-id="62bfa-104">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

><span data-ttu-id="62bfa-105">**Observação** Você não poderá excluir itens na pasta itens recuperáveis exclusões (representado pelo [nome da pasta conhecido](../resources/mailfolder.md) `recoverableitemsdeletions`).</span><span class="sxs-lookup"><span data-stu-id="62bfa-105">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="62bfa-106">Para obter mais informações, consulte [retenção de itens excluídos](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) e [Limpar itens excluídos](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="62bfa-106">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="62bfa-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="62bfa-107">Permissions</span></span>
<span data-ttu-id="62bfa-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62bfa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62bfa-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62bfa-110">Permission type</span></span>      | <span data-ttu-id="62bfa-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="62bfa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62bfa-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62bfa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="62bfa-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="62bfa-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="62bfa-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62bfa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62bfa-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="62bfa-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="62bfa-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62bfa-116">Application</span></span> | <span data-ttu-id="62bfa-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="62bfa-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="62bfa-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62bfa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="62bfa-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62bfa-119">Request headers</span></span>
| <span data-ttu-id="62bfa-120">Nome</span><span class="sxs-lookup"><span data-stu-id="62bfa-120">Name</span></span>       | <span data-ttu-id="62bfa-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="62bfa-121">Type</span></span> | <span data-ttu-id="62bfa-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="62bfa-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="62bfa-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="62bfa-123">Authorization</span></span>  | <span data-ttu-id="62bfa-124">string</span><span class="sxs-lookup"><span data-stu-id="62bfa-124">string</span></span>  | <span data-ttu-id="62bfa-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62bfa-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62bfa-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62bfa-127">Request body</span></span>
<span data-ttu-id="62bfa-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="62bfa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62bfa-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="62bfa-129">Response</span></span>

<span data-ttu-id="62bfa-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62bfa-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62bfa-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62bfa-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="62bfa-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62bfa-133">Request</span></span>
<span data-ttu-id="62bfa-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="62bfa-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="62bfa-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="62bfa-135">Response</span></span>
<span data-ttu-id="62bfa-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62bfa-136">Here is an example of the response.</span></span> 
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
  "description": "Delete message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
