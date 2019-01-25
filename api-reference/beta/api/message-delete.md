---
title: Excluir mensagem
description: Excluir uma mensagem na caixa de correio do usuário especificado ou excluir uma relação da mensagem.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 1237ba7e4aa5ab0439af9f07902705e7b4061374
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513540"
---
# <a name="delete-message"></a><span data-ttu-id="f4f8f-103">Excluir mensagem</span><span class="sxs-lookup"><span data-stu-id="f4f8f-103">Delete message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4f8f-104">Excluir uma mensagem na caixa de correio do usuário especificado ou excluir uma relação da mensagem.</span><span class="sxs-lookup"><span data-stu-id="f4f8f-104">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

<span data-ttu-id="f4f8f-105">Por exemplo, você pode excluir um [@ mencionam](../resources/mention.md) específica do usuário especificado na mensagem.</span><span class="sxs-lookup"><span data-stu-id="f4f8f-105">For example, you can delete a specific [@-mention](../resources/mention.md) of the specified user in the message.</span></span>

><span data-ttu-id="f4f8f-106">**Observação** Você não poderá excluir itens na pasta itens recuperáveis exclusões (representado pelo [nome da pasta conhecido](../resources/mailfolder.md) `recoverableitemsdeletions`).</span><span class="sxs-lookup"><span data-stu-id="f4f8f-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="f4f8f-107">Para obter mais informações, consulte [retenção de itens excluídos](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) e [Limpar itens excluídos](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="f4f8f-107">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4f8f-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f4f8f-108">Permissions</span></span>
<span data-ttu-id="f4f8f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4f8f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4f8f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4f8f-111">Permission type</span></span>      | <span data-ttu-id="f4f8f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f4f8f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4f8f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4f8f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f4f8f-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f4f8f-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f4f8f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4f8f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4f8f-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f4f8f-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f4f8f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4f8f-117">Application</span></span> | <span data-ttu-id="f4f8f-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f4f8f-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4f8f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4f8f-119">HTTP request</span></span>

<span data-ttu-id="f4f8f-120">Para excluir a mensagem especificada:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="f4f8f-120">To delete the specified message: <!-- { "blockType": "ignored" } --></span></span>
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="f4f8f-121">Para excluir um específicos [mencionar](../resources/mention.md) em uma mensagem:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="f4f8f-121">To delete a specific [mention](../resources/mention.md) in a message: <!-- { "blockType": "ignored" } --></span></span>
```http
DELETE /me/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/mentions/{id}
DELETE /me/mailFolders/{id}/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/mentions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f4f8f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4f8f-122">Request headers</span></span>
| <span data-ttu-id="f4f8f-123">Nome</span><span class="sxs-lookup"><span data-stu-id="f4f8f-123">Name</span></span>       | <span data-ttu-id="f4f8f-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4f8f-124">Type</span></span> | <span data-ttu-id="f4f8f-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4f8f-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f4f8f-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4f8f-126">Authorization</span></span>  | <span data-ttu-id="f4f8f-127">string</span><span class="sxs-lookup"><span data-stu-id="f4f8f-127">string</span></span>  | <span data-ttu-id="f4f8f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4f8f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4f8f-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4f8f-130">Request body</span></span>
<span data-ttu-id="f4f8f-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f4f8f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4f8f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4f8f-132">Response</span></span>

<span data-ttu-id="f4f8f-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4f8f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4f8f-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4f8f-135">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="f4f8f-136">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="f4f8f-136">Request 1</span></span>
<span data-ttu-id="f4f8f-137">O primeiro exemplo exclui a mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="f4f8f-137">The first example deletes the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
##### <a name="response-1"></a><span data-ttu-id="f4f8f-138">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="f4f8f-138">Response 1</span></span>
<span data-ttu-id="f4f8f-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4f8f-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="request-2"></a><span data-ttu-id="f4f8f-140">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="f4f8f-140">Request 2</span></span>
<span data-ttu-id="f4f8f-141">O exemplo a seguir exclui uma determinada **mencionar** na mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="f4f8f-141">The next example deletes a certain **mention** in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mention_in_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}/mentions/{id}
```
##### <a name="response-2"></a><span data-ttu-id="f4f8f-142">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="f4f8f-142">Response 2</span></span>
<span data-ttu-id="f4f8f-143">Este é um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4f8f-143">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
