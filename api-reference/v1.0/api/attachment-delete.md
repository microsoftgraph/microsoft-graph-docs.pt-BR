---
title: Excluir anexo
description: Exclua um anexo de um evento de calendário, email ou postagem de grupo.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: db7f6282644443d459bba1655ecd01bce1955382
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434927"
---
# <a name="delete-attachment"></a><span data-ttu-id="2fd4e-103">Excluir anexo</span><span class="sxs-lookup"><span data-stu-id="2fd4e-103">Delete attachment</span></span>

<span data-ttu-id="2fd4e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fd4e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2fd4e-105">Exclua um anexo de um evento de calendário do usuário, mensagem de email ou postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="2fd4e-105">Delete an attachment from a user calendar event, mail message, or group post.</span></span>
## <a name="permissions"></a><span data-ttu-id="2fd4e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2fd4e-106">Permissions</span></span>

<span data-ttu-id="2fd4e-107">Dependendo do recurso (**evento** **,** mensagem , **outlookTask** ou **postagem**) ao qual o anexo está anexado e o tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é o mínimo privilegiado necessário para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="2fd4e-107">Depending on the resource (**event**, **message**, **outlookTask**, or **post**) that the attachment is attached to and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="2fd4e-108">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fd4e-108">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2fd4e-109">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="2fd4e-109">Supported resource</span></span> | <span data-ttu-id="2fd4e-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2fd4e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2fd4e-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2fd4e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fd4e-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2fd4e-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="2fd4e-113">evento</span><span class="sxs-lookup"><span data-stu-id="2fd4e-113">event</span></span>](../resources/event.md) | <span data-ttu-id="2fd4e-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2fd4e-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="2fd4e-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2fd4e-115">Calendars.ReadWrite</span></span> | <span data-ttu-id="2fd4e-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2fd4e-116">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="2fd4e-117">mensagem</span><span class="sxs-lookup"><span data-stu-id="2fd4e-117">message</span></span>](../resources/message.md) | <span data-ttu-id="2fd4e-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2fd4e-118">Mail.ReadWrite</span></span> | <span data-ttu-id="2fd4e-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2fd4e-119">Mail.ReadWrite</span></span> | <span data-ttu-id="2fd4e-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2fd4e-120">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="2fd4e-121">postagem</span><span class="sxs-lookup"><span data-stu-id="2fd4e-121">post</span></span>](../resources/post.md) | <span data-ttu-id="2fd4e-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fd4e-122">Group.ReadWrite.All</span></span> | <span data-ttu-id="2fd4e-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2fd4e-123">Not supported</span></span> | <span data-ttu-id="2fd4e-124">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2fd4e-124">Not supported</span></span> |


<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All.
-->

## <a name="http-request"></a><span data-ttu-id="2fd4e-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2fd4e-125">HTTP request</span></span>
<span data-ttu-id="2fd4e-126">Anexos de um [event](../resources/event.md) no [calendar](../resources/calendar.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="2fd4e-126">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}

DELETE /me/calendar/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}/attachments/{id}
```

<span data-ttu-id="2fd4e-127">Anexos de [um evento](../resources/event.md) no calendário [especificado](../resources/calendar.md) pertencente ao usuário.</span><span class="sxs-lookup"><span data-stu-id="2fd4e-127">Attachments for an [event](../resources/event.md) in the specified [calendar](../resources/calendar.md) belonging to the user.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}
```

<!-- Tried adding and getting group event with attachment, event exists but without attachment. Assume group event attachment not supported.
DELETE /groups/{id}/events/{id}/attachments/{id}
DELETE /groups/{id}/calendar/events/{id}/attachments/{id}
-->

<span data-ttu-id="2fd4e-128">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence ao [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="2fd4e-128">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="2fd4e-129">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence a um [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="2fd4e-129">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="2fd4e-130">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="2fd4e-130">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="2fd4e-131">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="2fd4e-131">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="2fd4e-p102">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante. </span><span class="sxs-lookup"><span data-stu-id="2fd4e-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. </span></span><!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="2fd4e-134">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="2fd4e-134">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2fd4e-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2fd4e-135">Request headers</span></span>
| <span data-ttu-id="2fd4e-136">Nome</span><span class="sxs-lookup"><span data-stu-id="2fd4e-136">Name</span></span>       | <span data-ttu-id="2fd4e-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fd4e-137">Type</span></span> | <span data-ttu-id="2fd4e-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fd4e-138">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2fd4e-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="2fd4e-139">Authorization</span></span>  | <span data-ttu-id="2fd4e-140">string</span><span class="sxs-lookup"><span data-stu-id="2fd4e-140">string</span></span>  | <span data-ttu-id="2fd4e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2fd4e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2fd4e-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2fd4e-143">Request body</span></span>
<span data-ttu-id="2fd4e-144">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2fd4e-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2fd4e-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fd4e-145">Response</span></span>

<span data-ttu-id="2fd4e-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2fd4e-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fd4e-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2fd4e-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2fd4e-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2fd4e-149">Request</span></span>
<span data-ttu-id="2fd4e-150">Veja um exemplo da solicitação para excluir um anexo em um evento.</span><span class="sxs-lookup"><span data-stu-id="2fd4e-150">Here is an example of the request to delete an attachment on an event.</span></span>

# <a name="http"></a>[<span data-ttu-id="2fd4e-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="2fd4e-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
# <a name="c"></a>[<span data-ttu-id="2fd4e-152">C#</span><span class="sxs-lookup"><span data-stu-id="2fd4e-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2fd4e-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2fd4e-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2fd4e-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2fd4e-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2fd4e-155">Java</span><span class="sxs-lookup"><span data-stu-id="2fd4e-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2fd4e-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fd4e-156">Response</span></span>
<span data-ttu-id="2fd4e-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2fd4e-157">Here is an example of the response.</span></span>
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

