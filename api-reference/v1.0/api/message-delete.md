---
title: Excluir mensagem
description: Excluir uma mensagem na caixa de correio do usuário especificado ou excluir uma relação da mensagem.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: cb9e6fd563688fc422bcaf748d931daf97c74985
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565069"
---
# <a name="delete-message"></a><span data-ttu-id="52579-103">Excluir mensagem</span><span class="sxs-lookup"><span data-stu-id="52579-103">Delete message</span></span>

<span data-ttu-id="52579-104">Excluir uma mensagem na caixa de correio do usuário especificado ou excluir uma relação da mensagem.</span><span class="sxs-lookup"><span data-stu-id="52579-104">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

><span data-ttu-id="52579-105">**Observação** Você pode não conseguir excluir itens da pasta exclusão de itens recuperáveis (representado pelo [nome](../resources/mailfolder.md) `recoverableitemsdeletions`de pasta conhecido).</span><span class="sxs-lookup"><span data-stu-id="52579-105">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="52579-106">Veja [retenção de item excluído](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) e [limpar itens excluídos](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="52579-106">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="52579-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="52579-107">Permissions</span></span>
<span data-ttu-id="52579-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52579-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52579-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52579-110">Permission type</span></span>      | <span data-ttu-id="52579-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52579-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52579-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52579-112">Delegated (work or school account)</span></span> | <span data-ttu-id="52579-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52579-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="52579-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52579-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52579-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52579-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="52579-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52579-116">Application</span></span> | <span data-ttu-id="52579-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52579-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="52579-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52579-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="52579-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52579-119">Request headers</span></span>
| <span data-ttu-id="52579-120">Nome</span><span class="sxs-lookup"><span data-stu-id="52579-120">Name</span></span>       | <span data-ttu-id="52579-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="52579-121">Type</span></span> | <span data-ttu-id="52579-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="52579-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="52579-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="52579-123">Authorization</span></span>  | <span data-ttu-id="52579-124">string</span><span class="sxs-lookup"><span data-stu-id="52579-124">string</span></span>  | <span data-ttu-id="52579-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52579-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52579-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52579-127">Request body</span></span>
<span data-ttu-id="52579-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="52579-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52579-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="52579-129">Response</span></span>

<span data-ttu-id="52579-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52579-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52579-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52579-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="52579-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52579-133">Request</span></span>
<span data-ttu-id="52579-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52579-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="52579-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="52579-135">Response</span></span>
<span data-ttu-id="52579-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52579-136">Here is an example of the response.</span></span> 
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
