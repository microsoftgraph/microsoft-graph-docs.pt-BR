---
title: Excluir anexo
description: Exclua um anexo de um evento de calendário, email ou postagem de grupo.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 78b8fd39741fb58b4386a70bc463de2cf4a4d546
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347714"
---
# <a name="delete-attachment"></a><span data-ttu-id="9e550-103">Excluir anexo</span><span class="sxs-lookup"><span data-stu-id="9e550-103">Delete attachment</span></span>

<span data-ttu-id="9e550-104">Exclua um anexo de um evento de calendário, email ou postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="9e550-104">Delete an attachment from a calendar event, mail message, or group post.</span></span>
## <a name="permissions"></a><span data-ttu-id="9e550-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9e550-105">Permissions</span></span>
<span data-ttu-id="9e550-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e550-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="9e550-108">Se estiver acessando anexos em mensagens: mail. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="9e550-108">If accessing attachments in messages: Mail.ReadWrite.</span></span>
* <span data-ttu-id="9e550-109">Se estiver acessando anexos em eventos: Calendars. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="9e550-109">If accessing attachments in events: Calendars.ReadWrite.</span></span>
* <span data-ttu-id="9e550-110">Se estiver acessando anexos em Postagens de Grupo: Group. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="9e550-110">If accessing attachments in group posts: Group.ReadWrite.All.</span></span>

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All.
-->

## <a name="http-request"></a><span data-ttu-id="9e550-111">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e550-111">HTTP request</span></span>
<span data-ttu-id="9e550-112">Anexos de um [event](../resources/event.md) no [calendar](../resources/calendar.md) padrão do usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="9e550-112">Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}

DELETE /me/calendar/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}/attachments/{id}
```

<!--
DELETE /groups/{id}/events/{id}/attachments/{id}
DELETE /groups/{id}/calendar/events/{id}/attachments/{id}
-->

<span data-ttu-id="9e550-113">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence ao [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="9e550-113">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="9e550-114">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence a um [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="9e550-114">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="9e550-115">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="9e550-115">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="9e550-116">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="9e550-116">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="9e550-p102">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="9e550-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. </span></span><!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="9e550-119">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="9e550-119">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9e550-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e550-120">Request headers</span></span>
| <span data-ttu-id="9e550-121">Nome</span><span class="sxs-lookup"><span data-stu-id="9e550-121">Name</span></span>       | <span data-ttu-id="9e550-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e550-122">Type</span></span> | <span data-ttu-id="9e550-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e550-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9e550-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e550-124">Authorization</span></span>  | <span data-ttu-id="9e550-125">string</span><span class="sxs-lookup"><span data-stu-id="9e550-125">string</span></span>  | <span data-ttu-id="9e550-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e550-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e550-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e550-128">Request body</span></span>
<span data-ttu-id="9e550-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9e550-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e550-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e550-130">Response</span></span>

<span data-ttu-id="9e550-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e550-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e550-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e550-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e550-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e550-134">Request</span></span>
<span data-ttu-id="9e550-135">Veja um exemplo da solicitação para excluir um anexo em um evento.</span><span class="sxs-lookup"><span data-stu-id="9e550-135">Here is an example of the request to delete an attachment on an event.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9e550-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e550-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9e550-137">C#</span><span class="sxs-lookup"><span data-stu-id="9e550-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9e550-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e550-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9e550-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9e550-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9e550-140">Java</span><span class="sxs-lookup"><span data-stu-id="9e550-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9e550-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e550-141">Response</span></span>
<span data-ttu-id="9e550-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e550-142">Here is an example of the response.</span></span>
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
