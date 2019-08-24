---
title: Excluir anexo
description: Exclua um anexo de um evento de calendário, email ou postagem de grupo.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8482bdc9a19ea1ba5febc805970e0faca83446e3
ms.sourcegitcommit: 83a053067f6248fb49ec5d473738ab1555fb4295
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/24/2019
ms.locfileid: "36622541"
---
# <a name="delete-attachment"></a><span data-ttu-id="62f7b-103">Excluir anexo</span><span class="sxs-lookup"><span data-stu-id="62f7b-103">Delete attachment</span></span>

<span data-ttu-id="62f7b-104">Excluir um anexo de um evento de calendário de usuário, mensagem de email ou postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="62f7b-104">Delete an attachment from a user calendar event, mail message, or group post.</span></span>
## <a name="permissions"></a><span data-ttu-id="62f7b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="62f7b-105">Permissions</span></span>
<span data-ttu-id="62f7b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62f7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="62f7b-108">Se estiver acessando anexos em mensagens: mail. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="62f7b-108">If accessing attachments in messages: Mail.ReadWrite.</span></span>
* <span data-ttu-id="62f7b-109">Se estiver acessando anexos em eventos: Calendars. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="62f7b-109">If accessing attachments in events: Calendars.ReadWrite.</span></span>
* <span data-ttu-id="62f7b-110">Se estiver acessando anexos em Postagens de Grupo: Group. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="62f7b-110">If accessing attachments in group posts: Group.ReadWrite.All.</span></span>

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All.
-->

## <a name="http-request"></a><span data-ttu-id="62f7b-111">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62f7b-111">HTTP request</span></span>
<span data-ttu-id="62f7b-112">Anexos de um [evento](../resources/event.md) no [calendário](../resources/calendar.md)padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="62f7b-112">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}

DELETE /me/calendar/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}/attachments/{id}
```

<span data-ttu-id="62f7b-113">Anexos de um [evento](../resources/event.md) no [calendário](../resources/calendar.md) especificado pertencente ao usuário.</span><span class="sxs-lookup"><span data-stu-id="62f7b-113">Attachments for an [event](../resources/event.md) in the specified [calendar](../resources/calendar.md) belonging to the user.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}
```

<!-- Tried adding and getting group event with attachment, event exists but without attachment. Assume group event attachment not supported.
DELETE /groups/{id}/events/{id}/attachments/{id}
DELETE /groups/{id}/calendar/events/{id}/attachments/{id}
-->

<span data-ttu-id="62f7b-114">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence ao [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="62f7b-114">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="62f7b-115">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence a um [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="62f7b-115">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="62f7b-116">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="62f7b-116">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="62f7b-117">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="62f7b-117">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="62f7b-p102">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="62f7b-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. </span></span><!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="62f7b-120">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="62f7b-120">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="62f7b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62f7b-121">Request headers</span></span>
| <span data-ttu-id="62f7b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="62f7b-122">Name</span></span>       | <span data-ttu-id="62f7b-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="62f7b-123">Type</span></span> | <span data-ttu-id="62f7b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="62f7b-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="62f7b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="62f7b-125">Authorization</span></span>  | <span data-ttu-id="62f7b-126">string</span><span class="sxs-lookup"><span data-stu-id="62f7b-126">string</span></span>  | <span data-ttu-id="62f7b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62f7b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62f7b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62f7b-129">Request body</span></span>
<span data-ttu-id="62f7b-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="62f7b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62f7b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="62f7b-131">Response</span></span>

<span data-ttu-id="62f7b-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62f7b-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62f7b-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62f7b-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="62f7b-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62f7b-135">Request</span></span>
<span data-ttu-id="62f7b-136">Veja um exemplo da solicitação para excluir um anexo em um evento.</span><span class="sxs-lookup"><span data-stu-id="62f7b-136">Here is an example of the request to delete an attachment on an event.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="62f7b-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="62f7b-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="62f7b-138">C#</span><span class="sxs-lookup"><span data-stu-id="62f7b-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="62f7b-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62f7b-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="62f7b-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="62f7b-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="62f7b-141">Java</span><span class="sxs-lookup"><span data-stu-id="62f7b-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="62f7b-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="62f7b-142">Response</span></span>
<span data-ttu-id="62f7b-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62f7b-143">Here is an example of the response.</span></span>
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
  "description": "Delete attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
