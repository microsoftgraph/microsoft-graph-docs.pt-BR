---
title: Obter anexo
description: 'Leia as propriedades e as relações de um anexo, anexados a um evento,  '
localization_priority: Priority
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9429146c099a981abf2779d9f7f8a8334c1a89aa
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48403766"
---
# <a name="get-attachment"></a><span data-ttu-id="9430c-103">Obter anexo</span><span class="sxs-lookup"><span data-stu-id="9430c-103">Get attachment</span></span>

<span data-ttu-id="9430c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9430c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9430c-105">Leia as propriedades, os relacionamentos ou o conteúdo bruto de um anexo de um [evento](../resources/event.md), [mensagem](../resources/message.md) ou [postagem](../resources/post.md) do usuário.</span><span class="sxs-lookup"><span data-stu-id="9430c-105">Read the properties, relationships, or raw contents of an attachment, attached to a user [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md).</span></span> 

<span data-ttu-id="9430c-106">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="9430c-106">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="9430c-107">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="9430c-107">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="9430c-108">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="9430c-108">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span> <span data-ttu-id="9430c-109">Você pode usar `$expand` para obter mais propriedades desse item.</span><span class="sxs-lookup"><span data-stu-id="9430c-109">You can use `$expand` to further get the properties of that item.</span></span> <span data-ttu-id="9430c-110">Veja um [exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="9430c-110">See an [example](#request-2) below.</span></span>
* <span data-ttu-id="9430c-111">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="9430c-111">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="9430c-112">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="9430c-112">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

### <a name="get-the-raw-contents-of-a-file-or-item-attachment"></a><span data-ttu-id="9430c-113">Obter o conteúdo bruto de um arquivo ou anexo de item</span><span class="sxs-lookup"><span data-stu-id="9430c-113">Get the raw contents of a file or item attachment</span></span>
<span data-ttu-id="9430c-114">Você pode anexar o segmento do caminho `/$value` para obter o conteúdo bruto de um arquivo ou anexo de item.</span><span class="sxs-lookup"><span data-stu-id="9430c-114">You can append the path segment `/$value` to get the raw contents of a file or item attachment.</span></span> 

<span data-ttu-id="9430c-115">Para um anexo de arquivo, o tipo de conteúdo é baseado no tipo de conteúdo original.</span><span class="sxs-lookup"><span data-stu-id="9430c-115">For a file attachment, the content type is based on its original content type.</span></span> <span data-ttu-id="9430c-116">Veja um [exemplo](#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message) abaixo.</span><span class="sxs-lookup"><span data-stu-id="9430c-116">See an [example](#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message) below.</span></span>

<span data-ttu-id="9430c-117">Para um anexo de item que é um [contato](../resources/contact.md), [evento](../resources/event.md) ou [mensagem](../resources/message.md), o conteúdo bruto retornado está no formato MIME.</span><span class="sxs-lookup"><span data-stu-id="9430c-117">For an item attachment that is a [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md), the raw contents returned is in MIME format.</span></span>

| <span data-ttu-id="9430c-118">Tipo de anexo do item</span><span class="sxs-lookup"><span data-stu-id="9430c-118">Item attachment type</span></span>  | <span data-ttu-id="9430c-119">Conteúdo bruto retornado</span><span class="sxs-lookup"><span data-stu-id="9430c-119">Raw contents returned</span></span> |
|:-----------|:----------|
| <span data-ttu-id="9430c-120">**contato**</span><span class="sxs-lookup"><span data-stu-id="9430c-120">**contact**</span></span> | <span data-ttu-id="9430c-121">Formato [vCard](http://www.faqs.org/rfcs/rfc2426.html) MIME.</span><span class="sxs-lookup"><span data-stu-id="9430c-121">[vCard](http://www.faqs.org/rfcs/rfc2426.html) MIME format.</span></span> <span data-ttu-id="9430c-122">Confira um [exemplo](#example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="9430c-122">See [example](#example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message).</span></span> |
| <span data-ttu-id="9430c-123">**event**</span><span class="sxs-lookup"><span data-stu-id="9430c-123">**event**</span></span> | <span data-ttu-id="9430c-124">Formato iCal MIME.</span><span class="sxs-lookup"><span data-stu-id="9430c-124">iCal MIME format.</span></span> <span data-ttu-id="9430c-125">Confira um [exemplo](#example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="9430c-125">See [example](#example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message).</span></span> |
| <span data-ttu-id="9430c-126">**message**</span><span class="sxs-lookup"><span data-stu-id="9430c-126">**message**</span></span> | <span data-ttu-id="9430c-127">Formato MIME.</span><span class="sxs-lookup"><span data-stu-id="9430c-127">MIME format.</span></span> <span data-ttu-id="9430c-128">Confira um [exemplo](#example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="9430c-128">See [example](#example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message).</span></span> |

<span data-ttu-id="9430c-129">A tentativa de obter o `$value` de um anexo de referência retorna HTTP 405.</span><span class="sxs-lookup"><span data-stu-id="9430c-129">Attempting to get the `$value` of a reference attachment returns HTTP 405.</span></span>

## <a name="permissions"></a><span data-ttu-id="9430c-130">Permissões</span><span class="sxs-lookup"><span data-stu-id="9430c-130">Permissions</span></span>
<span data-ttu-id="9430c-p106">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9430c-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="9430c-133">Se estiver acessando anexos em Mensagens: Mail.Read.</span><span class="sxs-lookup"><span data-stu-id="9430c-133">If accessing attachments in messages: Mail.Read.</span></span>
* <span data-ttu-id="9430c-134">Se estiver acessando anexos em Eventos: Calendars.Read.</span><span class="sxs-lookup"><span data-stu-id="9430c-134">If accessing attachments in events: Calendars.Read.</span></span>
* <span data-ttu-id="9430c-135">Se estiver acessando anexos em postagens de grupo: Group.Read.All.</span><span class="sxs-lookup"><span data-stu-id="9430c-135">If accessing attachments in group posts: Group.Read.All.</span></span>

<!--
* If accessing attachments in group events or posts: Group.Read.All.
-->

## <a name="http-request"></a><span data-ttu-id="9430c-136">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9430c-136">HTTP request</span></span>
<span data-ttu-id="9430c-137">Esta seção mostra a sintaxe da solicitação HTTP GET para cada uma das entidades ([evento](../resources/event.md), [mensagem](../resources/message.md) e [postagem](../resources/post.md)) que oferecem suporte a anexos:</span><span class="sxs-lookup"><span data-stu-id="9430c-137">This section shows the HTTP GET request syntax for each of the entities ([event](../resources/event.md), [message](../resources/message.md), and [post](../resources/post.md)) that support attachments:</span></span>

- <span data-ttu-id="9430c-138">Para obter as propriedades e os relacionamentos de um anexo, especifique o ID do anexo a ser indexado na coleção de **anexos**, anexada ao [evento](../resources/event.md), [mensagem](../resources/message.md) ou instância de [postagem](../resources/post.md) especificada.</span><span class="sxs-lookup"><span data-stu-id="9430c-138">To get the properties and relationships of an attachment, specify the attachment ID to index into the **attachments** collection, attached to the specified [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) instance.</span></span>
- <span data-ttu-id="9430c-139">Se o anexo for um arquivo ou item do Outlook (contato, evento ou mensagem), você poderá obter ainda mais o conteúdo bruto do anexo anexando o segmento de caminho `/$value` à URL da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9430c-139">If the attachment is a file or Outlook item (contact, event, or message), you can further get the raw contents of the attachment by appending the path segment `/$value` to the request URL.</span></span>

<span data-ttu-id="9430c-140">Anexos de um [event](../resources/event.md) no [calendar](../resources/calendar.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="9430c-140">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

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

<span data-ttu-id="9430c-141">Anexos para um [evento](../resources/event.md) no [calendário](../resources/calendar.md) do usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="9430c-141">Attachments for an [event](../resources/event.md) in the specified user [calendar](../resources/calendar.md).</span></span>
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

<span data-ttu-id="9430c-142">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence ao [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="9430c-142">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}

GET /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}/$value
```
<span data-ttu-id="9430c-143">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence a um [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="9430c-143">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}

GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}/$value
```
<span data-ttu-id="9430c-144">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="9430c-144">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}

GET /me/messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}/$value
```
<span data-ttu-id="9430c-145">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="9430c-145">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}

GET /me/mailFolders/{id}/messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}/$value
```
<span data-ttu-id="9430c-p107">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante. </span><span class="sxs-lookup"><span data-stu-id="9430c-p107">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. </span></span><!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}

GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}/$value
```
<span data-ttu-id="9430c-148">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="9430c-148">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}

GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9430c-149">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9430c-149">Optional query parameters</span></span>
<span data-ttu-id="9430c-150">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9430c-150">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9430c-151">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9430c-151">Request headers</span></span>
| <span data-ttu-id="9430c-152">Nome</span><span class="sxs-lookup"><span data-stu-id="9430c-152">Name</span></span>       | <span data-ttu-id="9430c-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="9430c-153">Type</span></span> | <span data-ttu-id="9430c-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="9430c-154">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9430c-155">Autorização</span><span class="sxs-lookup"><span data-stu-id="9430c-155">Authorization</span></span>  | <span data-ttu-id="9430c-156">string</span><span class="sxs-lookup"><span data-stu-id="9430c-156">string</span></span>  | <span data-ttu-id="9430c-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9430c-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9430c-159">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9430c-159">Request body</span></span>
<span data-ttu-id="9430c-160">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9430c-160">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9430c-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="9430c-161">Response</span></span>

<span data-ttu-id="9430c-162">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="9430c-162">If successful, this method returns a `200 OK` response code.</span></span>

<span data-ttu-id="9430c-163">Se você estiver obtendo as propriedades e os relacionamentos de um anexo, o corpo da resposta incluirá um objeto de [anexo](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="9430c-163">If you're getting the properties and relationships of an attachment, the response body includes an [attachment](../resources/attachment.md) object.</span></span> <span data-ttu-id="9430c-164">As propriedades desse tipo de anexo são retornadas: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) ou [referenceAttachment](../resources/referenceattachment.md).</span><span class="sxs-lookup"><span data-stu-id="9430c-164">The properties of that type of attachment are returned: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md).</span></span>

<span data-ttu-id="9430c-165">Se você estiver obtendo o conteúdo bruto de um anexo de arquivo ou de item, o corpo da resposta incluirá o valor bruto do anexo.</span><span class="sxs-lookup"><span data-stu-id="9430c-165">If you're getting the raw contents of a file or item attachment, the response body includes the raw value of the attachment.</span></span>

## <a name="examples"></a><span data-ttu-id="9430c-166">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9430c-166">Examples</span></span> 

### <a name="example-1-get-the-properties-of-a-file-attachment"></a><span data-ttu-id="9430c-167">Exemplo 1: Obter as propriedades de um anexo de arquivo</span><span class="sxs-lookup"><span data-stu-id="9430c-167">Example 1: Get the properties of a file attachment</span></span>

#### <a name="request"></a><span data-ttu-id="9430c-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9430c-168">Request</span></span>

<span data-ttu-id="9430c-169">Veja um exemplo da solicitação para obter um anexo de arquivo de um evento.</span><span class="sxs-lookup"><span data-stu-id="9430c-169">Here is an example of the request to get a file attachment on an event.</span></span>

# <a name="http"></a>[<span data-ttu-id="9430c-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="9430c-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_file_attachment_v1",
  "sampleKeys": ["AAMkAGUzY5QKjAAA=","AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=
```
# <a name="c"></a>[<span data-ttu-id="9430c-171">C#</span><span class="sxs-lookup"><span data-stu-id="9430c-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-file-attachment-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9430c-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9430c-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-file-attachment-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9430c-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9430c-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-file-attachment-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9430c-174">Java</span><span class="sxs-lookup"><span data-stu-id="9430c-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-file-attachment-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9430c-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="9430c-175">Response</span></span>
<span data-ttu-id="9430c-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9430c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
### <a name="example-2-get-the-properties-of-an-item-attachment"></a><span data-ttu-id="9430c-179">Exemplo 2: Obter as propriedades de um anexo de item</span><span class="sxs-lookup"><span data-stu-id="9430c-179">Example 2: Get the properties of an item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="9430c-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9430c-180">Request</span></span>

<span data-ttu-id="9430c-181">O próximo exemplo mostra como obter um anexo de item em uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="9430c-181">The next example shows how to get an item attachment on a message.</span></span> <span data-ttu-id="9430c-182">As propriedades de **itemAttachment** são retornadas.</span><span class="sxs-lookup"><span data-stu-id="9430c-182">The properties of the **itemAttachment** are returned.</span></span>

# <a name="http"></a>[<span data-ttu-id="9430c-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="9430c-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1M-zAAA=", "AAMkADA1M-CJKtzmnlcqVgqI="],
  "name": "get_item_attachment"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=
```
# <a name="c"></a>[<span data-ttu-id="9430c-184">C#</span><span class="sxs-lookup"><span data-stu-id="9430c-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9430c-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9430c-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9430c-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9430c-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9430c-187">Java</span><span class="sxs-lookup"><span data-stu-id="9430c-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9430c-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="9430c-188">Response</span></span>
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

### <a name="example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message"></a><span data-ttu-id="9430c-189">Exemplo 3: Expandir e obter as propriedades do item anexado a uma mensagem</span><span class="sxs-lookup"><span data-stu-id="9430c-189">Example 3: Expand and get the properties of the item attached to a message</span></span>
#### <a name="request"></a><span data-ttu-id="9430c-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9430c-190">Request</span></span>
<span data-ttu-id="9430c-191">O próximo exemplo mostra como usar `$expand` para obter as propriedades do item (contato, evento ou mensagem) anexado à mensagem.</span><span class="sxs-lookup"><span data-stu-id="9430c-191">The next example shows how to use `$expand` to get the properties of the item (contact, event, or message) that is attached to the message.</span></span> <span data-ttu-id="9430c-192">Neste exemplo, esse item é uma mensagem. As propriedades dessa mensagem anexadas também são retornadas.</span><span class="sxs-lookup"><span data-stu-id="9430c-192">In this example, that item is a message; the properties of that attached message are also returned.</span></span>

# <a name="http"></a>[<span data-ttu-id="9430c-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="9430c-193">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1M-zAAA=", "AAMkADA1M-CJKtzmnlcqVgqI="],
  "name": "get_and_expand_item_attachment"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=/?$expand=microsoft.graph.itemattachment/item 
```
# <a name="c"></a>[<span data-ttu-id="9430c-194">C#</span><span class="sxs-lookup"><span data-stu-id="9430c-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-and-expand-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9430c-195">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9430c-195">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-and-expand-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9430c-196">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9430c-196">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-and-expand-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9430c-197">Java</span><span class="sxs-lookup"><span data-stu-id="9430c-197">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-and-expand-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9430c-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="9430c-198">Response</span></span>
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
    "importance":"normal",
    "conversationId":"AAQkADA1MzMyOGI4LTlkZDctNDkzYy05M2RiLTdiN2E1NDE3MTRkOQAQAMG_NSCMBqdKrLa2EmR-lO0=",
    "conversationIndex":"AQHTAbcSwb41IIwGp0qstrYSZH+U7Q==",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADA1M3MTRkOQAAAA%3D%3D&exvsurl=1&viewmodel=ReadMessageItem",
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
    ]
  }
}
```



### <a name="example-4-get-the-properties-of-a-reference-attachment"></a><span data-ttu-id="9430c-199">Exemplo 4: Obter as propriedades de um anexo de referência</span><span class="sxs-lookup"><span data-stu-id="9430c-199">Example 4: Get the properties of a reference attachment</span></span>

#### <a name="request"></a><span data-ttu-id="9430c-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9430c-200">Request</span></span>
<span data-ttu-id="9430c-201">Aqui está um exemplo da solicitação para obter um anexo de referência de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="9430c-201">Here is an example of the request to get a reference attachment on a message.</span></span>

# <a name="http"></a>[<span data-ttu-id="9430c-202">HTTP</span><span class="sxs-lookup"><span data-stu-id="9430c-202">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment",
  "sampleKeys": ["AAMkAGUzY5QKgAAA=","AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8="]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGUzY5QKgAAA=/attachments/AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8=
```
# <a name="c"></a>[<span data-ttu-id="9430c-203">C#</span><span class="sxs-lookup"><span data-stu-id="9430c-203">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reference-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9430c-204">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9430c-204">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reference-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9430c-205">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9430c-205">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reference-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9430c-206">Java</span><span class="sxs-lookup"><span data-stu-id="9430c-206">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-reference-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9430c-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="9430c-207">Response</span></span>
<span data-ttu-id="9430c-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9430c-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-5-get-the-raw-contents-of-a-file-attachment-on-a-message"></a><span data-ttu-id="9430c-211">Exemplo 5: Obter o conteúdo bruto de um anexo de arquivo em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="9430c-211">Example 5: Get the raw contents of a file attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="9430c-212">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9430c-212">Request</span></span>

<span data-ttu-id="9430c-213">Aqui está um exemplo da solicitação para obter o conteúdo bruto de um arquivo do Word que foi anexado a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="9430c-213">Here is an example of the request to get the raw contents of a Word file that has been attached to a message.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_value_file_attachment",
  "sampleKeys": ["AAMkAGUzY5QKjAAA=","AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
}-->

```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=/$value
```

#### <a name="response"></a><span data-ttu-id="9430c-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="9430c-214">Response</span></span>
<span data-ttu-id="9430c-215">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9430c-215">Here is an example of the response.</span></span> <span data-ttu-id="9430c-216">O corpo da resposta real inclui os bytes brutos do anexo do arquivo, que são abreviados aqui por questões de brevidade.</span><span class="sxs-lookup"><span data-stu-id="9430c-216">The actual response body includes the raw bytes of the file attachment, which are abbreviated here for brevity.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_value_file_attachment",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK

{Raw bytes of the file}
```


### <a name="example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message"></a><span data-ttu-id="9430c-217">Exemplo 6: obter o conteúdo bruto MIME de um anexo de contato em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="9430c-217">Example 6: Get the MIME raw contents of a contact attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="9430c-218">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9430c-218">Request</span></span>

<span data-ttu-id="9430c-219">Aqui está um exemplo da solicitação para obter o conteúdo bruto de um item de contato que foi anexado a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="9430c-219">Here is an example of the request to get the raw contents of a contact item that has been attached to a message.</span></span> 
<!-- {
  "blockType": "ignored",
  "name": "get_value_contact_attachment",
  "sampleKeys": ["AAMkADI5MAAGjk2PxAAA=","AAMkADI5MAAGjk2PxAAABEgAQACEJqrbJZBNIlr3pGFvd9K8="]
}-->

```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADI5MAAGjk2PxAAA=/attachments/AAMkADI5MAAGjk2PxAAABEgAQACEJqrbJZBNIlr3pGFvd9K8=/$value
```

#### <a name="response"></a><span data-ttu-id="9430c-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="9430c-220">Response</span></span>
<span data-ttu-id="9430c-221">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9430c-221">Here is an example of the response.</span></span> 

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


### <a name="example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message"></a><span data-ttu-id="9430c-222">Exemplo 7: Obter o conteúdo bruto MIME de um anexo de evento em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="9430c-222">Example 7: Get the MIME raw contents of an event attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="9430c-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9430c-223">Request</span></span>

<span data-ttu-id="9430c-224">Aqui está um exemplo da solicitação para obter o conteúdo bruto de um evento que foi anexado a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="9430c-224">Here is an example of the request to get the raw contents of an event that has been attached to a message.</span></span> 
<!-- {
  "blockType": "ignored",
  "name": "get_value_event_attachment",
  "sampleKeys": ["AAMkADVIOAAA=","AAMkADVIOAAABEgAQACvkutl6c4FMifPyS6NvXsM="]
}-->

```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADVIOAAA=/attachments/AAMkADVIOAAABEgAQACvkutl6c4FMifPyS6NvXsM=/$value
```

#### <a name="response"></a><span data-ttu-id="9430c-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="9430c-225">Response</span></span>
<span data-ttu-id="9430c-226">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9430c-226">Here is an example of the response.</span></span> 

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


### <a name="example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message"></a><span data-ttu-id="9430c-227">Exemplo 8: Obter o conteúdo bruto MIME de um anexo de item de convite de reunião em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="9430c-227">Example 8: Get the MIME raw contents of a meeting invitation item attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="9430c-228">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9430c-228">Request</span></span>

<span data-ttu-id="9430c-229">Aqui está um exemplo da solicitação para obter o conteúdo bruto de um convite para reunião (do tipo [eventMessage](../resources/eventmessage.md)) que foi anexado a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="9430c-229">Here is an example of the request to get the raw contents of a meeting invitation (of the [eventMessage](../resources/eventmessage.md) type) that has been attached to a message.</span></span> <span data-ttu-id="9430c-230">A entidade **eventMessage** é baseada no tipo de **mensagem**.</span><span class="sxs-lookup"><span data-stu-id="9430c-230">The **eventMessage** entity is based on the **message** type.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_value_message_attachment",
  "sampleKeys": ["AAMkAGUzY5QKiAAA=","AAMkAGUzY5QKiAAABEgAQAK8ktgiIO19OqkvUZAqLmyQ="]
}-->

```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGUzY5QKiAAA=/attachments/AAMkAGUzY5QKiAAABEgAQAK8ktgiIO19OqkvUZAqLmyQ=/$value
```

#### <a name="response"></a><span data-ttu-id="9430c-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="9430c-231">Response</span></span>
<span data-ttu-id="9430c-232">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9430c-232">Here is an example of the response.</span></span> 

<span data-ttu-id="9430c-233">O corpo da resposta inclui o anexo **eventMessage** no formato MIME.</span><span class="sxs-lookup"><span data-stu-id="9430c-233">The response body includes the **eventMessage** attachment in MIME format.</span></span> <span data-ttu-id="9430c-234">O corpo do **eventMessage** é truncado por questões de brevidade.</span><span class="sxs-lookup"><span data-stu-id="9430c-234">The body of the  **eventMessage** is truncated for brevity.</span></span> <span data-ttu-id="9430c-235">O corpo completo da mensagem é retornado de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9430c-235">The full message body is returned from an actual call.</span></span>

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
    "Error: get_and_expand_item_attachment/item:
      Property 'item' is of type Custom but has no custom members."
  ],
  "tocPath": ""
}-->