---
title: Excluir anexo
description: Excluir um anexo de um evento de calendário, mensagem, tarefa do Outlook ou postagem.
localization_priority: Normal
doc_type: apiPageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: 14d012fbd33ce0ae29c700821822974fc0f5b316
ms.sourcegitcommit: 6deec57c0ab736260ee3599703bfd3f567ee6d82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2019
ms.locfileid: "37581221"
---
# <a name="delete-attachment"></a><span data-ttu-id="80394-103">Excluir anexo</span><span class="sxs-lookup"><span data-stu-id="80394-103">Delete attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80394-104">Excluir um anexo de um [evento](../resources/event.md)de calendário, [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postagem](../resources/post.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="80394-104">Delete an attachment from a user calendar [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="80394-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="80394-105">Permissions</span></span>

<span data-ttu-id="80394-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80394-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="80394-108">Se estiver acessando anexos em mensagens: mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80394-108">If accessing attachments in messages: Mail.ReadWrite</span></span>
* <span data-ttu-id="80394-109">Se estiver acessando anexos em eventos: Calendars. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80394-109">If accessing attachments in events: Calendars.ReadWrite</span></span>
* <span data-ttu-id="80394-110">Se estiver acessando anexos em tarefas do Outlook: Tasks. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80394-110">If accessing attachments in Outlook tasks: Tasks.ReadWrite</span></span>
* <span data-ttu-id="80394-111">Se estiver acessando anexos em Postagens de Grupo: Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="80394-111">If accessing attachments in group posts: Group.ReadWrite.All</span></span>

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All
-->

## <a name="http-request"></a><span data-ttu-id="80394-112">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80394-112">HTTP request</span></span>

<span data-ttu-id="80394-113">Anexos de um [evento](../resources/event.md) no [calendário](../resources/calendar.md)padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="80394-113">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}

DELETE /me/calendar/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}/attachments/{id}
```

<span data-ttu-id="80394-114">Anexos de um [evento](../resources/event.md) no [calendário](../resources/calendar.md) especificado pertencente ao usuário.</span><span class="sxs-lookup"><span data-stu-id="80394-114">Attachments for an [event](../resources/event.md) in the specified [calendar](../resources/calendar.md) belonging to the user.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}
```

<!-- Tried adding and getting group event with attachment, event exists but without attachment. Group event attachment not supported.
DELETE /groups/{id}/events/{id}/attachments/{id}
DELETE /groups/{id}/calendar/events/{id}/attachments/{id}
-->

<span data-ttu-id="80394-115">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence ao [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="80394-115">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="80394-116">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence a um [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="80394-116">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="80394-117">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="80394-117">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```

<span data-ttu-id="80394-118">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="80394-118">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="80394-p102">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="80394-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. </span></span><!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="80394-121">Anexos de uma [tarefa do Outlook](../resources/outlooktask.md).</span><span class="sxs-lookup"><span data-stu-id="80394-121">Attachments for an [Outlook task](../resources/outlooktask.md).</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/{id}/attachments/{id}
DELETE /users/{id}/outlook/tasks/{id}/attachments/{id}
```

<span data-ttu-id="80394-122">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="80394-122">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="80394-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80394-123">Request headers</span></span>

| <span data-ttu-id="80394-124">Nome</span><span class="sxs-lookup"><span data-stu-id="80394-124">Name</span></span>       | <span data-ttu-id="80394-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="80394-125">Type</span></span> | <span data-ttu-id="80394-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="80394-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="80394-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="80394-127">Authorization</span></span>  | <span data-ttu-id="80394-128">string</span><span class="sxs-lookup"><span data-stu-id="80394-128">string</span></span>  | <span data-ttu-id="80394-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80394-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80394-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80394-131">Request body</span></span>

<span data-ttu-id="80394-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="80394-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80394-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="80394-133">Response</span></span>

<span data-ttu-id="80394-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80394-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80394-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80394-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="80394-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80394-137">Request</span></span>

<span data-ttu-id="80394-138">Veja um exemplo da solicitação para excluir um anexo em um evento.</span><span class="sxs-lookup"><span data-stu-id="80394-138">Here is an example of the request to delete an attachment on an event.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="80394-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="80394-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="80394-140">C#</span><span class="sxs-lookup"><span data-stu-id="80394-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="80394-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80394-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="80394-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80394-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="80394-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="80394-143">Response</span></span>

<span data-ttu-id="80394-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80394-144">Here is an example of the response.</span></span>
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
