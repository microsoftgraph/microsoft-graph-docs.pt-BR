---
title: Excluir anexo
description: Exclua um anexo de um evento de calendário, mensagem, tarefa do Outlook ou postagem.
localization_priority: Normal
ms.openlocfilehash: c8af55d2237dd481e89b888d9bc025e6a1093695
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824938"
---
# <a name="delete-attachment"></a><span data-ttu-id="c4f20-103">Excluir anexo</span><span class="sxs-lookup"><span data-stu-id="c4f20-103">Delete attachment</span></span>

> <span data-ttu-id="c4f20-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c4f20-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4f20-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c4f20-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c4f20-106">Exclua um anexo de um [evento](../resources/event.md)do calendário, [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postar](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="c4f20-106">Delete an attachment from a calendar [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c4f20-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="c4f20-107">Permissions</span></span>

<span data-ttu-id="c4f20-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4f20-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="c4f20-110">Se acessando anexos em mensagens: Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4f20-110">If accessing attachments in messages: Mail.ReadWrite</span></span>
* <span data-ttu-id="c4f20-111">Se acessando anexos em eventos: Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4f20-111">If accessing attachments in events: Calendars.ReadWrite</span></span>
* <span data-ttu-id="c4f20-112">Se acessando anexos em tarefas do Outlook: Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4f20-112">If accessing attachments in Outlook tasks: Tasks.ReadWrite</span></span>
* <span data-ttu-id="c4f20-113">Se acessando anexos em postagens de grupo: Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4f20-113">If accessing attachments in group posts: Group.ReadWrite.All</span></span>

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All
-->

## <a name="http-request"></a><span data-ttu-id="c4f20-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4f20-114">HTTP request</span></span>

<span data-ttu-id="c4f20-115">Anexos para um [evento](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="c4f20-115">Attachments for an [event](../resources/event.md).</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}
```

<!--
DELETE /groups/{id}/events/{id}/attachments/{id}
-->

<span data-ttu-id="c4f20-116">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="c4f20-116">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```

<span data-ttu-id="c4f20-117">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="c4f20-117">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="c4f20-118">Anexos de uma [mensagem](../resources/message.md) contidos em uma pasta filho de um [mailFolder](../resources/mailfolder.md) na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="c4f20-118">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>  <span data-ttu-id="c4f20-119">O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada no filho de um filho e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="c4f20-119">The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="c4f20-120">Anexos para uma [tarefa do Outlook](../resources/outlooktask.md).</span><span class="sxs-lookup"><span data-stu-id="c4f20-120">Attachments for an [Outlook task](../resources/outlooktask.md).</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/<id>/attachments/{id}
DELETE /users/<id>/outlook/tasks/<id>/attachments/{id}
```

<span data-ttu-id="c4f20-121">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="c4f20-121">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c4f20-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4f20-122">Request headers</span></span>

| <span data-ttu-id="c4f20-123">Nome</span><span class="sxs-lookup"><span data-stu-id="c4f20-123">Name</span></span>       | <span data-ttu-id="c4f20-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4f20-124">Type</span></span> | <span data-ttu-id="c4f20-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4f20-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c4f20-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4f20-126">Authorization</span></span>  | <span data-ttu-id="c4f20-127">string</span><span class="sxs-lookup"><span data-stu-id="c4f20-127">string</span></span>  | <span data-ttu-id="c4f20-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4f20-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4f20-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4f20-130">Request body</span></span>

<span data-ttu-id="c4f20-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c4f20-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4f20-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4f20-132">Response</span></span>

<span data-ttu-id="c4f20-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4f20-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4f20-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4f20-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4f20-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4f20-136">Request</span></span>

<span data-ttu-id="c4f20-137">Veja um exemplo da solicitação para excluir um anexo em um evento.</span><span class="sxs-lookup"><span data-stu-id="c4f20-137">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```

### <a name="response"></a><span data-ttu-id="c4f20-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4f20-138">Response</span></span>

<span data-ttu-id="c4f20-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4f20-139">Here is an example of the response.</span></span>
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
