---
title: Excluir mensagem
description: Excluir uma mensagem na caixa de correio do usuário especificado ou excluir uma relação da mensagem.
localization_priority: Normal
ms.openlocfilehash: 3a76c936f72ebd238ee6d7a898dfd6a3e0356036
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864523"
---
# <a name="delete-message"></a><span data-ttu-id="e259e-103">Excluir mensagem</span><span class="sxs-lookup"><span data-stu-id="e259e-103">Delete message</span></span>

> <span data-ttu-id="e259e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e259e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e259e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e259e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e259e-106">Excluir uma mensagem na caixa de correio do usuário especificado ou excluir uma relação da mensagem.</span><span class="sxs-lookup"><span data-stu-id="e259e-106">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

<span data-ttu-id="e259e-107">Por exemplo, você pode excluir um [@ mencionam](../resources/mention.md) específica do usuário especificado na mensagem.</span><span class="sxs-lookup"><span data-stu-id="e259e-107">For example, you can delete a specific [@-mention](../resources/mention.md) of the specified user in the message.</span></span>

><span data-ttu-id="e259e-108">**Observação** Você não poderá excluir itens na pasta itens recuperáveis exclusões (representado pelo [nome da pasta conhecido](../resources/mailfolder.md) `recoverableitemsdeletions`).</span><span class="sxs-lookup"><span data-stu-id="e259e-108">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="e259e-109">Para obter mais informações, consulte [retenção de itens excluídos](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) e [Limpar itens excluídos](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="e259e-109">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="e259e-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="e259e-110">Permissions</span></span>
<span data-ttu-id="e259e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e259e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e259e-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e259e-113">Permission type</span></span>      | <span data-ttu-id="e259e-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e259e-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e259e-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e259e-115">Delegated (work or school account)</span></span> | <span data-ttu-id="e259e-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e259e-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e259e-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e259e-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e259e-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e259e-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e259e-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e259e-119">Application</span></span> | <span data-ttu-id="e259e-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e259e-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e259e-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e259e-121">HTTP request</span></span>

<span data-ttu-id="e259e-122">Para excluir a mensagem especificada:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="e259e-122">To delete the specified message: <!-- { "blockType": "ignored" } --></span></span>
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="e259e-123">Para excluir um específicos [mencionar](../resources/mention.md) em uma mensagem:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="e259e-123">To delete a specific [mention](../resources/mention.md) in a message: <!-- { "blockType": "ignored" } --></span></span>
```http
DELETE /me/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/mentions/{id}
DELETE /me/mailFolders/{id}/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/mentions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e259e-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e259e-124">Request headers</span></span>
| <span data-ttu-id="e259e-125">Nome</span><span class="sxs-lookup"><span data-stu-id="e259e-125">Name</span></span>       | <span data-ttu-id="e259e-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="e259e-126">Type</span></span> | <span data-ttu-id="e259e-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="e259e-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e259e-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="e259e-128">Authorization</span></span>  | <span data-ttu-id="e259e-129">string</span><span class="sxs-lookup"><span data-stu-id="e259e-129">string</span></span>  | <span data-ttu-id="e259e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e259e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e259e-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e259e-132">Request body</span></span>
<span data-ttu-id="e259e-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e259e-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e259e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e259e-134">Response</span></span>

<span data-ttu-id="e259e-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e259e-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e259e-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e259e-137">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="e259e-138">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="e259e-138">Request 1</span></span>
<span data-ttu-id="e259e-139">O primeiro exemplo exclui a mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="e259e-139">The first example deletes the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
##### <a name="response-1"></a><span data-ttu-id="e259e-140">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="e259e-140">Response 1</span></span>
<span data-ttu-id="e259e-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e259e-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="request-2"></a><span data-ttu-id="e259e-142">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="e259e-142">Request 2</span></span>
<span data-ttu-id="e259e-143">O exemplo a seguir exclui uma determinada **mencionar** na mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="e259e-143">The next example deletes a certain **mention** in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mention_in_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}/mentions/{id}
```
##### <a name="response-2"></a><span data-ttu-id="e259e-144">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="e259e-144">Response 2</span></span>
<span data-ttu-id="e259e-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e259e-145">Here is an example of the response.</span></span> 
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
