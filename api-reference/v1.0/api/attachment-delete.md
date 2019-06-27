---
title: Excluir anexo
description: Exclua um anexo de um evento de calendário, email ou postagem de grupo.
localization_priority: Normal
ms.openlocfilehash: aa1a031826c4e0875007ba63ea8cf21695d8e49b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272664"
---
# <a name="delete-attachment"></a><span data-ttu-id="8d3b8-103">Excluir anexo</span><span class="sxs-lookup"><span data-stu-id="8d3b8-103">Delete attachment</span></span>

<span data-ttu-id="8d3b8-104">Exclua um anexo de um evento de calendário, email ou postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="8d3b8-104">Delete an attachment from a calendar event, mail message, or group post.</span></span>
## <a name="permissions"></a><span data-ttu-id="8d3b8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8d3b8-105">Permissions</span></span>
<span data-ttu-id="8d3b8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d3b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="8d3b8-108">Se estiver acessando anexos em mensagens: mail. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="8d3b8-108">If accessing attachments in messages: Mail.ReadWrite.</span></span>
* <span data-ttu-id="8d3b8-109">Se estiver acessando anexos em eventos: Calendars. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="8d3b8-109">If accessing attachments in events: Calendars.ReadWrite.</span></span>
* <span data-ttu-id="8d3b8-110">Se estiver acessando anexos em Postagens de Grupo: Group. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="8d3b8-110">If accessing attachments in group posts: Group.ReadWrite.All.</span></span>

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All.
-->

## <a name="http-request"></a><span data-ttu-id="8d3b8-111">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d3b8-111">HTTP request</span></span>
<span data-ttu-id="8d3b8-112">Anexos de um [event](../resources/event.md) no [calendar](../resources/calendar.md) padrão do usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="8d3b8-112">Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).</span></span>
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

<span data-ttu-id="8d3b8-113">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence ao [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="8d3b8-113">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="8d3b8-114">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence a um [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="8d3b8-114">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="8d3b8-115">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="8d3b8-115">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="8d3b8-116">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="8d3b8-116">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="8d3b8-p102">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="8d3b8-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. </span></span><!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="8d3b8-119">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="8d3b8-119">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8d3b8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d3b8-120">Request headers</span></span>
| <span data-ttu-id="8d3b8-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8d3b8-121">Name</span></span>       | <span data-ttu-id="8d3b8-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d3b8-122">Type</span></span> | <span data-ttu-id="8d3b8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d3b8-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8d3b8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d3b8-124">Authorization</span></span>  | <span data-ttu-id="8d3b8-125">string</span><span class="sxs-lookup"><span data-stu-id="8d3b8-125">string</span></span>  | <span data-ttu-id="8d3b8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d3b8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d3b8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d3b8-128">Request body</span></span>
<span data-ttu-id="8d3b8-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8d3b8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d3b8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d3b8-130">Response</span></span>

<span data-ttu-id="8d3b8-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d3b8-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d3b8-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d3b8-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8d3b8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d3b8-134">Request</span></span>
<span data-ttu-id="8d3b8-135">Veja um exemplo da solicitação para excluir um anexo em um evento.</span><span class="sxs-lookup"><span data-stu-id="8d3b8-135">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
##### <a name="response"></a><span data-ttu-id="8d3b8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d3b8-136">Response</span></span>
<span data-ttu-id="8d3b8-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d3b8-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8d3b8-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="8d3b8-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8d3b8-139">C#</span><span class="sxs-lookup"><span data-stu-id="8d3b8-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_attachment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8d3b8-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="8d3b8-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_attachment-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8d3b8-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8d3b8-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_attachment-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/attachment-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/attachment-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/attachment-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
