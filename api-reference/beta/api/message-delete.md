---
title: Excluir mensagem
description: Excluir uma mensagem na caixa de correio do usuário especificado ou excluir uma relação da mensagem.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 8ef6636e98d516bab1dea29c37dcc23caa7a01ed
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942441"
---
# <a name="delete-message"></a><span data-ttu-id="a586a-103">Excluir mensagem</span><span class="sxs-lookup"><span data-stu-id="a586a-103">Delete message</span></span>

> <span data-ttu-id="a586a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a586a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a586a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a586a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a586a-106">Excluir uma mensagem na caixa de correio do usuário especificado ou excluir uma relação da mensagem.</span><span class="sxs-lookup"><span data-stu-id="a586a-106">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

<span data-ttu-id="a586a-107">Por exemplo, você pode excluir um [@ mencionam](../resources/mention.md) específica do usuário especificado na mensagem.</span><span class="sxs-lookup"><span data-stu-id="a586a-107">For example, you can delete a specific [@-mention](../resources/mention.md) of the specified user in the message.</span></span>

><span data-ttu-id="a586a-108">**Observação** Você não poderá excluir itens na pasta itens recuperáveis exclusões (representado pelo [nome da pasta conhecido](../resources/mailfolder.md) `recoverableitemsdeletions`).</span><span class="sxs-lookup"><span data-stu-id="a586a-108">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="a586a-109">Para obter mais informações, consulte [retenção de itens excluídos](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) e [Limpar itens excluídos](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="a586a-109">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="a586a-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="a586a-110">Permissions</span></span>
<span data-ttu-id="a586a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a586a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a586a-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a586a-113">Permission type</span></span>      | <span data-ttu-id="a586a-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a586a-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a586a-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a586a-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a586a-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a586a-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a586a-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a586a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a586a-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a586a-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a586a-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a586a-119">Application</span></span> | <span data-ttu-id="a586a-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a586a-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a586a-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a586a-121">HTTP request</span></span>

<span data-ttu-id="a586a-122">Para excluir a mensagem especificada:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="a586a-122">To delete the specified message: <!-- { "blockType": "ignored" } --></span></span>
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="a586a-123">Para excluir um específicos [mencionar](../resources/mention.md) em uma mensagem:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="a586a-123">To delete a specific [mention](../resources/mention.md) in a message: <!-- { "blockType": "ignored" } --></span></span>
```http
DELETE /me/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/mentions/{id}
DELETE /me/mailFolders/{id}/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/mentions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a586a-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a586a-124">Request headers</span></span>
| <span data-ttu-id="a586a-125">Nome</span><span class="sxs-lookup"><span data-stu-id="a586a-125">Name</span></span>       | <span data-ttu-id="a586a-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="a586a-126">Type</span></span> | <span data-ttu-id="a586a-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a586a-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a586a-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="a586a-128">Authorization</span></span>  | <span data-ttu-id="a586a-129">string</span><span class="sxs-lookup"><span data-stu-id="a586a-129">string</span></span>  | <span data-ttu-id="a586a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a586a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a586a-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a586a-132">Request body</span></span>
<span data-ttu-id="a586a-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a586a-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a586a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a586a-134">Response</span></span>

<span data-ttu-id="a586a-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a586a-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a586a-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a586a-137">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="a586a-138">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="a586a-138">Request 1</span></span>
<span data-ttu-id="a586a-139">O primeiro exemplo exclui a mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="a586a-139">The first example deletes the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
##### <a name="response-1"></a><span data-ttu-id="a586a-140">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="a586a-140">Response 1</span></span>
<span data-ttu-id="a586a-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a586a-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="request-2"></a><span data-ttu-id="a586a-142">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="a586a-142">Request 2</span></span>
<span data-ttu-id="a586a-143">O exemplo a seguir exclui uma determinada **mencionar** na mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="a586a-143">The next example deletes a certain **mention** in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mention_in_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}/mentions/{id}
```
##### <a name="response-2"></a><span data-ttu-id="a586a-144">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="a586a-144">Response 2</span></span>
<span data-ttu-id="a586a-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a586a-145">Here is an example of the response.</span></span> 
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
