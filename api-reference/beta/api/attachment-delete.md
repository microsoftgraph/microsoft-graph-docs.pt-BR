---
title: Excluir anexo
description: Exclua um anexo de um evento de calendário, mensagem, tarefa do Outlook ou postagem.
localization_priority: Normal
ms.openlocfilehash: 5bb24fc97a2f99dbb0fbec77e2de941f770c27fc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510894"
---
# <a name="delete-attachment"></a><span data-ttu-id="26b1c-103">Excluir anexo</span><span class="sxs-lookup"><span data-stu-id="26b1c-103">Delete attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26b1c-104">Exclua um anexo de um [evento](../resources/event.md)do calendário, [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postar](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="26b1c-104">Delete an attachment from a calendar [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="26b1c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="26b1c-105">Permissions</span></span>

<span data-ttu-id="26b1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26b1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="26b1c-108">Se estiver acessando anexos em Mensagens: Mail.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="26b1c-108">If accessing attachments in messages: Mail.ReadWrite</span></span>
* <span data-ttu-id="26b1c-109">Se estiver acessando anexos em Eventos: Calendars.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="26b1c-109">If accessing attachments in events: Calendars.ReadWrite</span></span>
* <span data-ttu-id="26b1c-110">Se acessando anexos em tarefas do Outlook: Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26b1c-110">If accessing attachments in Outlook tasks: Tasks.ReadWrite</span></span>
* <span data-ttu-id="26b1c-111">Se acessando anexos em postagens de grupo: Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26b1c-111">If accessing attachments in group posts: Group.ReadWrite.All</span></span>

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All
-->

## <a name="http-request"></a><span data-ttu-id="26b1c-112">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26b1c-112">HTTP request</span></span>

<span data-ttu-id="26b1c-113">Anexos para um [evento](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="26b1c-113">Attachments for an [event](../resources/event.md).</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}
```

<!--
DELETE /groups/{id}/events/{id}/attachments/{id}
-->

<span data-ttu-id="26b1c-114">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="26b1c-114">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```

<span data-ttu-id="26b1c-115">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="26b1c-115">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="26b1c-p102">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="26b1c-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. <!-- { "blockType": "ignored" } --></span></span>

```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="26b1c-118">Anexos para uma [tarefa do Outlook](../resources/outlooktask.md).</span><span class="sxs-lookup"><span data-stu-id="26b1c-118">Attachments for an [Outlook task](../resources/outlooktask.md).</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/<id>/attachments/{id}
DELETE /users/<id>/outlook/tasks/<id>/attachments/{id}
```

<span data-ttu-id="26b1c-119">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="26b1c-119">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="26b1c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26b1c-120">Request headers</span></span>

| <span data-ttu-id="26b1c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="26b1c-121">Name</span></span>       | <span data-ttu-id="26b1c-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="26b1c-122">Type</span></span> | <span data-ttu-id="26b1c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="26b1c-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="26b1c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="26b1c-124">Authorization</span></span>  | <span data-ttu-id="26b1c-125">string</span><span class="sxs-lookup"><span data-stu-id="26b1c-125">string</span></span>  | <span data-ttu-id="26b1c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26b1c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26b1c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26b1c-128">Request body</span></span>

<span data-ttu-id="26b1c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="26b1c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26b1c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="26b1c-130">Response</span></span>

<span data-ttu-id="26b1c-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26b1c-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26b1c-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26b1c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="26b1c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26b1c-134">Request</span></span>

<span data-ttu-id="26b1c-135">Veja um exemplo da solicitação para excluir um anexo em um evento.</span><span class="sxs-lookup"><span data-stu-id="26b1c-135">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```

### <a name="response"></a><span data-ttu-id="26b1c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="26b1c-136">Response</span></span>

<span data-ttu-id="26b1c-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26b1c-137">Here is an example of the response.</span></span>
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
    "Error: /api-reference/beta/api/attachment-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
