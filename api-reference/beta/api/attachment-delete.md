---
title: Excluir anexo
description: Excluir um anexo de um evento de calendário
ms.openlocfilehash: 5e5fe0205e667908947993b01388f90c1688c95e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033717"
---
# <a name="delete-attachment"></a><span data-ttu-id="806ee-103">Excluir anexo</span><span class="sxs-lookup"><span data-stu-id="806ee-103">Delete attachment</span></span>

> <span data-ttu-id="806ee-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="806ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="806ee-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="806ee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="806ee-106">Exclua um anexo de um [evento](../resources/event.md)do calendário, [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postar](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="806ee-106">Delete an attachment from a calendar [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="806ee-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="806ee-107">Permissions</span></span>
<span data-ttu-id="806ee-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="806ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="806ee-110">Se acessando anexos em mensagens: Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="806ee-110">If accessing attachments in messages: Mail.ReadWrite</span></span>
* <span data-ttu-id="806ee-111">Se acessando anexos em eventos: Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="806ee-111">If accessing attachments in events: Calendars.ReadWrite</span></span>
* <span data-ttu-id="806ee-112">Se acessando anexos em tarefas do Outlook: Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="806ee-112">If accessing attachments in Outlook tasks: Tasks.ReadWrite</span></span>
* <span data-ttu-id="806ee-113">Se acessando anexos em postagens de grupo: Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="806ee-113">If accessing attachments in group posts: Group.ReadWrite.All</span></span>
<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All
-->

## <a name="http-request"></a><span data-ttu-id="806ee-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="806ee-114">HTTP request</span></span>
<span data-ttu-id="806ee-115">Anexos em um [evento](../resources/event.md) do usuário padrão [calendário](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="806ee-115">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

<!--
Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).
-->
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

<span data-ttu-id="806ee-116">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence ao [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="806ee-116">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="806ee-117">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence a um [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="806ee-117">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="806ee-118">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="806ee-118">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="806ee-119">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="806ee-119">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="806ee-120">Anexos de uma [mensagem](../resources/message.md) contidos em uma pasta filho de um [mailFolder](../resources/mailfolder.md) na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="806ee-120">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>  <span data-ttu-id="806ee-121">O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada no filho de um filho e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="806ee-121">The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="806ee-122">Anexos para uma [tarefa do Outlook](../resources/outlooktask.md) na caixa de correio do usuário ou em uma pasta de tarefas especificado ou o grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="806ee-122">Attachments for an [Outlook task](../resources/outlooktask.md) in the user's mailbox, or in a specified task folder or task group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/tasks/<id>/attachments/{id}
DELETE /users/<id>/outlook/tasks/<id>/attachments/{id}

DELETE /me/outlook/taskFolders/<id>/tasks/<id>/attachments/{id}
DELETE /users/<id>/outlook/taskFolders/<id>/tasks/<id>/attachments/{id}

DELETE /me/outlook/taskGroups/<id>/taskFolders/<id>/tasks/<id>/attachments/{id}
DELETE /users/<id>/outlook/taskGroups/<id>/taskFolders/<id>/tasks/<id>/attachments/{id}
```

<span data-ttu-id="806ee-123">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="806ee-123">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="806ee-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="806ee-124">Request headers</span></span>
| <span data-ttu-id="806ee-125">Nome</span><span class="sxs-lookup"><span data-stu-id="806ee-125">Name</span></span>       | <span data-ttu-id="806ee-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="806ee-126">Type</span></span> | <span data-ttu-id="806ee-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="806ee-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="806ee-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="806ee-128">Authorization</span></span>  | <span data-ttu-id="806ee-129">string</span><span class="sxs-lookup"><span data-stu-id="806ee-129">string</span></span>  | <span data-ttu-id="806ee-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="806ee-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="806ee-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="806ee-132">Request body</span></span>
<span data-ttu-id="806ee-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="806ee-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="806ee-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="806ee-134">Response</span></span>

<span data-ttu-id="806ee-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="806ee-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="806ee-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="806ee-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="806ee-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="806ee-138">Request</span></span>
<span data-ttu-id="806ee-139">Veja um exemplo da solicitação para excluir um anexo em um evento.</span><span class="sxs-lookup"><span data-stu-id="806ee-139">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```
##### <a name="response"></a><span data-ttu-id="806ee-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="806ee-140">Response</span></span>
<span data-ttu-id="806ee-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="806ee-141">Here is an example of the response.</span></span>
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
