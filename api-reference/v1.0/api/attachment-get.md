---
title: Obter anexo
description: 'Leia as propriedades e as relações de um anexo, anexados a um evento,  '
localization_priority: Priority
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 69160b9e583cd480c09baebed58b079472b3a65b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054200"
---
# <a name="get-attachment"></a><span data-ttu-id="c13e2-103">Obter anexo</span><span class="sxs-lookup"><span data-stu-id="c13e2-103">Get attachment</span></span>

<span data-ttu-id="c13e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c13e2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c13e2-105">Leia as propriedades, os relacionamentos ou o conteúdo bruto de um anexo que está vinculado a um usuário [evento](../resources/event.md), [mensagem](../resources/message.md), ou postagem de [grupo](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="c13e2-105">Read the properties, relationships, or raw contents of an attachment that is attached to a user [event](../resources/event.md), [message](../resources/message.md), or group [post](../resources/post.md).</span></span> 

<span data-ttu-id="c13e2-106">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="c13e2-106">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="c13e2-107">Um arquivo.</span><span class="sxs-lookup"><span data-stu-id="c13e2-107">A file.</span></span> <span data-ttu-id="c13e2-108">Programaticamente, este é um recurso [fileAttachment](../resources/fileattachment.md).</span><span class="sxs-lookup"><span data-stu-id="c13e2-108">Programmatically, this is a [fileAttachment](../resources/fileattachment.md) resource.</span></span> <span data-ttu-id="c13e2-109">Veja [exemplo 1](#example-1-get-the-properties-of-a-file-attachment).</span><span class="sxs-lookup"><span data-stu-id="c13e2-109">See [example 1](#example-1-get-the-properties-of-a-file-attachment).</span></span>
* <span data-ttu-id="c13e2-110">Um item do Outlook (contato, evento ou mensagem).</span><span class="sxs-lookup"><span data-stu-id="c13e2-110">An Outlook item (contact, event or message).</span></span> <span data-ttu-id="c13e2-111">Programaticamente, um anexo de item é um recurso [itemAttachment](../resources/itemattachment.md).</span><span class="sxs-lookup"><span data-stu-id="c13e2-111">Programmatically, an item attachment is an [itemAttachment](../resources/itemattachment.md) resource.</span></span> <span data-ttu-id="c13e2-112">Você pode usar `$expand` para obter ainda mais as propriedades desse item, incluindo quaisquer anexos aninhados em até 30 níveis.</span><span class="sxs-lookup"><span data-stu-id="c13e2-112">You can use `$expand` to further get the properties of that item, including any nested attachments up to 30 levels.</span></span> <span data-ttu-id="c13e2-113">Veja o [exemplo 3](#example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message) e o [exemplo 4](#example-4-expand-and-get-the-properties-of-an-item-attached-to-a-message-including-any-attachment-to-the-item).</span><span class="sxs-lookup"><span data-stu-id="c13e2-113">See [example 3](#example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message) and [example 4](#example-4-expand-and-get-the-properties-of-an-item-attached-to-a-message-including-any-attachment-to-the-item).</span></span>
* <span data-ttu-id="c13e2-114">Um link para um arquivo armazenado na nuvem.</span><span class="sxs-lookup"><span data-stu-id="c13e2-114">A link to a file stored in the cloud.</span></span> <span data-ttu-id="c13e2-115">Programaticamente, este é um recurso [referenceAttachment](../resources/referenceattachment.md).</span><span class="sxs-lookup"><span data-stu-id="c13e2-115">Programmatically, this is a [referenceAttachment](../resources/referenceattachment.md) resource.</span></span> <span data-ttu-id="c13e2-116">Veja o[exemplo 5](#example-5-get-the-properties-of-a-reference-attachment).</span><span class="sxs-lookup"><span data-stu-id="c13e2-116">See [example 5](#example-5-get-the-properties-of-a-reference-attachment).</span></span>

<span data-ttu-id="c13e2-117">Todos esses tipos de anexos são derivados do recurso [anexo](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="c13e2-117">All these types of attachments are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

### <a name="get-the-raw-contents-of-a-file-or-item-attachment"></a><span data-ttu-id="c13e2-118">Obter o conteúdo bruto de um arquivo ou anexo de item</span><span class="sxs-lookup"><span data-stu-id="c13e2-118">Get the raw contents of a file or item attachment</span></span>
<span data-ttu-id="c13e2-119">Você pode anexar o segmento do caminho `/$value` para obter o conteúdo bruto de um arquivo ou anexo de item.</span><span class="sxs-lookup"><span data-stu-id="c13e2-119">You can append the path segment `/$value` to get the raw contents of a file or item attachment.</span></span> 

<span data-ttu-id="c13e2-120">Para um anexo de arquivo, o tipo de conteúdo é baseado no tipo de conteúdo original.</span><span class="sxs-lookup"><span data-stu-id="c13e2-120">For a file attachment, the content type is based on its original content type.</span></span> <span data-ttu-id="c13e2-121">Veja o[exemplo 6](#example-6-get-the-raw-contents-of-a-file-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="c13e2-121">See [example 6](#example-6-get-the-raw-contents-of-a-file-attachment-on-a-message).</span></span>

<span data-ttu-id="c13e2-122">Para um anexo de item que é um [contato](../resources/contact.md), [evento](../resources/event.md) ou [mensagem](../resources/message.md), o conteúdo bruto retornado está no formato MIME.</span><span class="sxs-lookup"><span data-stu-id="c13e2-122">For an item attachment that is a [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md), the raw contents returned is in MIME format.</span></span>

| <span data-ttu-id="c13e2-123">Tipo de anexo do item</span><span class="sxs-lookup"><span data-stu-id="c13e2-123">Item attachment type</span></span>  | <span data-ttu-id="c13e2-124">Conteúdo bruto retornado</span><span class="sxs-lookup"><span data-stu-id="c13e2-124">Raw contents returned</span></span> |
|:-----------|:----------|
| <span data-ttu-id="c13e2-125">**contato**</span><span class="sxs-lookup"><span data-stu-id="c13e2-125">**contact**</span></span> | <span data-ttu-id="c13e2-126">Formato [vCard](http://www.faqs.org/rfcs/rfc2426.html) MIME.</span><span class="sxs-lookup"><span data-stu-id="c13e2-126">[vCard](http://www.faqs.org/rfcs/rfc2426.html) MIME format.</span></span> <span data-ttu-id="c13e2-127">Confira um [exemplo](#example-7-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="c13e2-127">See [example](#example-7-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message).</span></span> |
| <span data-ttu-id="c13e2-128">**event**</span><span class="sxs-lookup"><span data-stu-id="c13e2-128">**event**</span></span> | <span data-ttu-id="c13e2-129">Formato iCal MIME.</span><span class="sxs-lookup"><span data-stu-id="c13e2-129">iCal MIME format.</span></span> <span data-ttu-id="c13e2-130">Confira um [exemplo](#example-8-get-the-mime-raw-contents-of-an-event-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="c13e2-130">See [example](#example-8-get-the-mime-raw-contents-of-an-event-attachment-on-a-message).</span></span> |
| <span data-ttu-id="c13e2-131">**message**</span><span class="sxs-lookup"><span data-stu-id="c13e2-131">**message**</span></span> | <span data-ttu-id="c13e2-132">Formato MIME.</span><span class="sxs-lookup"><span data-stu-id="c13e2-132">MIME format.</span></span> <span data-ttu-id="c13e2-133">Confira um [exemplo](#example-9-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="c13e2-133">See [example](#example-9-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message).</span></span> |

<span data-ttu-id="c13e2-134">A tentativa de obter o `$value` de um anexo de referência retorna HTTP 405.</span><span class="sxs-lookup"><span data-stu-id="c13e2-134">Attempting to get the `$value` of a reference attachment returns HTTP 405.</span></span>

## <a name="permissions"></a><span data-ttu-id="c13e2-135">Permissões</span><span class="sxs-lookup"><span data-stu-id="c13e2-135">Permissions</span></span>

<span data-ttu-id="c13e2-136">Dependendo do recurso (**evento**, **mensagem** ou **postagem**) ao qual o anexo está anexado e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="c13e2-136">Depending on the resource (**event**, **message**, or **post**) that the attachment is attached to and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="c13e2-137">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c13e2-137">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c13e2-138">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="c13e2-138">Supported resource</span></span> | <span data-ttu-id="c13e2-139">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c13e2-139">Delegated (work or school account)</span></span> | <span data-ttu-id="c13e2-140">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c13e2-140">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c13e2-141">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c13e2-141">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="c13e2-142">evento</span><span class="sxs-lookup"><span data-stu-id="c13e2-142">event</span></span>](../resources/event.md) | <span data-ttu-id="c13e2-143">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c13e2-143">Calendars.Read</span></span> | <span data-ttu-id="c13e2-144">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c13e2-144">Calendars.Read</span></span> | <span data-ttu-id="c13e2-145">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c13e2-145">Calendars.Read</span></span> |
| [<span data-ttu-id="c13e2-146">message</span><span class="sxs-lookup"><span data-stu-id="c13e2-146">message</span></span>](../resources/message.md) | <span data-ttu-id="c13e2-147">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c13e2-147">Mail.Read</span></span> | <span data-ttu-id="c13e2-148">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c13e2-148">Mail.Read</span></span> | <span data-ttu-id="c13e2-149">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c13e2-149">Mail.Read</span></span> |
| [<span data-ttu-id="c13e2-150">postagem</span><span class="sxs-lookup"><span data-stu-id="c13e2-150">post</span></span>](../resources/post.md) | <span data-ttu-id="c13e2-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c13e2-151">Group.Read.All</span></span> | <span data-ttu-id="c13e2-152">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c13e2-152">Not supported</span></span> | <span data-ttu-id="c13e2-153">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c13e2-153">Not supported</span></span> |


<!--
* If accessing attachments in group events or posts: Group.Read.All.
-->

## <a name="http-request"></a><span data-ttu-id="c13e2-154">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c13e2-154">HTTP request</span></span>
<span data-ttu-id="c13e2-155">Esta seção mostra a sintaxe da solicitação HTTP GET para cada uma das entidades ([evento](../resources/event.md), [mensagem](../resources/message.md) e [postagem](../resources/post.md)) que oferecem suporte a anexos:</span><span class="sxs-lookup"><span data-stu-id="c13e2-155">This section shows the HTTP GET request syntax for each of the entities ([event](../resources/event.md), [message](../resources/message.md), and [post](../resources/post.md)) that support attachments:</span></span>

- <span data-ttu-id="c13e2-156">Para obter as propriedades e os relacionamentos de um anexo, especifique o ID do anexo a ser indexado na coleção de **anexos**, anexada ao [evento](../resources/event.md), [mensagem](../resources/message.md) ou instância de [postagem](../resources/post.md) especificada.</span><span class="sxs-lookup"><span data-stu-id="c13e2-156">To get the properties and relationships of an attachment, specify the attachment ID to index into the **attachments** collection, attached to the specified [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) instance.</span></span>
- <span data-ttu-id="c13e2-157">Se o anexo for um arquivo ou item do Outlook (contato, evento ou mensagem), você poderá obter ainda mais o conteúdo bruto do anexo anexando o segmento de caminho `/$value` à URL da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c13e2-157">If the attachment is a file or Outlook item (contact, event, or message), you can further get the raw contents of the attachment by appending the path segment `/$value` to the request URL.</span></span>

<span data-ttu-id="c13e2-158">Anexos de um [event](../resources/event.md) no [calendar](../resources/calendar.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="c13e2-158">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

<!--
Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).
-->
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}

GET /me/events/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}/$value
```

<span data-ttu-id="c13e2-159">Anexos para um [evento](../resources/event.md) no [calendário](../resources/calendar.md) do usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="c13e2-159">Attachments for an [event](../resources/event.md) in the specified user [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

GET /me/calendars/{id}/events/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}/$value
```

<!--
GET /groups/{id}/events/{id}/attachments/{id}
GET /groups/{id}/calendar/events/{id}/attachments/{id}
-->

<span data-ttu-id="c13e2-160">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence a um [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="c13e2-160">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}

GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}/$value
```
<span data-ttu-id="c13e2-161">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="c13e2-161">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}

GET /me/messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}/$value
```
<span data-ttu-id="c13e2-162">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="c13e2-162">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}

GET /me/mailFolders/{id}/messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}/$value
```
<span data-ttu-id="c13e2-p109">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante. </span><span class="sxs-lookup"><span data-stu-id="c13e2-p109">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. </span></span><!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}

GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}/$value
```
<span data-ttu-id="c13e2-165">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="c13e2-165">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}

GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c13e2-166">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c13e2-166">Optional query parameters</span></span>
<span data-ttu-id="c13e2-167">Este método também dá suporte a alguns [Parâmetros de Consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c13e2-167">This method supports some of the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="c13e2-168">Use `$expand` para obter as propriedades de um anexo de item (contato, evento ou mensagem).</span><span class="sxs-lookup"><span data-stu-id="c13e2-168">Use `$expand` to get the properties of an item attachment (contact, event, or message).</span></span> <span data-ttu-id="c13e2-169">Veja o [exemplo 3](#example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message) e o [exemplo 4](#example-4-expand-and-get-the-properties-of-an-item-attached-to-a-message-including-any-attachment-to-the-item).</span><span class="sxs-lookup"><span data-stu-id="c13e2-169">See [example 3](#example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message) and [example 4](#example-4-expand-and-get-the-properties-of-an-item-attached-to-a-message-including-any-attachment-to-the-item).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c13e2-170">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c13e2-170">Request headers</span></span>
| <span data-ttu-id="c13e2-171">Nome</span><span class="sxs-lookup"><span data-stu-id="c13e2-171">Name</span></span>       | <span data-ttu-id="c13e2-172">Tipo</span><span class="sxs-lookup"><span data-stu-id="c13e2-172">Type</span></span> | <span data-ttu-id="c13e2-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="c13e2-173">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c13e2-174">Autorização</span><span class="sxs-lookup"><span data-stu-id="c13e2-174">Authorization</span></span>  | <span data-ttu-id="c13e2-175">string</span><span class="sxs-lookup"><span data-stu-id="c13e2-175">string</span></span>  | <span data-ttu-id="c13e2-p111">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c13e2-p111">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c13e2-178">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c13e2-178">Request body</span></span>
<span data-ttu-id="c13e2-179">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c13e2-179">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c13e2-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="c13e2-180">Response</span></span>

<span data-ttu-id="c13e2-181">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="c13e2-181">If successful, this method returns a `200 OK` response code.</span></span>

<span data-ttu-id="c13e2-182">Se você estiver obtendo as propriedades e os relacionamentos de um anexo, o corpo da resposta incluirá um objeto de [anexo](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="c13e2-182">If you're getting the properties and relationships of an attachment, the response body includes an [attachment](../resources/attachment.md) object.</span></span> <span data-ttu-id="c13e2-183">As propriedades desse tipo de anexo são retornadas: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) ou [referenceAttachment](../resources/referenceattachment.md).</span><span class="sxs-lookup"><span data-stu-id="c13e2-183">The properties of that type of attachment are returned: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md).</span></span>

<span data-ttu-id="c13e2-184">Se você estiver obtendo o conteúdo bruto de um anexo de arquivo ou de item, o corpo da resposta incluirá o valor bruto do anexo.</span><span class="sxs-lookup"><span data-stu-id="c13e2-184">If you're getting the raw contents of a file or item attachment, the response body includes the raw value of the attachment.</span></span>

## <a name="examples"></a><span data-ttu-id="c13e2-185">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c13e2-185">Examples</span></span> 

### <a name="example-1-get-the-properties-of-a-file-attachment"></a><span data-ttu-id="c13e2-186">Exemplo 1: Obter as propriedades de um anexo de arquivo</span><span class="sxs-lookup"><span data-stu-id="c13e2-186">Example 1: Get the properties of a file attachment</span></span>

#### <a name="request"></a><span data-ttu-id="c13e2-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c13e2-187">Request</span></span>

<span data-ttu-id="c13e2-188">Veja um exemplo da solicitação para obter um anexo de arquivo de um evento.</span><span class="sxs-lookup"><span data-stu-id="c13e2-188">Here is an example of the request to get a file attachment on an event.</span></span>

# <a name="http"></a>[<span data-ttu-id="c13e2-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="c13e2-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_file_attachment_v1",
  "sampleKeys": ["AAMkAGUzY5QKjAAA=","AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=
```
# <a name="c"></a>[<span data-ttu-id="c13e2-190">C#</span><span class="sxs-lookup"><span data-stu-id="c13e2-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-file-attachment-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c13e2-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c13e2-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-file-attachment-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c13e2-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c13e2-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-file-attachment-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c13e2-193">Java</span><span class="sxs-lookup"><span data-stu-id="c13e2-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-file-attachment-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c13e2-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="c13e2-194">Response</span></span>
<span data-ttu-id="c13e2-195">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c13e2-195">Here is an example of the response.</span></span> <span data-ttu-id="c13e2-196">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c13e2-196">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_file_attachment_v1",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages('AAMkAGUzY5QKjAAA%3D')/attachments/$entity",
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
### <a name="example-2-get-the-properties-of-an-item-attachment"></a><span data-ttu-id="c13e2-197">Exemplo 2: Obter as propriedades de um anexo de item</span><span class="sxs-lookup"><span data-stu-id="c13e2-197">Example 2: Get the properties of an item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="c13e2-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c13e2-198">Request</span></span>

<span data-ttu-id="c13e2-199">O próximo exemplo mostra como obter um anexo de item em uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="c13e2-199">The next example shows how to get an item attachment on a message.</span></span> <span data-ttu-id="c13e2-200">As propriedades de **itemAttachment** são retornadas.</span><span class="sxs-lookup"><span data-stu-id="c13e2-200">The properties of the **itemAttachment** are returned.</span></span>

# <a name="http"></a>[<span data-ttu-id="c13e2-201">HTTP</span><span class="sxs-lookup"><span data-stu-id="c13e2-201">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1M-zAAA=", "AAMkADA1M-CJKtzmnlcqVgqI="],
  "name": "get_item_attachment"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=
```
# <a name="c"></a>[<span data-ttu-id="c13e2-202">C#</span><span class="sxs-lookup"><span data-stu-id="c13e2-202">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c13e2-203">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c13e2-203">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c13e2-204">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c13e2-204">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c13e2-205">Java</span><span class="sxs-lookup"><span data-stu-id="c13e2-205">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c13e2-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="c13e2-206">Response</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false
}
```

### <a name="example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message"></a><span data-ttu-id="c13e2-207">Exemplo 3: Expandir e obter as propriedades do item anexado a uma mensagem</span><span class="sxs-lookup"><span data-stu-id="c13e2-207">Example 3: Expand and get the properties of the item attached to a message</span></span>
#### <a name="request"></a><span data-ttu-id="c13e2-208">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c13e2-208">Request</span></span>
<span data-ttu-id="c13e2-209">O próximo exemplo mostra como usar `$expand` para obter as propriedades do item (contato, evento ou mensagem) anexado à mensagem.</span><span class="sxs-lookup"><span data-stu-id="c13e2-209">The next example shows how to use `$expand` to get the properties of the item (contact, event, or message) that is attached to the message.</span></span> <span data-ttu-id="c13e2-210">Neste exemplo, esse item é uma mensagem. As propriedades dessa mensagem anexadas também são retornadas.</span><span class="sxs-lookup"><span data-stu-id="c13e2-210">In this example, that item is a message; the properties of that attached message are also returned.</span></span>

# <a name="http"></a>[<span data-ttu-id="c13e2-211">HTTP</span><span class="sxs-lookup"><span data-stu-id="c13e2-211">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1M-zAAA=", "AAMkADA1M-CJKtzmnlcqVgqI="],
  "name": "get_and_expand_item_attachment"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=/?$expand=microsoft.graph.itemattachment/item 
```
# <a name="c"></a>[<span data-ttu-id="c13e2-212">C#</span><span class="sxs-lookup"><span data-stu-id="c13e2-212">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-and-expand-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c13e2-213">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c13e2-213">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-and-expand-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c13e2-214">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c13e2-214">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-and-expand-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c13e2-215">Java</span><span class="sxs-lookup"><span data-stu-id="c13e2-215">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-and-expand-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c13e2-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="c13e2-216">Response</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false,
  "item@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments('AAMkADA1M-CJKtzmnlcqVgqI%3D')/microsoft.graph.itemAttachment/item/$entity",
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

### <a name="example-4-expand-and-get-the-properties-of-an-item-attached-to-a-message-including-any-attachment-to-the-item"></a><span data-ttu-id="c13e2-217">Exemplo 4: Expanda e obtenha as propriedades de um item anexado a uma mensagem, incluindo qualquer anexo do item</span><span class="sxs-lookup"><span data-stu-id="c13e2-217">Example 4: Expand and get the properties of an item attached to a message, including any attachment to the item</span></span>
#### <a name="request"></a><span data-ttu-id="c13e2-218">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c13e2-218">Request</span></span>
<span data-ttu-id="c13e2-219">O próximo exemplo usa a mesma solicitação do [exemplo 3](#example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message) para obter as propriedades de um anexo de item em uma mensagem usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="c13e2-219">The next example uses the same request as in [example 3](#example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message) to get the properties of an item attachment on a message by using `$expand`.</span></span> <span data-ttu-id="c13e2-220">Nesse caso, como o item anexado também contém um anexo de arquivo, a resposta também inclui as propriedades do anexo de arquivo.</span><span class="sxs-lookup"><span data-stu-id="c13e2-220">In this case, because the attached item also has a file attachment, the response includes the properties of the file attachment as well.</span></span> 

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1M-zAAA=", "AAMkADA1M-CJKtzmnlcqVgqI="],
  "name": "get_and_expand_nested_item_attachment"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=/?$expand=microsoft.graph.itemattachment/item 
```

#### <a name="response"></a><span data-ttu-id="c13e2-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="c13e2-221">Response</span></span>
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

### <a name="example-5-get-the-properties-of-a-reference-attachment"></a><span data-ttu-id="c13e2-222">Exemplo 5: Obtenha as propriedades de um anexo de referência</span><span class="sxs-lookup"><span data-stu-id="c13e2-222">Example 5: Get the properties of a reference attachment</span></span>

#### <a name="request"></a><span data-ttu-id="c13e2-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c13e2-223">Request</span></span>
<span data-ttu-id="c13e2-224">Aqui está um exemplo da solicitação para obter um anexo de referência de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="c13e2-224">Here is an example of the request to get a reference attachment on a message.</span></span>

# <a name="http"></a>[<span data-ttu-id="c13e2-225">HTTP</span><span class="sxs-lookup"><span data-stu-id="c13e2-225">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment",
  "sampleKeys": ["AAMkAGUzY5QKgAAA=","AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8="]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGUzY5QKgAAA=/attachments/AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8=
```
# <a name="c"></a>[<span data-ttu-id="c13e2-226">C#</span><span class="sxs-lookup"><span data-stu-id="c13e2-226">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reference-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c13e2-227">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c13e2-227">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reference-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c13e2-228">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c13e2-228">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reference-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c13e2-229">Java</span><span class="sxs-lookup"><span data-stu-id="c13e2-229">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-reference-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="c13e2-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="c13e2-230">Response</span></span>
<span data-ttu-id="c13e2-231">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c13e2-231">Here is an example of the response.</span></span> <span data-ttu-id="c13e2-232">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c13e2-232">Note: The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages('AAMkAGUzY5QKgAAA%3D')/attachments/$entity",
    "@odata.type": "#microsoft.graph.referenceAttachment",
    "id": "AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8=",
    "lastModifiedDateTime": "2019-04-02T02:58:11Z",
    "name": "Sales Invoice Template.docx",
    "contentType": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
    "size": 1060,
    "isInline": true
}
```

### <a name="example-6-get-the-raw-contents-of-a-file-attachment-on-a-message"></a><span data-ttu-id="c13e2-233">Exemplo 6: Obtenha o conteúdo bruto de um anexo de arquivo em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="c13e2-233">Example 6: Get the raw contents of a file attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="c13e2-234">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c13e2-234">Request</span></span>

<span data-ttu-id="c13e2-235">Aqui está um exemplo da solicitação para obter o conteúdo bruto de um arquivo do Word que foi anexado a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="c13e2-235">Here is an example of the request to get the raw contents of a Word file that has been attached to a message.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_value_file_attachment",
  "sampleKeys": ["AAMkAGUzY5QKjAAA=","AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
}-->

```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=/$value
```

#### <a name="response"></a><span data-ttu-id="c13e2-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="c13e2-236">Response</span></span>
<span data-ttu-id="c13e2-p118">Aqui está um exemplo da resposta. O corpo de resposta real inclui os bytes brutos do anexo do arquivo, que são abreviados aqui para brevidade.</span><span class="sxs-lookup"><span data-stu-id="c13e2-p118">Here is an example of the response. The actual response body includes the raw bytes of the file attachment, which are abbreviated here for brevity.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_value_file_attachment",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK

{Raw bytes of the file}
```


### <a name="example-7-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message"></a><span data-ttu-id="c13e2-239">Exemplo 7: Obtenha o conteúdo bruto MIME de um anexo de contato em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="c13e2-239">Example 7: Get the MIME raw contents of a contact attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="c13e2-240">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c13e2-240">Request</span></span>

<span data-ttu-id="c13e2-241">Aqui está um exemplo da solicitação para obter o conteúdo bruto de um item de contato que foi anexado a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="c13e2-241">Here is an example of the request to get the raw contents of a contact item that has been attached to a message.</span></span> 
<!-- {
  "blockType": "ignored",
  "name": "get_value_contact_attachment",
  "sampleKeys": ["AAMkADI5MAAGjk2PxAAA=","AAMkADI5MAAGjk2PxAAABEgAQACEJqrbJZBNIlr3pGFvd9K8="]
}-->

```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADI5MAAGjk2PxAAA=/attachments/AAMkADI5MAAGjk2PxAAABEgAQACEJqrbJZBNIlr3pGFvd9K8=/$value
```

#### <a name="response"></a><span data-ttu-id="c13e2-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="c13e2-242">Response</span></span>
<span data-ttu-id="c13e2-243">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c13e2-243">Here is an example of the response.</span></span> 

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


### <a name="example-8-get-the-mime-raw-contents-of-an-event-attachment-on-a-message"></a><span data-ttu-id="c13e2-244">Exemplo 8: Obtenha o conteúdo bruto MIME de um anexo de evento em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="c13e2-244">Example 8: Get the MIME raw contents of an event attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="c13e2-245">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c13e2-245">Request</span></span>

<span data-ttu-id="c13e2-246">Aqui está um exemplo da solicitação para obter o conteúdo bruto de um evento que foi anexado a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="c13e2-246">Here is an example of the request to get the raw contents of an event that has been attached to a message.</span></span> 
<!-- {
  "blockType": "ignored",
  "name": "get_value_event_attachment",
  "sampleKeys": ["AAMkADVIOAAA=","AAMkADVIOAAABEgAQACvkutl6c4FMifPyS6NvXsM="]
}-->

```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADVIOAAA=/attachments/AAMkADVIOAAABEgAQACvkutl6c4FMifPyS6NvXsM=/$value
```

#### <a name="response"></a><span data-ttu-id="c13e2-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="c13e2-247">Response</span></span>
<span data-ttu-id="c13e2-248">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c13e2-248">Here is an example of the response.</span></span> 

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


### <a name="example-9-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message"></a><span data-ttu-id="c13e2-249">Exemplo 9: Obtenha o conteúdo bruto MIME de um anexo de item de convite de reunião em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="c13e2-249">Example 9: Get the MIME raw contents of a meeting invitation item attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="c13e2-250">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c13e2-250">Request</span></span>

<span data-ttu-id="c13e2-251">Aqui está um exemplo da solicitação para obter o conteúdo bruto de um convite para reunião (do tipo [eventMessage](../resources/eventmessage.md)) que foi anexado a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="c13e2-251">Here is an example of the request to get the raw contents of a meeting invitation (of the [eventMessage](../resources/eventmessage.md) type) that has been attached to a message.</span></span> <span data-ttu-id="c13e2-252">A entidade **eventMessage** é baseada no tipo de **mensagem**.</span><span class="sxs-lookup"><span data-stu-id="c13e2-252">The **eventMessage** entity is based on the **message** type.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_value_message_attachment",
  "sampleKeys": ["AAMkAGUzY5QKiAAA=","AAMkAGUzY5QKiAAABEgAQAK8ktgiIO19OqkvUZAqLmyQ="]
}-->

```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGUzY5QKiAAA=/attachments/AAMkAGUzY5QKiAAABEgAQAK8ktgiIO19OqkvUZAqLmyQ=/$value
```

#### <a name="response"></a><span data-ttu-id="c13e2-253">Resposta</span><span class="sxs-lookup"><span data-stu-id="c13e2-253">Response</span></span>
<span data-ttu-id="c13e2-254">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c13e2-254">Here is an example of the response.</span></span> 

<span data-ttu-id="c13e2-255">O corpo da resposta inclui o anexo **eventMessage** no formato MIME.</span><span class="sxs-lookup"><span data-stu-id="c13e2-255">The response body includes the **eventMessage** attachment in MIME format.</span></span> <span data-ttu-id="c13e2-256">O corpo do **eventMessage** é truncado por questões de brevidade.</span><span class="sxs-lookup"><span data-stu-id="c13e2-256">The body of the  **eventMessage** is truncated for brevity.</span></span> <span data-ttu-id="c13e2-257">O corpo completo da mensagem é retornado de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c13e2-257">The full message body is returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get attachment",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
  ],
  "tocPath": ""
}-->
