---
title: Obter anexo
description: Leia as propriedades e os relacionamentos de um anexo, anexados a um evento, mensagem, tarefa do Outlook ou postagem.
localization_priority: Normal
doc_type: apiPageType
author: abheek-das
ms.prod: outlook
ms.openlocfilehash: abe9ef81f8b00fdbac85cc9ff44cde1fffb4c10e
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176938"
---
# <a name="get-attachment"></a><span data-ttu-id="976d9-103">Obter anexo</span><span class="sxs-lookup"><span data-stu-id="976d9-103">Get attachment</span></span>

<span data-ttu-id="976d9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="976d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="976d9-105">Leia as propriedades, relações ou conteúdo bruto de um anexo anexado a um evento de usuário [,](../resources/event.md)mensagem [,](../resources/message.md)tarefa do [Outlook](../resources/outlooktask.md)ou postagem de [grupo.](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="976d9-105">Read the properties, relationships, or raw contents of an attachment that is attached to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or group [post](../resources/post.md).</span></span> 

<span data-ttu-id="976d9-106">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="976d9-106">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="976d9-107">Um arquivo.</span><span class="sxs-lookup"><span data-stu-id="976d9-107">A file.</span></span> <span data-ttu-id="976d9-108">Programaticamente, este é um recurso [fileAttachment](../resources/fileattachment.md).</span><span class="sxs-lookup"><span data-stu-id="976d9-108">Programmatically, this is a [fileAttachment](../resources/fileattachment.md) resource.</span></span> <span data-ttu-id="976d9-109">Veja [o exemplo 1](#example-1-get-the-properties-of-a-file-attachment).</span><span class="sxs-lookup"><span data-stu-id="976d9-109">See [example 1](#example-1-get-the-properties-of-a-file-attachment).</span></span>
* <span data-ttu-id="976d9-110">Um item do Outlook (contato, evento ou mensagem).</span><span class="sxs-lookup"><span data-stu-id="976d9-110">An Outlook item (contact, event or message).</span></span> <span data-ttu-id="976d9-111">Programaticamente, um anexo de item é um recurso [itemAttachment](../resources/itemattachment.md).</span><span class="sxs-lookup"><span data-stu-id="976d9-111">Programmatically, an item attachment is an [itemAttachment](../resources/itemattachment.md) resource.</span></span> <span data-ttu-id="976d9-112">Você pode usar `$expand` para obter ainda mais as propriedades desse item, incluindo todos os anexos aninhados até 30 níveis.</span><span class="sxs-lookup"><span data-stu-id="976d9-112">You can use `$expand` to further get the properties of that item, including any nested attachments up to 30 levels.</span></span> <span data-ttu-id="976d9-113">Veja [o exemplo 3](#example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message) e [o exemplo 4.](#example-4-expand-and-get-the-properties-of-an-item-attached-to-a-message-including-any-attachment-to-the-item)</span><span class="sxs-lookup"><span data-stu-id="976d9-113">See [example 3](#example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message) and [example 4](#example-4-expand-and-get-the-properties-of-an-item-attached-to-a-message-including-any-attachment-to-the-item).</span></span>
* <span data-ttu-id="976d9-114">Um link para um arquivo armazenado na nuvem.</span><span class="sxs-lookup"><span data-stu-id="976d9-114">A link to a file stored in the cloud.</span></span> <span data-ttu-id="976d9-115">Programaticamente, este é um recurso [referenceAttachment](../resources/referenceattachment.md).</span><span class="sxs-lookup"><span data-stu-id="976d9-115">Programmatically, this is a [referenceAttachment](../resources/referenceattachment.md) resource.</span></span> <span data-ttu-id="976d9-116">Veja [o exemplo 5](#example-5-get-the-properties-of-a-reference-attachment).</span><span class="sxs-lookup"><span data-stu-id="976d9-116">See [example 5](#example-5-get-the-properties-of-a-reference-attachment).</span></span>

<span data-ttu-id="976d9-117">Todos esses tipos de anexos são derivados do recurso [anexo](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="976d9-117">All these types of attachments are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

### <a name="get-the-raw-contents-of-a-file-or-item-attachment"></a><span data-ttu-id="976d9-118">Obter o conteúdo bruto de um arquivo ou anexo de item</span><span class="sxs-lookup"><span data-stu-id="976d9-118">Get the raw contents of a file or item attachment</span></span>
<span data-ttu-id="976d9-119">Você pode anexar o segmento do caminho `/$value` para obter o conteúdo bruto de um arquivo ou anexo de item.</span><span class="sxs-lookup"><span data-stu-id="976d9-119">You can append the path segment `/$value` to get the raw contents of a file or item attachment.</span></span> 

<span data-ttu-id="976d9-120">Para um anexo de arquivo, o tipo de conteúdo é baseado no tipo de conteúdo original.</span><span class="sxs-lookup"><span data-stu-id="976d9-120">For a file attachment, the content type is based on its original content type.</span></span> <span data-ttu-id="976d9-121">Veja um [exemplo 6](#example-6-get-the-raw-contents-of-a-file-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="976d9-121">See an [example 6](#example-6-get-the-raw-contents-of-a-file-attachment-on-a-message).</span></span>

<span data-ttu-id="976d9-122">Para um anexo de item que é um [contato](../resources/contact.md), [evento](../resources/event.md) ou [mensagem](../resources/message.md), o conteúdo bruto retornado está no formato MIME.</span><span class="sxs-lookup"><span data-stu-id="976d9-122">For an item attachment that is a [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md), the raw contents returned is in MIME format.</span></span>

| <span data-ttu-id="976d9-123">Tipo de anexo do item</span><span class="sxs-lookup"><span data-stu-id="976d9-123">Item attachment type</span></span>  | <span data-ttu-id="976d9-124">Conteúdo bruto retornado</span><span class="sxs-lookup"><span data-stu-id="976d9-124">Raw contents returned</span></span> |
|:-----------|:----------|
| <span data-ttu-id="976d9-125">**contato**</span><span class="sxs-lookup"><span data-stu-id="976d9-125">**contact**</span></span> | <span data-ttu-id="976d9-126">Formato [vCard](http://www.faqs.org/rfcs/rfc2426.html) MIME.</span><span class="sxs-lookup"><span data-stu-id="976d9-126">[vCard](http://www.faqs.org/rfcs/rfc2426.html) MIME format.</span></span> <span data-ttu-id="976d9-127">Veja [o exemplo 7](#example-7-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="976d9-127">See [example 7](#example-7-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message).</span></span> |
| <span data-ttu-id="976d9-128">**event**</span><span class="sxs-lookup"><span data-stu-id="976d9-128">**event**</span></span> | <span data-ttu-id="976d9-129">Formato iCal MIME.</span><span class="sxs-lookup"><span data-stu-id="976d9-129">iCal MIME format.</span></span> <span data-ttu-id="976d9-130">Veja [o exemplo 8](#example-8-get-the-mime-raw-contents-of-an-event-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="976d9-130">See [example 8](#example-8-get-the-mime-raw-contents-of-an-event-attachment-on-a-message).</span></span> |
| <span data-ttu-id="976d9-131">**message**</span><span class="sxs-lookup"><span data-stu-id="976d9-131">**message**</span></span> | <span data-ttu-id="976d9-132">Formato MIME.</span><span class="sxs-lookup"><span data-stu-id="976d9-132">MIME format.</span></span> <span data-ttu-id="976d9-133">Veja [o exemplo 9](#example-9-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="976d9-133">See [example 9](#example-9-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message).</span></span> |

<span data-ttu-id="976d9-134">A tentativa de obter o `$value` de um anexo de referência retorna HTTP 405.</span><span class="sxs-lookup"><span data-stu-id="976d9-134">Attempting to get the `$value` of a reference attachment returns HTTP 405.</span></span>

## <a name="permissions"></a><span data-ttu-id="976d9-135">Permissões</span><span class="sxs-lookup"><span data-stu-id="976d9-135">Permissions</span></span>

<span data-ttu-id="976d9-136">Dependendo do recurso (**evento** **,** mensagem , **outlookTask** ou **postagem**) ao qual o anexo está anexado e o tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é o menos privilegiado necessário para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="976d9-136">Depending on the resource (**event**, **message**, **outlookTask**, or **post**) that the attachment is attached to and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="976d9-137">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="976d9-137">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="976d9-138">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="976d9-138">Supported resource</span></span> | <span data-ttu-id="976d9-139">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="976d9-139">Delegated (work or school account)</span></span> | <span data-ttu-id="976d9-140">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="976d9-140">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="976d9-141">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="976d9-141">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="976d9-142">evento</span><span class="sxs-lookup"><span data-stu-id="976d9-142">event</span></span>](../resources/event.md) | <span data-ttu-id="976d9-143">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="976d9-143">Calendars.Read</span></span> | <span data-ttu-id="976d9-144">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="976d9-144">Calendars.Read</span></span> | <span data-ttu-id="976d9-145">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="976d9-145">Calendars.Read</span></span> |
| [<span data-ttu-id="976d9-146">message</span><span class="sxs-lookup"><span data-stu-id="976d9-146">message</span></span>](../resources/message.md) | <span data-ttu-id="976d9-147">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="976d9-147">Mail.Read</span></span> | <span data-ttu-id="976d9-148">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="976d9-148">Mail.Read</span></span> | <span data-ttu-id="976d9-149">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="976d9-149">Mail.Read</span></span> |
| [<span data-ttu-id="976d9-150">outlookTask</span><span class="sxs-lookup"><span data-stu-id="976d9-150">outlookTask</span></span>](../resources/outlooktask.md) |  <span data-ttu-id="976d9-151">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="976d9-151">Tasks.Read</span></span> | <span data-ttu-id="976d9-152">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="976d9-152">Tasks.Read</span></span> | <span data-ttu-id="976d9-153">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="976d9-153">Not supported</span></span> |
| [<span data-ttu-id="976d9-154">postagem</span><span class="sxs-lookup"><span data-stu-id="976d9-154">post</span></span>](../resources/post.md) | <span data-ttu-id="976d9-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="976d9-155">Group.Read.All</span></span> | <span data-ttu-id="976d9-156">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="976d9-156">Not supported</span></span> | <span data-ttu-id="976d9-157">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="976d9-157">Not supported</span></span> |


<!--
* If accessing attachments in group events or posts: Group.Read.All
-->

## <a name="http-request"></a><span data-ttu-id="976d9-158">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="976d9-158">HTTP request</span></span>

<span data-ttu-id="976d9-159">Esta seção mostra a sintaxe de solicitação HTTP GET para cada uma das entidades ([evento](../resources/event.md) [,](../resources/message.md)mensagem , tarefa do [Outlook](../resources/outlooktask.md)e [postagem](../resources/post.md)) que suportam anexos:</span><span class="sxs-lookup"><span data-stu-id="976d9-159">This section shows the HTTP GET request syntax for each of the entities ([event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), and [post](../resources/post.md)) that support attachments:</span></span>

- <span data-ttu-id="976d9-160">Para obter as propriedades e os relacionamentos de um anexo, especifique a ID do anexo a ser indexada na coleção **attachments,** anexada ao evento especificado [,](../resources/event.md)mensagem [,](../resources/message.md)tarefa do [Outlook](../resources/outlooktask.md)ou instância [de postagem.](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="976d9-160">To get the properties and relationships of an attachment, specify the attachment ID to index into the **attachments** collection, attached to the specified [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) instance.</span></span>
- <span data-ttu-id="976d9-161">Se o anexo for um arquivo ou item do Outlook (contato, evento ou mensagem), você poderá obter ainda mais o conteúdo bruto do anexo anexando o segmento de caminho `/$value` à URL da solicitação.</span><span class="sxs-lookup"><span data-stu-id="976d9-161">If the attachment is a file or Outlook item (contact, event, or message), you can further get the raw contents of the attachment by appending the path segment `/$value` to the request URL.</span></span>

<span data-ttu-id="976d9-162">Um anexo de um [evento:](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="976d9-162">An attachment of an [event](../resources/event.md):</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}
GET /me/events/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}/$value
```

<!--
GET /groups/{id}/events/{id}/attachments/{id}
-->

<span data-ttu-id="976d9-163">Um anexo de uma [mensagem na](../resources/message.md) caixa de correio de um usuário:</span><span class="sxs-lookup"><span data-stu-id="976d9-163">An attachment of a [message](../resources/message.md) in a user's mailbox:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
GET /me/messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}/$value
```

<span data-ttu-id="976d9-164">Um anexo de uma [mensagem contida](../resources/message.md) em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário:</span><span class="sxs-lookup"><span data-stu-id="976d9-164">An attachment of a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}/$value
```

<span data-ttu-id="976d9-165">Um anexo de uma [mensagem contida](../resources/message.md) em uma pasta filha de [uma mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário:</span><span class="sxs-lookup"><span data-stu-id="976d9-165">An attachment of a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}/$value
```

<span data-ttu-id="976d9-166">O exemplo anterior mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="976d9-166">The preceding example shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>

<span data-ttu-id="976d9-167">Um anexo de uma [tarefa do Outlook:](../resources/outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="976d9-167">An attachment of an [Outlook task](../resources/outlooktask.md):</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}/attachments/{id}
GET /users/{id}/outlook/tasks/{id}/attachments/{id}
GET /me/outlook/tasks/{id}/attachments/{id}/$value
GET /users/{id}/outlook/tasks/{id}/attachments/{id}/$value
```

<span data-ttu-id="976d9-168">Um anexo de [uma postagem](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a [uma conversa](../resources/conversation.md) de um grupo:</span><span class="sxs-lookup"><span data-stu-id="976d9-168">An attachment of a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
```

## <a name="optional-query-parameters"></a><span data-ttu-id="976d9-169">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="976d9-169">Optional query parameters</span></span>

<span data-ttu-id="976d9-170">Este método também dá suporte a alguns [Parâmetros de Consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="976d9-170">This method supports some of the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="976d9-171">Use `$expand` para obter as propriedades de um anexo de item (contato, evento ou mensagem).</span><span class="sxs-lookup"><span data-stu-id="976d9-171">Use `$expand` to get the properties of an item attachment (contact, event, or message).</span></span> <span data-ttu-id="976d9-172">Veja [o exemplo 3](#example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message) e [o exemplo 4.](#example-4-expand-and-get-the-properties-of-an-item-attached-to-a-message-including-any-attachment-to-the-item)</span><span class="sxs-lookup"><span data-stu-id="976d9-172">See [example 3](#example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message) and [example 4](#example-4-expand-and-get-the-properties-of-an-item-attached-to-a-message-including-any-attachment-to-the-item).</span></span>

## <a name="request-headers"></a><span data-ttu-id="976d9-173">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="976d9-173">Request headers</span></span>

| <span data-ttu-id="976d9-174">Nome</span><span class="sxs-lookup"><span data-stu-id="976d9-174">Name</span></span>       | <span data-ttu-id="976d9-175">Tipo</span><span class="sxs-lookup"><span data-stu-id="976d9-175">Type</span></span> | <span data-ttu-id="976d9-176">Descrição</span><span class="sxs-lookup"><span data-stu-id="976d9-176">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="976d9-177">Autorização</span><span class="sxs-lookup"><span data-stu-id="976d9-177">Authorization</span></span>  | <span data-ttu-id="976d9-178">string</span><span class="sxs-lookup"><span data-stu-id="976d9-178">string</span></span>  | <span data-ttu-id="976d9-p110">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="976d9-p110">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="976d9-181">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="976d9-181">Request body</span></span>

<span data-ttu-id="976d9-182">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="976d9-182">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="976d9-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="976d9-183">Response</span></span>

<span data-ttu-id="976d9-184">Se tiver êxito, o método GET retornará um `200 OK` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="976d9-184">If successful, the GET method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="976d9-185">Se você estiver obtendo as propriedades e os relacionamentos de um anexo, o corpo da resposta incluirá um objeto de [anexo](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="976d9-185">If you're getting the properties and relationships of an attachment, the response body includes an [attachment](../resources/attachment.md) object.</span></span>
<span data-ttu-id="976d9-186">As propriedades desse tipo de anexo são retornadas: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) ou [referenceAttachment](../resources/referenceattachment.md).</span><span class="sxs-lookup"><span data-stu-id="976d9-186">The properties of that type of attachment are returned: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md).</span></span>

<span data-ttu-id="976d9-187">Se você estiver obtendo o conteúdo bruto de um anexo de arquivo ou de item, o corpo da resposta incluirá o valor bruto do anexo.</span><span class="sxs-lookup"><span data-stu-id="976d9-187">If you're getting the raw contents of a file or item attachment, the response body includes the raw value of the attachment.</span></span>

## <a name="examples"></a><span data-ttu-id="976d9-188">Exemplos</span><span class="sxs-lookup"><span data-stu-id="976d9-188">Examples</span></span>

### <a name="example-1-get-the-properties-of-a-file-attachment"></a><span data-ttu-id="976d9-189">Exemplo 1: Obter as propriedades de um anexo de arquivo</span><span class="sxs-lookup"><span data-stu-id="976d9-189">Example 1: Get the properties of a file attachment</span></span>

#### <a name="request"></a><span data-ttu-id="976d9-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="976d9-190">Request</span></span>

<span data-ttu-id="976d9-191">Aqui está um exemplo da solicitação para obter as propriedades de um anexo de arquivo em uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="976d9-191">Here is an example of the request to get the properties of a file attachment on a message.</span></span>

# <a name="http"></a>[<span data-ttu-id="976d9-192">HTTP</span><span class="sxs-lookup"><span data-stu-id="976d9-192">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_file_attachment_beta",
  "sampleKeys": ["AAMkAGUzY5QKjAAA=","AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=
```
# <a name="c"></a>[<span data-ttu-id="976d9-193">C#</span><span class="sxs-lookup"><span data-stu-id="976d9-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-file-attachment-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="976d9-194">JavaScript</span><span class="sxs-lookup"><span data-stu-id="976d9-194">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-file-attachment-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="976d9-195">Objective-C</span><span class="sxs-lookup"><span data-stu-id="976d9-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-file-attachment-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="976d9-196">Java</span><span class="sxs-lookup"><span data-stu-id="976d9-196">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-file-attachment-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="976d9-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="976d9-197">Response</span></span>

<span data-ttu-id="976d9-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="976d9-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_file_attachment_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages('AAMkAGUzY5QKjAAA%3D')/attachments/$entity",
    "@odata.type": "#microsoft.graph.fileAttachment",
    "id": "AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=",
    "lastModifiedDateTime": "2019-04-02T03:41:29Z",
    "name": "Draft sales invoice template.docx",
    "contentType": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
    "size": 13068,
    "isInline": false,
    "contentId": null,
    "contentLocation": null,
    "contentBytes": "UEsDBBQABgAIAAAAIQ4AAAAA"
}
```

### <a name="example-2-get-the-properties-of-an-item-attachment"></a><span data-ttu-id="976d9-201">Exemplo 2: Obter as propriedades de um anexo de item</span><span class="sxs-lookup"><span data-stu-id="976d9-201">Example 2: Get the properties of an item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="976d9-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="976d9-202">Request</span></span>

<span data-ttu-id="976d9-203">O próximo exemplo mostra como obter um anexo de item em uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="976d9-203">The next example shows how to get an item attachment on a message.</span></span> <span data-ttu-id="976d9-204">As propriedades de **itemAttachment** são retornadas.</span><span class="sxs-lookup"><span data-stu-id="976d9-204">The properties of the **itemAttachment** are returned.</span></span>

# <a name="http"></a>[<span data-ttu-id="976d9-205">HTTP</span><span class="sxs-lookup"><span data-stu-id="976d9-205">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_item_attachment",
  "sampleKeys": ["AAMkADA1M-zAAA=","AAMkADA1M-CJKtzmnlcqVgqI="]
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')
```
# <a name="c"></a>[<span data-ttu-id="976d9-206">C#</span><span class="sxs-lookup"><span data-stu-id="976d9-206">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="976d9-207">JavaScript</span><span class="sxs-lookup"><span data-stu-id="976d9-207">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="976d9-208">Objective-C</span><span class="sxs-lookup"><span data-stu-id="976d9-208">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="976d9-209">Java</span><span class="sxs-lookup"><span data-stu-id="976d9-209">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="976d9-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="976d9-210">Response</span></span>
<span data-ttu-id="976d9-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="976d9-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_item_attachment",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1M-CJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false
}
```

### <a name="example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message"></a><span data-ttu-id="976d9-214">Exemplo 3: Expandir e obter as propriedades do item anexado a uma mensagem</span><span class="sxs-lookup"><span data-stu-id="976d9-214">Example 3: Expand and get the properties of the item attached to a message</span></span>
#### <a name="request"></a><span data-ttu-id="976d9-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="976d9-215">Request</span></span>

<span data-ttu-id="976d9-216">O próximo exemplo mostra como usar `$expand` para obter as propriedades do item (contato, evento ou mensagem) anexado à mensagem.</span><span class="sxs-lookup"><span data-stu-id="976d9-216">The next example shows how to use `$expand` to get the properties of the item (contact, event, or message) that is attached to the message.</span></span> <span data-ttu-id="976d9-217">Neste exemplo, esse item é uma mensagem. As propriedades dessa mensagem anexadas também são retornadas.</span><span class="sxs-lookup"><span data-stu-id="976d9-217">In this example, that item is a message; the properties of that attached message are also returned.</span></span>

# <a name="http"></a>[<span data-ttu-id="976d9-218">HTTP</span><span class="sxs-lookup"><span data-stu-id="976d9-218">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_and_expand_item_attachment",
  "sampleKeys": ["AAMkADA1M-zAAA=","AAMkADA1M-CJKtzmnlcqVgqI="]
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')/?$expand=microsoft.graph.itemattachment/item
```
# <a name="c"></a>[<span data-ttu-id="976d9-219">C#</span><span class="sxs-lookup"><span data-stu-id="976d9-219">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-and-expand-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="976d9-220">JavaScript</span><span class="sxs-lookup"><span data-stu-id="976d9-220">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-and-expand-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="976d9-221">Objective-C</span><span class="sxs-lookup"><span data-stu-id="976d9-221">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-and-expand-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="976d9-222">Java</span><span class="sxs-lookup"><span data-stu-id="976d9-222">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-and-expand-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="976d9-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="976d9-223">Response</span></span>
<span data-ttu-id="976d9-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="976d9-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_and_expand_item_attachment",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false,
  "item@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments('AAMkADA1M-CJKtzmnlcqVgqI%3D')/microsoft.graph.itemAttachment/item/$entity",
  "item":{
    "@odata.type":"#microsoft.graph.message",
    "id":"",
    "createdDateTime":"2017-07-21T00:20:41Z",
    "lastModifiedDateTime":"2017-07-21T00:20:34Z",
    "receivedDateTime":"2017-07-21T00:19:55Z",
    "sentDateTime":"2017-07-21T00:19:52Z",
    "hasAttachments":false,
    "internetMessageId":"<BY2PR15MB05189A084C01F466709E414F9CA40@BY2PR15MB0518.namprd15.prod.outlook.com>",
    "subject":"Reminder - please bring laptop",
    "bodyPreview": "PFA\r\n\r\nThanks,\r\nRob",
    "importance":"normal",
    "conversationId":"AAQkADA1MzMyOGI4LTlkZDctNDkzYy05M2RiLTdiN2E1NDE3MTRkOQAQAMG_NSCMBqdKrLa2EmR-lO0=",
    "conversationIndex":"AQHTAbcSwb41IIwGp0qstrYSZH+U7Q==",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADA1M3MTRkOQAAAA%3D%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "internetMessageHeaders": [ ],
    "body":{
      "contentType":"html",
      "content":"<html><head>\r\n</head>\r\n<body>\r\n</body>\r\n</html>"
    },
    "sender":{
      "emailAddress":{
        "name":"Adele Vance",
        "address":"AdeleV@contoso.onmicrosoft.com"
      }
    },
    "from":{
      "emailAddress":{
        "name":"Adele Vance",
        "address":"AdeleV@contoso.onmicrosoft.com"
      }
    },
    "toRecipients":[
      {
        "emailAddress":{
          "name":"Alex Wilbur",
          "address":"AlexW@contoso.onmicrosoft.com"
        }
      }
    ],
    "ccRecipients":[
      {
        "emailAddress":{
          "name":"Adele Vance",
          "address":"AdeleV@contoso.onmicrosoft.com"
        }
      }
    ],
    "flag":{
      "flagStatus":"notFlagged"
    }
  }
}
```

### <a name="example-4-expand-and-get-the-properties-of-an-item-attached-to-a-message-including-any-attachment-to-the-item"></a><span data-ttu-id="976d9-227">Exemplo 4: Expandir e obter as propriedades de um item anexado a uma mensagem, incluindo qualquer anexo ao item</span><span class="sxs-lookup"><span data-stu-id="976d9-227">Example 4: Expand and get the properties of an item attached to a message, including any attachment to the item</span></span>
#### <a name="request"></a><span data-ttu-id="976d9-228">Solicitação</span><span class="sxs-lookup"><span data-stu-id="976d9-228">Request</span></span>
<span data-ttu-id="976d9-229">O próximo exemplo usa a mesma solicitação que no [exemplo 3](#example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message) para obter as propriedades de um anexo de item em uma mensagem usando `$expand` .</span><span class="sxs-lookup"><span data-stu-id="976d9-229">The next example uses the same request as in [example 3](#example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message) to get the properties of an item attachment on a message by using `$expand`.</span></span> <span data-ttu-id="976d9-230">Nesse caso, como o item anexado também tem um anexo de arquivo, a resposta também inclui as propriedades do anexo de arquivo.</span><span class="sxs-lookup"><span data-stu-id="976d9-230">In this case, because the attached item also has a file attachment, the response includes the properties of the file attachment as well.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_and_expand_nested_item_attachment",
  "sampleKeys": ["AAMkADA1M-zAAA=","AAMkADA1M-CJKtzmnlcqVgqI="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')/?$expand=microsoft.graph.itemattachment/item
```

#### <a name="response"></a><span data-ttu-id="976d9-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="976d9-231">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "get_and_expand_nested_item_attachment",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments(microsoft.graph.itemAttachment/item())/$entity",
    "@odata.type": "#microsoft.graph.itemAttachment",
    "id": "AAMkADA1MCJKtzmnlcqVgqI=",
    "lastModifiedDateTime": "2021-01-06T13:28:11Z",
    "name": "Nested Message With Attachment",
    "contentType": null,
    "size": 465916,
    "isInline": false,
    "item@odata.context": "https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments('AAMkADA1M-CJKtzmnlcqVgqI%3D')/microsoft.graph.itemAttachment/item/$entity",
    "item": {
        "@odata.type": "#microsoft.graph.message",
        "id": "",
        "createdDateTime": "2021-01-06T13:28:30Z",
        "lastModifiedDateTime": "2021-01-06T13:27:40Z",
        "receivedDateTime": "2021-01-06T13:27:25Z",
        "sentDateTime": "2021-01-06T13:27:04Z",
        "hasAttachments": true,
        "internetMessageId": "<BY2PR15MB05189A084C01F466709E414F9CA40@BY2PR15MB0518.namprd15.prod.outlook.com>",
        "subject": "Nested Message With Attachment",
        "bodyPreview": "PFAThanks,Adele",
        "importance": "normal",
        "conversationId": "AAQkADg3NTY5MDg4LWMzYmQtNDQzNi05OTgwLWQyZjg2YWQwMTNkZAAQAO6hkp84oMdGm6ZBsSH72sE=",
        "conversationIndex": "AQHW5C+U7qGSnzigx0abpkGxIfvawQ==",
        "isDeliveryReceiptRequested": false,
        "isReadReceiptRequested": false,
        "isRead": true,
        "isDraft": false,
        "webLink": "https://outlook.office365.com/owa/?ItemID=AAMkADA1M3MTRkOQAAAA%3D%3D&exvsurl=1&viewmodel=ItemAttachment",
        "internetMessageHeaders": [],
        "body": {
            "contentType": "html",
            "content": "<html><head>\r\n</head>\r\n<body>\r\n</body>\r\n</html>"
        },
        "sender": {
            "emailAddress": {
                "name": "Adele Vance",
                "address": "Adele.Vance@microsoft.com"
            }
        },
        "from": {
            "emailAddress": {
                "name": "Adele Vance",
                "address": "Adele.Vance@microsoft.com"
            }
        },
        "toRecipients": [
            {
                "emailAddress": {
                    "name": "Adele Vance",
                    "address": "Adele.Vance@microsoft.com"
                }
            }
        ],
        "flag": {
            "flagStatus": "notFlagged"
        },
        "attachments@odata.context": "https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments('AAMkADA1M-CJKtzmnlcqVgqI%3D')/microsoft.graph.itemAttachment/microsoft.graph.itemAttachment/item/microsoft.graph.message/microsoft.graph.message/microsoft.graph.message/microsoft.graph.message/microsoft.graph.message/microsoft.graph.message/microsoft.graph.message/attachments",
        "attachments": [
            {
                "@odata.type": "#microsoft.graph.fileAttachment",
                "@odata.mediaContentType": "application/pdf",
                "id": "AAMkADg3NTYULmbsDYNg==",
                "lastModifiedDateTime": "2021-01-21T14:56:18Z",
                "name": "Info.pdf",
                "contentType": "application/pdf",
                "size": 417351,
                "isInline": false,
                "contentId": null,
                "contentLocation": null,
                "contentBytes": "JVBERi0xLjUNCiW1tbW1DQoxIDAgb2JqDQo8PC9UeXBlL0NhdGFsb2cvUGFnZXMgMiAwIFIvTGFuZyhlbi1JTikgL1N0cnVjdFRyZWVSb29"
            }
        ]
    }
}
```

### <a name="example-5-get-the-properties-of-a-reference-attachment"></a><span data-ttu-id="976d9-232">Exemplo 5: Obter as propriedades de um anexo de referência</span><span class="sxs-lookup"><span data-stu-id="976d9-232">Example 5: Get the properties of a reference attachment</span></span>

#### <a name="request"></a><span data-ttu-id="976d9-233">Solicitação</span><span class="sxs-lookup"><span data-stu-id="976d9-233">Request</span></span>

<span data-ttu-id="976d9-234">Aqui está um exemplo da solicitação para obter um anexo de referência em um evento.</span><span class="sxs-lookup"><span data-stu-id="976d9-234">Here is an example of the request to get a reference attachment on an event.</span></span>

# <a name="http"></a>[<span data-ttu-id="976d9-235">HTTP</span><span class="sxs-lookup"><span data-stu-id="976d9-235">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment",
  "sampleKeys": ["AAMkAGE1M88AADUv0uAAAG=","AAMkAGE1Mg72tgf7hJp0PICVGCc0g="]
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkAGE1M88AADUv0uAAAG=/attachments/AAMkAGE1Mg72tgf7hJp0PICVGCc0g=
```
# <a name="c"></a>[<span data-ttu-id="976d9-236">C#</span><span class="sxs-lookup"><span data-stu-id="976d9-236">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reference-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="976d9-237">JavaScript</span><span class="sxs-lookup"><span data-stu-id="976d9-237">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reference-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="976d9-238">Objective-C</span><span class="sxs-lookup"><span data-stu-id="976d9-238">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reference-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="976d9-239">Java</span><span class="sxs-lookup"><span data-stu-id="976d9-239">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-reference-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="976d9-240">Resposta</span><span class="sxs-lookup"><span data-stu-id="976d9-240">Response</span></span>
<span data-ttu-id="976d9-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="976d9-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_reference_attachment",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/ddfcd489-628b-40d7-b48b-57002df800e5/events/AAMkAGE1M88AADUv0uAAAG%3D/attachments/$entity",
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "id": "AAMkAGE1Mg72tgf7hJp0PCGVCIc0g=",
  "lastModifiedDateTime": "2016-03-12T06:04:38Z",
  "name": "Personal pictures",
  "contentType": null,
  "size": 382,
  "isInline": false,
  "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
  "providerType": "oneDriveConsumer",
  "thumbnailUrl": null,
  "previewUrl": null,
  "permission": "edit",
  "isFolder": true
}
```


### <a name="example-6-get-the-raw-contents-of-a-file-attachment-on-a-message"></a><span data-ttu-id="976d9-244">Exemplo 6: Obter o conteúdo bruto de um anexo de arquivo em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="976d9-244">Example 6: Get the raw contents of a file attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="976d9-245">Solicitação</span><span class="sxs-lookup"><span data-stu-id="976d9-245">Request</span></span>

<span data-ttu-id="976d9-246">Aqui está um exemplo da solicitação para obter o conteúdo bruto de um arquivo do Word que foi anexado a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="976d9-246">Here is an example of the request to get the raw contents of a Word file that has been attached to a message.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_value_file_attachment",
  "sampleKeys": ["AAMkAGUzY5QKjAAA=","AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=/$value
```

#### <a name="response"></a><span data-ttu-id="976d9-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="976d9-247">Response</span></span>
<span data-ttu-id="976d9-248">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="976d9-248">Here is an example of the response.</span></span> <span data-ttu-id="976d9-249">O corpo da resposta real inclui os bytes brutos do anexo do arquivo, que são abreviados aqui por questões de brevidade.</span><span class="sxs-lookup"><span data-stu-id="976d9-249">The actual response body includes the raw bytes of the file attachment, which are abbreviated here for brevity.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_value_file_attachment",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK

{Raw bytes of the file}
```


### <a name="example-7-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message"></a><span data-ttu-id="976d9-250">Exemplo 7: Obter o conteúdo bruto MIME de um anexo de contato em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="976d9-250">Example 7: Get the MIME raw contents of a contact attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="976d9-251">Solicitação</span><span class="sxs-lookup"><span data-stu-id="976d9-251">Request</span></span>

<span data-ttu-id="976d9-252">Aqui está um exemplo da solicitação para obter o conteúdo bruto de um item de contato que foi anexado a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="976d9-252">Here is an example of the request to get the raw contents of a contact item that has been attached to a message.</span></span> 
<!-- {
  "blockType": "ignored",
  "name": "get_value_contact_attachment",
  "sampleKeys": ["AAMkADI5MAAGjk2PxAAA=","AAMkADI5MAAGjk2PxAAABEgAQACEJqrbJZBNIlr3pGFvd9K8="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkADI5MAAGjk2PxAAA=/attachments/AAMkADI5MAAGjk2PxAAABEgAQACEJqrbJZBNIlr3pGFvd9K8=/$value
```

#### <a name="response"></a><span data-ttu-id="976d9-253">Resposta</span><span class="sxs-lookup"><span data-stu-id="976d9-253">Response</span></span>
<span data-ttu-id="976d9-254">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="976d9-254">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "ignored",
  "name": "get_value_contact_attachment",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK

BEGIN:VCARD
PROFILE:VCARD
VERSION:3.0
MAILER:Microsoft Exchange
PRODID:Microsoft Exchange
FN:Alex Wilbur
N:Wilbur;Alex;;;
NOTE:Sunday\, June 10\, 2012 5:44 PM:\nGutter\, window cleaning\, pressure 
 washing\, roof debris blowing\n
ORG:Contoso;
CLASS:PUBLIC
ADR;TYPE=WORK,PREF:;;4567 Main St;Buffalo;NY;98052;United States of America
LABEL;TYPE=WORK,PREF:4567 Main St\nBuffalo\, NY 98052
ADR;TYPE=HOME:;;;;;;
ADR;TYPE=POSTAL:;;;;;;
TEL;TYPE=WORK:(425) 555-0100
TITLE:
X-MS-IMADDRESS:
REV;VALUE=DATE-TIME:2019-04-09T02:13:31,161Z
END:VCARD
```


### <a name="example-8-get-the-mime-raw-contents-of-an-event-attachment-on-a-message"></a><span data-ttu-id="976d9-255">Exemplo 8: Obter o conteúdo bruto MIME de um anexo de evento em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="976d9-255">Example 8: Get the MIME raw contents of an event attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="976d9-256">Solicitação</span><span class="sxs-lookup"><span data-stu-id="976d9-256">Request</span></span>

<span data-ttu-id="976d9-257">Aqui está um exemplo da solicitação para obter o conteúdo bruto de um evento que foi anexado a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="976d9-257">Here is an example of the request to get the raw contents of an event that has been attached to a message.</span></span> 
<!-- {
  "blockType": "ignored",
  "name": "get_value_event_attachment",
  "sampleKeys": ["AAMkADVIOAAA=","AAMkADVIOAAABEgAQACvkutl6c4FMifPyS6NvXsM="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkADVIOAAA=/attachments/AAMkADVIOAAABEgAQACvkutl6c4FMifPyS6NvXsM=/$value
```

#### <a name="response"></a><span data-ttu-id="976d9-258">Resposta</span><span class="sxs-lookup"><span data-stu-id="976d9-258">Response</span></span>
<span data-ttu-id="976d9-259">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="976d9-259">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "ignored",
  "name": "get_value_event_attachment",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK

BEGIN:VCALENDAR
METHOD:PUBLISH
PRODID:Microsoft Exchange Server 2010
VERSION:2.0
BEGIN:VTIMEZONE
TZID:Pacific Standard Time
BEGIN:STANDARD
DTSTART:16010101T020000
TZOFFSETFROM:-0700
TZOFFSETTO:-0800
RRULE:FREQ=YEARLY;INTERVAL=1;BYDAY=1SU;BYMONTH=11
END:STANDARD
BEGIN:DAYLIGHT
DTSTART:16010101T020000
TZOFFSETFROM:-0800
TZOFFSETTO:-0700
RRULE:FREQ=YEARLY;INTERVAL=1;BYDAY=2SU;BYMONTH=3
END:DAYLIGHT
END:VTIMEZONE
BEGIN:VEVENT
ORGANIZER;CN=Adele Vance:MAILTO:adelev@contoso.com
ATTENDEE;ROLE=REQ-PARTICIPANT;PARTSTAT=NEEDS-ACTION;RSVP=TRUE;CN=Adele Vance:MAILTO:adelev@contoso.com
DESCRIPTION;LANGUAGE=en-US:\n
UID:040000008200
SUMMARY;LANGUAGE=en-US:Review Megan's docs
DTSTART;TZID=Pacific Standard Time:20190409T140000
DTEND;TZID=Pacific Standard Time:20190409T160000
CLASS:PUBLIC
PRIORITY:5
DTSTAMP:20190409T211833Z
TRANSP:OPAQUE
STATUS:CONFIRMED
SEQUENCE:0
LOCATION;LANGUAGE=en-US:
X-MICROSOFT-CDO-APPT-SEQUENCE:0
X-MICROSOFT-CDO-OWNERAPPTID:0
X-MICROSOFT-CDO-BUSYSTATUS:BUSY
X-MICROSOFT-CDO-INTENDEDSTATUS:BUSY
X-MICROSOFT-CDO-ALLDAYEVENT:FALSE
X-MICROSOFT-CDO-IMPORTANCE:1
X-MICROSOFT-CDO-INSTTYPE:0
X-MICROSOFT-DONOTFORWARDMEETING:FALSE
X-MICROSOFT-DISALLOW-COUNTER:FALSE
X-MICROSOFT-LOCATIONS:[]
BEGIN:VALARM
DESCRIPTION:REMINDER
TRIGGER;RELATED=START:-PT15M
ACTION:DISPLAY
END:VALARM
END:VEVENT
END:VCALENDAR
```


### <a name="example-9-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message"></a><span data-ttu-id="976d9-260">Exemplo 9: Obter o conteúdo bruto MIME de um anexo de item de convite de reunião em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="976d9-260">Example 9: Get the MIME raw contents of a meeting invitation item attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="976d9-261">Solicitação</span><span class="sxs-lookup"><span data-stu-id="976d9-261">Request</span></span>

<span data-ttu-id="976d9-262">Aqui está um exemplo da solicitação para obter o conteúdo bruto de um convite para reunião (do tipo [eventMessage](../resources/eventmessage.md)) que foi anexado a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="976d9-262">Here is an example of the request to get the raw contents of a meeting invitation (of the [eventMessage](../resources/eventmessage.md) type) that has been attached to a message.</span></span> <span data-ttu-id="976d9-263">A entidade **eventMessage** é baseada no tipo de **mensagem**.</span><span class="sxs-lookup"><span data-stu-id="976d9-263">The **eventMessage** entity is based on the **message** type.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_value_message_attachment",
  "sampleKeys": ["AAMkAGUzY5QKiAAA=","AAMkAGUzY5QKiAAABEgAQAK8ktgiIO19OqkvUZAqLmyQ="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKiAAA=/attachments/AAMkAGUzY5QKiAAABEgAQAK8ktgiIO19OqkvUZAqLmyQ=/$value
```

#### <a name="response"></a><span data-ttu-id="976d9-264">Resposta</span><span class="sxs-lookup"><span data-stu-id="976d9-264">Response</span></span>
<span data-ttu-id="976d9-265">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="976d9-265">Here is an example of the response.</span></span> 

<span data-ttu-id="976d9-266">O corpo da resposta inclui o anexo **eventMessage** no formato MIME.</span><span class="sxs-lookup"><span data-stu-id="976d9-266">The response body includes the **eventMessage** attachment in MIME format.</span></span> <span data-ttu-id="976d9-267">O corpo do **eventMessage** é truncado por questões de brevidade.</span><span class="sxs-lookup"><span data-stu-id="976d9-267">The body of the  **eventMessage** is truncated for brevity.</span></span> <span data-ttu-id="976d9-268">O corpo completo da mensagem é retornado de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="976d9-268">The full message body is returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_value_message_attachment",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK

From: Megan Bowen <MeganB@contoso.OnMicrosoft.com>
To: Adele Vance <AdeleV@contoso.OnMicrosoft.com>
Subject: Let's go for lunch
Thread-Topic: Let's go for lunch
Thread-Index: AdTPqxOmg4AXoJV960a1j5NrJCHYjA==
X-MS-Exchange-MessageSentRepresentingType: 1
Date: Thu, 28 Feb 2019 21:17:58 +0000
Message-ID:
    <CY4PR2201MB1046E9C83FC42478EF4EE283C9750@CY4PR2201MB1046.namprd22.prod.outlook.com>
Content-Language: en-US
X-MS-Has-Attach:
X-MS-Exchange-Organization-SCL: -1
X-MS-TNEF-Correlator:
X-MS-Exchange-Organization-RecordReviewCfmType: 0
Content-Type: multipart/alternative;
    boundary="_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_"
MIME-Version: 1.0

--_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_
Content-Type: text/plain; charset="us-ascii"

Does mid month work for you?

--_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_
Content-Type: text/html; charset="us-ascii"

<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=us-ascii">
</head>
<body>
Does mid month work for you?
</body>
</html>

--_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_
Content-Type: text/calendar; charset="utf-8"; method=REQUEST
Content-Transfer-Encoding: base64

QkVHSU46VkNBTEVOREFSDQpNRVRIT0Q6UkVRVUVTVA0KUFJPRElEOk1pY3Jvc29mdCBFeGNoYW5n


--_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_--
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
