---
title: Excluir anexo
description: Exclua um anexo de um evento de calendário, email ou postagem de grupo.
localization_priority: Normal
ms.openlocfilehash: f6ac2e60c9fdc8a224e22a49e6928cdc41e9730b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551460"
---
# <a name="delete-attachment"></a><span data-ttu-id="db6f5-103">Excluir anexo</span><span class="sxs-lookup"><span data-stu-id="db6f5-103">Delete attachment</span></span>

<span data-ttu-id="db6f5-104">Exclua um anexo de um evento de calendário, email ou postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="db6f5-104">Delete an attachment from a calendar event, mail message, or group post.</span></span>
## <a name="permissions"></a><span data-ttu-id="db6f5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="db6f5-105">Permissions</span></span>
<span data-ttu-id="db6f5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db6f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="db6f5-108">Se estiver acessando anexos em mensagens: mail. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="db6f5-108">If accessing attachments in messages: Mail.ReadWrite.</span></span>
* <span data-ttu-id="db6f5-109">Se estiver acessando anexos em eventos: caLendars. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="db6f5-109">If accessing attachments in events: Calendars.ReadWrite.</span></span>
* <span data-ttu-id="db6f5-110">Se estiver acessando anexos em Postagens de Grupo: Group. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="db6f5-110">If accessing attachments in group posts: Group.ReadWrite.All.</span></span>

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All.
-->

## <a name="http-request"></a><span data-ttu-id="db6f5-111">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db6f5-111">HTTP request</span></span>
<span data-ttu-id="db6f5-112">Anexos de um [event](../resources/event.md) no [calendar](../resources/calendar.md) padrão do usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="db6f5-112">Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).</span></span>
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

<span data-ttu-id="db6f5-113">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence ao [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="db6f5-113">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="db6f5-114">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence a um [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="db6f5-114">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="db6f5-115">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="db6f5-115">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="db6f5-116">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="db6f5-116">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="db6f5-p102">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="db6f5-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. </span></span><!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="db6f5-119">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="db6f5-119">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="db6f5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db6f5-120">Request headers</span></span>
| <span data-ttu-id="db6f5-121">Nome</span><span class="sxs-lookup"><span data-stu-id="db6f5-121">Name</span></span>       | <span data-ttu-id="db6f5-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="db6f5-122">Type</span></span> | <span data-ttu-id="db6f5-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="db6f5-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="db6f5-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="db6f5-124">Authorization</span></span>  | <span data-ttu-id="db6f5-125">string</span><span class="sxs-lookup"><span data-stu-id="db6f5-125">string</span></span>  | <span data-ttu-id="db6f5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db6f5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db6f5-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db6f5-128">Request body</span></span>
<span data-ttu-id="db6f5-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="db6f5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db6f5-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="db6f5-130">Response</span></span>

<span data-ttu-id="db6f5-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db6f5-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db6f5-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db6f5-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db6f5-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db6f5-134">Request</span></span>
<span data-ttu-id="db6f5-135">Veja um exemplo da solicitação para excluir um anexo em um evento.</span><span class="sxs-lookup"><span data-stu-id="db6f5-135">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
##### <a name="response"></a><span data-ttu-id="db6f5-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="db6f5-136">Response</span></span>
<span data-ttu-id="db6f5-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db6f5-137">Here is an example of the response.</span></span>
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
  "tocPath": ""
}-->
