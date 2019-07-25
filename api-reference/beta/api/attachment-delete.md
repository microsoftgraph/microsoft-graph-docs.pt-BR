---
title: Excluir anexo
description: Excluir um anexo de um evento de calendário, mensagem, tarefa do Outlook ou postagem.
localization_priority: Normal
ms.openlocfilehash: cc45d4ddd89cbf2f431de3d2107255e208797f46
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856601"
---
# <a name="delete-attachment"></a><span data-ttu-id="1bcc6-103">Excluir anexo</span><span class="sxs-lookup"><span data-stu-id="1bcc6-103">Delete attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bcc6-104">Excluir um anexo de um [evento](../resources/event.md)de calendário, [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postagem](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="1bcc6-104">Delete an attachment from a calendar [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1bcc6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1bcc6-105">Permissions</span></span>

<span data-ttu-id="1bcc6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bcc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="1bcc6-108">Se estiver acessando anexos em mensagens: mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1bcc6-108">If accessing attachments in messages: Mail.ReadWrite</span></span>
* <span data-ttu-id="1bcc6-109">Se estiver acessando anexos em eventos: Calendars. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1bcc6-109">If accessing attachments in events: Calendars.ReadWrite</span></span>
* <span data-ttu-id="1bcc6-110">Se estiver acessando anexos em tarefas do Outlook: Tasks. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1bcc6-110">If accessing attachments in Outlook tasks: Tasks.ReadWrite</span></span>
* <span data-ttu-id="1bcc6-111">Se estiver acessando anexos em Postagens de Grupo: Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1bcc6-111">If accessing attachments in group posts: Group.ReadWrite.All</span></span>

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All
-->

## <a name="http-request"></a><span data-ttu-id="1bcc6-112">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1bcc6-112">HTTP request</span></span>

<span data-ttu-id="1bcc6-113">Anexos de um [evento](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="1bcc6-113">Attachments for an [event](../resources/event.md).</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}
```

<!--
DELETE /groups/{id}/events/{id}/attachments/{id}
-->

<span data-ttu-id="1bcc6-114">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="1bcc6-114">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```

<span data-ttu-id="1bcc6-115">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="1bcc6-115">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="1bcc6-p102">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="1bcc6-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. </span></span><!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="1bcc6-118">Anexos de uma [tarefa do Outlook](../resources/outlooktask.md).</span><span class="sxs-lookup"><span data-stu-id="1bcc6-118">Attachments for an [Outlook task](../resources/outlooktask.md).</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/<id>/attachments/{id}
DELETE /users/<id>/outlook/tasks/<id>/attachments/{id}
```

<span data-ttu-id="1bcc6-119">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="1bcc6-119">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1bcc6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1bcc6-120">Request headers</span></span>

| <span data-ttu-id="1bcc6-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1bcc6-121">Name</span></span>       | <span data-ttu-id="1bcc6-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="1bcc6-122">Type</span></span> | <span data-ttu-id="1bcc6-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bcc6-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1bcc6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1bcc6-124">Authorization</span></span>  | <span data-ttu-id="1bcc6-125">string</span><span class="sxs-lookup"><span data-stu-id="1bcc6-125">string</span></span>  | <span data-ttu-id="1bcc6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bcc6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1bcc6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1bcc6-128">Request body</span></span>

<span data-ttu-id="1bcc6-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1bcc6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bcc6-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bcc6-130">Response</span></span>

<span data-ttu-id="1bcc6-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1bcc6-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bcc6-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1bcc6-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bcc6-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1bcc6-134">Request</span></span>

<span data-ttu-id="1bcc6-135">Veja um exemplo da solicitação para excluir um anexo em um evento.</span><span class="sxs-lookup"><span data-stu-id="1bcc6-135">Here is an example of the request to delete an attachment on an event.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1bcc6-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="1bcc6-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1bcc6-137">C#</span><span class="sxs-lookup"><span data-stu-id="1bcc6-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1bcc6-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="1bcc6-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1bcc6-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1bcc6-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1bcc6-140">Java</span><span class="sxs-lookup"><span data-stu-id="1bcc6-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1bcc6-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bcc6-141">Response</span></span>

<span data-ttu-id="1bcc6-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1bcc6-142">Here is an example of the response.</span></span>
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
  "description": "Delete attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
