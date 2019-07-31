---
title: Obter anexo
description: Leia as propriedades e as relações de um anexo, anexados a um evento, mensagem, tarefa do Outlook ou postagem.
localization_priority: Normal
doc_type: apiPageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 09a336da0f2ead60235240b60b3539007df6bd15
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945358"
---
# <a name="get-attachment"></a><span data-ttu-id="ff37d-103">Obter anexo</span><span class="sxs-lookup"><span data-stu-id="ff37d-103">Get attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff37d-104">Leia as propriedades e as relações de um anexo, anexados a um [evento](../resources/event.md), [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postagem](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="ff37d-104">Read the properties and relationships of an attachment, attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>

<span data-ttu-id="ff37d-105">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="ff37d-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="ff37d-106">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="ff37d-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="ff37d-107">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="ff37d-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span> <span data-ttu-id="ff37d-108">Você pode usar `$expand` o para obter as propriedades desse item.</span><span class="sxs-lookup"><span data-stu-id="ff37d-108">You can use `$expand` to further get the properties of that item.</span></span> <span data-ttu-id="ff37d-109">Veja um [exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="ff37d-109">See an [example](#request-2) below.</span></span>
* <span data-ttu-id="ff37d-110">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="ff37d-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="ff37d-111">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="ff37d-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span>

### <a name="get-the-raw-contents-of-a-file-or-item-attachment"></a><span data-ttu-id="ff37d-112">Obter o conteúdo bruto de um arquivo ou anexo de item</span><span class="sxs-lookup"><span data-stu-id="ff37d-112">Get the raw contents of a file or item attachment</span></span>
<span data-ttu-id="ff37d-113">Você pode acrescentar o segmento `/$value` de caminho para obter o conteúdo bruto de um arquivo ou anexo de item.</span><span class="sxs-lookup"><span data-stu-id="ff37d-113">You can append the path segment `/$value` to get the raw contents of a file or item attachment.</span></span> 

<span data-ttu-id="ff37d-114">Para um anexo de arquivo, o tipo de conteúdo se baseia em seu tipo de conteúdo original.</span><span class="sxs-lookup"><span data-stu-id="ff37d-114">For a file attachment, the content type is based on its original content type.</span></span> <span data-ttu-id="ff37d-115">Veja um [exemplo](#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message) abaixo.</span><span class="sxs-lookup"><span data-stu-id="ff37d-115">See an [example](#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message) below.</span></span>

<span data-ttu-id="ff37d-116">Para um anexo de item que é um [contato](../resources/contact.md), [evento](../resources/event.md)ou [mensagem](../resources/message.md), o conteúdo bruto retornado está no formato MIME.</span><span class="sxs-lookup"><span data-stu-id="ff37d-116">For an item attachment that is a [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md), the raw contents returned is in MIME format.</span></span>

| <span data-ttu-id="ff37d-117">Tipo de anexo de item</span><span class="sxs-lookup"><span data-stu-id="ff37d-117">Item attachment type</span></span>  | <span data-ttu-id="ff37d-118">Conteúdo bruto retornado</span><span class="sxs-lookup"><span data-stu-id="ff37d-118">Raw contents returned</span></span> |
|:-----------|:----------|
| <span data-ttu-id="ff37d-119">**contato**</span><span class="sxs-lookup"><span data-stu-id="ff37d-119">**contact**</span></span> | <span data-ttu-id="ff37d-120">[vCard](http://www.faqs.org/rfcs/rfc2426.html) Formato MIME.</span><span class="sxs-lookup"><span data-stu-id="ff37d-120">[vCard](http://www.faqs.org/rfcs/rfc2426.html) MIME format.</span></span> <span data-ttu-id="ff37d-121">Confira o [exemplo](#example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="ff37d-121">See [example](#example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message).</span></span> |
| <span data-ttu-id="ff37d-122">**evento**</span><span class="sxs-lookup"><span data-stu-id="ff37d-122">**event**</span></span> | <span data-ttu-id="ff37d-123">formato MIME iCal.</span><span class="sxs-lookup"><span data-stu-id="ff37d-123">iCal MIME format.</span></span> <span data-ttu-id="ff37d-124">Confira o [exemplo](#example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="ff37d-124">See [example](#example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message).</span></span> |
| <span data-ttu-id="ff37d-125">**message**</span><span class="sxs-lookup"><span data-stu-id="ff37d-125">**message**</span></span> | <span data-ttu-id="ff37d-126">Formato MIME.</span><span class="sxs-lookup"><span data-stu-id="ff37d-126">MIME format.</span></span> <span data-ttu-id="ff37d-127">Confira o [exemplo](#example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="ff37d-127">See [example](#example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message).</span></span> |

<span data-ttu-id="ff37d-128">Tentar obter um anexo `$value` de referência retorna http 405.</span><span class="sxs-lookup"><span data-stu-id="ff37d-128">Attempting to get the `$value` of a reference attachment returns HTTP 405.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff37d-129">Permissões</span><span class="sxs-lookup"><span data-stu-id="ff37d-129">Permissions</span></span>

<span data-ttu-id="ff37d-p106">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff37d-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="ff37d-132">Se estiver acessando anexos em mensagens: mail. Read</span><span class="sxs-lookup"><span data-stu-id="ff37d-132">If accessing attachments in messages: Mail.Read</span></span>
* <span data-ttu-id="ff37d-133">Se estiver acessando anexos em eventos: Calendars. Read</span><span class="sxs-lookup"><span data-stu-id="ff37d-133">If accessing attachments in events: Calendars.Read</span></span>
* <span data-ttu-id="ff37d-134">Se estiver acessando anexos em tarefas do Outlook: tarefas. leitura</span><span class="sxs-lookup"><span data-stu-id="ff37d-134">If accessing attachments in Outlook tasks: Tasks.Read</span></span>
* <span data-ttu-id="ff37d-135">Se estiver acessando anexos em Postagens de Grupo: Group. Read. All</span><span class="sxs-lookup"><span data-stu-id="ff37d-135">If accessing attachments in group posts: Group.Read.All</span></span>

<!--
* If accessing attachments in group events or posts: Group.Read.All
-->

## <a name="http-request"></a><span data-ttu-id="ff37d-136">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff37d-136">HTTP request</span></span>

<span data-ttu-id="ff37d-137">Esta seção mostra a sintaxe de solicitação HTTP GET para cada uma das entidades ([evento](../resources/event.md), [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postagem](../resources/post.md)) que dão suporte a anexos:</span><span class="sxs-lookup"><span data-stu-id="ff37d-137">This section shows the HTTP GET request syntax for each of the entities ([event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md)) that support attachments:</span></span>

- <span data-ttu-id="ff37d-138">Para obter as propriedades e as relações de um anexo, especifique a ID do anexo a ser \*\*\*\* indexada na coleção Attachments, anexada ao [evento](../resources/event.md)especificado, à [mensagem](../resources/message.md), à [tarefa do Outlook](../resources/outlooktask.md)ou à instância de [post](../resources/post.md) .</span><span class="sxs-lookup"><span data-stu-id="ff37d-138">To get the properties and relationships of an attachment, specify the attachment ID to index into the **attachments** collection, attached to the specified [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) instance.</span></span>
- <span data-ttu-id="ff37d-139">Se o anexo for um arquivo ou item do Outlook (contato, evento ou mensagem), você poderá obter o conteúdo bruto do anexo acrescentando o segmento `/$value` de caminho à URL de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff37d-139">If the attachment is a file or Outlook item (contact, event, or message), you can further get the raw contents of the attachment by appending the path segment `/$value` to the request URL.</span></span>

<span data-ttu-id="ff37d-140">Um anexo de um [evento](../resources/event.md):</span><span class="sxs-lookup"><span data-stu-id="ff37d-140">An attachment of an [event](../resources/event.md):</span></span>

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

<span data-ttu-id="ff37d-141">Um anexo de uma [mensagem](../resources/message.md) na caixa de correio de um usuário:</span><span class="sxs-lookup"><span data-stu-id="ff37d-141">An attachment of a [message](../resources/message.md) in a user's mailbox:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
GET /me/messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}/$value
```

<span data-ttu-id="ff37d-142">Um anexo de uma [mensagem](../resources/message.md) contida em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário:</span><span class="sxs-lookup"><span data-stu-id="ff37d-142">An attachment of a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}/$value
```

<span data-ttu-id="ff37d-143">Um anexo de uma [mensagem](../resources/message.md) contida em uma pasta filho de um [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário:</span><span class="sxs-lookup"><span data-stu-id="ff37d-143">An attachment of a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}/$value
```

<span data-ttu-id="ff37d-144">O exemplo anterior mostra um nível de aninhamento, mas uma mensagem pode ser localizada em um filho de um filho e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="ff37d-144">The preceding example shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>

<span data-ttu-id="ff37d-145">Um anexo de uma [tarefa do Outlook](../resources/outlooktask.md):</span><span class="sxs-lookup"><span data-stu-id="ff37d-145">An attachment of an [Outlook task](../resources/outlooktask.md):</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}/attachments/{id}
GET /users/{id}/outlook/tasks/{id}/attachments/{id}
GET /me/outlook/tasks/{id}/attachments/{id}/$value
GET /users/{id}/outlook/tasks/{id}/attachments/{id}/$value
```

<span data-ttu-id="ff37d-146">Um anexo de uma [postagem](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversa](../resources/conversation.md) de um grupo:</span><span class="sxs-lookup"><span data-stu-id="ff37d-146">An attachment of a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff37d-147">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ff37d-147">Optional query parameters</span></span>

<span data-ttu-id="ff37d-148">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ff37d-148">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff37d-149">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff37d-149">Request headers</span></span>

| <span data-ttu-id="ff37d-150">Nome</span><span class="sxs-lookup"><span data-stu-id="ff37d-150">Name</span></span>       | <span data-ttu-id="ff37d-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff37d-151">Type</span></span> | <span data-ttu-id="ff37d-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff37d-152">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ff37d-153">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff37d-153">Authorization</span></span>  | <span data-ttu-id="ff37d-154">string</span><span class="sxs-lookup"><span data-stu-id="ff37d-154">string</span></span>  | <span data-ttu-id="ff37d-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff37d-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff37d-157">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff37d-157">Request body</span></span>

<span data-ttu-id="ff37d-158">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ff37d-158">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff37d-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff37d-159">Response</span></span>

<span data-ttu-id="ff37d-160">Se tiver êxito, o método GET retornará `200 OK` um código de resposta.</span><span class="sxs-lookup"><span data-stu-id="ff37d-160">If successful, the GET method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="ff37d-161">Se você estiver obtendo as propriedades e as relações de um anexo, o corpo da resposta incluirá um objeto [Attachment](../resources/attachment.md) .</span><span class="sxs-lookup"><span data-stu-id="ff37d-161">If you're getting the properties and relationships of an attachment, the response body includes an [attachment](../resources/attachment.md) object.</span></span>

<span data-ttu-id="ff37d-162">Se você estiver obtendo o conteúdo bruto de um arquivo ou anexo de item, o corpo da resposta incluirá o valor bruto do anexo.</span><span class="sxs-lookup"><span data-stu-id="ff37d-162">If you're getting the raw contents of a file or item attachment, the response body includes the raw value of the attachment.</span></span>

## <a name="examples"></a><span data-ttu-id="ff37d-163">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ff37d-163">Examples</span></span>

### <a name="example-1-get-the-properties-of-a-file-attachment"></a><span data-ttu-id="ff37d-164">Exemplo 1: obter as propriedades de um anexo de arquivo</span><span class="sxs-lookup"><span data-stu-id="ff37d-164">Example 1: Get the properties of a file attachment</span></span>

#### <a name="request"></a><span data-ttu-id="ff37d-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff37d-165">Request</span></span>

<span data-ttu-id="ff37d-166">Aqui está um exemplo da solicitação para obter as propriedades de um anexo de arquivo em uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="ff37d-166">Here is an example of the request to get the properties of a file attachment on a message.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ff37d-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff37d-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_file_attachment",
  "sampleKeys": ["AAMkAGUzY5QKjAAA=","AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ff37d-168">C#</span><span class="sxs-lookup"><span data-stu-id="ff37d-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-file-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ff37d-169">Javascript</span><span class="sxs-lookup"><span data-stu-id="ff37d-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-file-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ff37d-170">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ff37d-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-file-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ff37d-171">Java</span><span class="sxs-lookup"><span data-stu-id="ff37d-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-file-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ff37d-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff37d-172">Response</span></span>

<span data-ttu-id="ff37d-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff37d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_file_attachment",
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
    "contentBytes": "base64,UEsDBBQABgAIAAAAIQ4AAAAA"
}
```

### <a name="example-2-get-the-properties-of-an-item-attachment"></a><span data-ttu-id="ff37d-176">Exemplo 2: obter as propriedades de um anexo de item</span><span class="sxs-lookup"><span data-stu-id="ff37d-176">Example 2: Get the properties of an item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="ff37d-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff37d-177">Request</span></span>

<span data-ttu-id="ff37d-178">O primeiro exemplo mostra como obter um anexo de item em uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="ff37d-178">The first example shows how to get an item attachment on a message.</span></span> <span data-ttu-id="ff37d-179">As propriedades do item de **anexo** são retornadas.</span><span class="sxs-lookup"><span data-stu-id="ff37d-179">The properties of the **itemAttachment** are returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ff37d-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff37d-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_item_attachment",
  "sampleKeys": ["AAMkADA1M-zAAA=","AAMkADA1M-CJKtzmnlcqVgqI="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ff37d-181">C#</span><span class="sxs-lookup"><span data-stu-id="ff37d-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ff37d-182">Javascript</span><span class="sxs-lookup"><span data-stu-id="ff37d-182">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ff37d-183">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ff37d-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ff37d-184">Java</span><span class="sxs-lookup"><span data-stu-id="ff37d-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ff37d-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff37d-185">Response</span></span>
<span data-ttu-id="ff37d-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff37d-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message"></a><span data-ttu-id="ff37d-189">Exemplo 3: expandir e obter as propriedades do item anexado a uma mensagem</span><span class="sxs-lookup"><span data-stu-id="ff37d-189">Example 3: Expand and get the properties of the item attached to a message</span></span>
#### <a name="request"></a><span data-ttu-id="ff37d-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff37d-190">Request</span></span>

<span data-ttu-id="ff37d-191">O exemplo a seguir mostra como usar `$expand` o para obter as propriedades do item (evento, mensagem, tarefa do Outlook ou postagem) anexado à mensagem.</span><span class="sxs-lookup"><span data-stu-id="ff37d-191">The next example shows how to use `$expand` to get the properties of the item (event, message, Outlook task, or post) that is attached to the message.</span></span> <span data-ttu-id="ff37d-192">Neste exemplo, esse item é uma mensagem; as propriedades dessa mensagem anexada também são retornadas.</span><span class="sxs-lookup"><span data-stu-id="ff37d-192">In this example, that item is a message; the properties of that attached message are also returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ff37d-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff37d-193">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_and_expand_item_attachment",
  "sampleKeys": ["AAMkADA1M-zAAA=","AAMkADA1M-CJKtzmnlcqVgqI="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')/?$expand=microsoft.graph.itemattachment/item
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ff37d-194">C#</span><span class="sxs-lookup"><span data-stu-id="ff37d-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-and-expand-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ff37d-195">Javascript</span><span class="sxs-lookup"><span data-stu-id="ff37d-195">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-and-expand-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ff37d-196">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ff37d-196">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-and-expand-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ff37d-197">Java</span><span class="sxs-lookup"><span data-stu-id="ff37d-197">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-and-expand-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ff37d-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff37d-198">Response</span></span>
<span data-ttu-id="ff37d-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff37d-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    ],
    "flag":{
      "flagStatus":"notFlagged"
    }
  }
}
```

### <a name="example-4-get-the-properties-of-a-reference-attachment"></a><span data-ttu-id="ff37d-202">Exemplo 4: obter as propriedades de um anexo de referência</span><span class="sxs-lookup"><span data-stu-id="ff37d-202">Example 4: Get the properties of a reference attachment</span></span>

#### <a name="request"></a><span data-ttu-id="ff37d-203">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff37d-203">Request</span></span>

<span data-ttu-id="ff37d-204">Aqui está um exemplo da solicitação para obter um anexo de referência em um evento.</span><span class="sxs-lookup"><span data-stu-id="ff37d-204">Here is an example of the request to get a reference attachment on an event.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ff37d-205">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff37d-205">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment",
  "sampleKeys": ["AAMkAGE1M88AADUv0uAAAG=","AAMkAGE1Mg72tgf7hJp0PICVGCc0g="]
}-->

```http
GET https://graph.microsoft.com/beta/me/events/AAMkAGE1M88AADUv0uAAAG=/attachments/AAMkAGE1Mg72tgf7hJp0PICVGCc0g=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ff37d-206">C#</span><span class="sxs-lookup"><span data-stu-id="ff37d-206">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reference-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ff37d-207">Javascript</span><span class="sxs-lookup"><span data-stu-id="ff37d-207">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reference-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ff37d-208">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ff37d-208">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reference-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ff37d-209">Java</span><span class="sxs-lookup"><span data-stu-id="ff37d-209">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-reference-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ff37d-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff37d-210">Response</span></span>
<span data-ttu-id="ff37d-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff37d-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


### <a name="example-5-get-the-raw-contents-of-a-file-attachment-on-a-message"></a><span data-ttu-id="ff37d-214">Exemplo 5: obter o conteúdo bruto de um anexo de arquivo em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="ff37d-214">Example 5: Get the raw contents of a file attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="ff37d-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff37d-215">Request</span></span>

<span data-ttu-id="ff37d-216">Aqui está um exemplo da solicitação para obter o conteúdo bruto de um arquivo do Word que tenha sido anexado a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="ff37d-216">Here is an example of the request to get the raw contents of a Word file that has been attached to a message.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_value_file_attachment",
  "sampleKeys": ["AAMkAGUzY5QKjAAA=","AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=/$value
```

#### <a name="response"></a><span data-ttu-id="ff37d-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff37d-217">Response</span></span>
<span data-ttu-id="ff37d-218">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff37d-218">Here is an example of the response.</span></span> <span data-ttu-id="ff37d-219">O corpo da resposta real inclui os bytes brutos do anexo de arquivo, abreviados aqui por brevidade.</span><span class="sxs-lookup"><span data-stu-id="ff37d-219">The actual response body includes the raw bytes of the file attachment, which are abbreviated here for brevity.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_value_file_attachment",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK

{Raw bytes of the file}
```


### <a name="example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message"></a><span data-ttu-id="ff37d-220">Exemplo 6: obter o conteúdo MIME bruto de um anexo de contato em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="ff37d-220">Example 6: Get the MIME raw contents of a contact attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="ff37d-221">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff37d-221">Request</span></span>

<span data-ttu-id="ff37d-222">Aqui está um exemplo da solicitação para obter o conteúdo bruto de um item de contato que tenha sido anexado a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="ff37d-222">Here is an example of the request to get the raw contents of a contact item that has been attached to a message.</span></span> 
<!-- {
  "blockType": "ignored",
  "name": "get_value_contact_attachment",
  "sampleKeys": ["AAMkADI5MAAGjk2PxAAA=","AAMkADI5MAAGjk2PxAAABEgAQACEJqrbJZBNIlr3pGFvd9K8="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkADI5MAAGjk2PxAAA=/attachments/AAMkADI5MAAGjk2PxAAABEgAQACEJqrbJZBNIlr3pGFvd9K8=/$value
```

#### <a name="response"></a><span data-ttu-id="ff37d-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff37d-223">Response</span></span>
<span data-ttu-id="ff37d-224">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff37d-224">Here is an example of the response.</span></span> 

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


### <a name="example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message"></a><span data-ttu-id="ff37d-225">Exemplo 7: obter o conteúdo bruto de MIME de um anexo de evento em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="ff37d-225">Example 7: Get the MIME raw contents of an event attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="ff37d-226">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff37d-226">Request</span></span>

<span data-ttu-id="ff37d-227">Aqui está um exemplo da solicitação para obter o conteúdo bruto de um evento que tenha sido anexado a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="ff37d-227">Here is an example of the request to get the raw contents of an event that has been attached to a message.</span></span> 
<!-- {
  "blockType": "ignored",
  "name": "get_value_event_attachment",
  "sampleKeys": ["AAMkADVIOAAA=","AAMkADVIOAAABEgAQACvkutl6c4FMifPyS6NvXsM="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkADVIOAAA=/attachments/AAMkADVIOAAABEgAQACvkutl6c4FMifPyS6NvXsM=/$value
```

#### <a name="response"></a><span data-ttu-id="ff37d-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff37d-228">Response</span></span>
<span data-ttu-id="ff37d-229">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff37d-229">Here is an example of the response.</span></span> 

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


### <a name="example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message"></a><span data-ttu-id="ff37d-230">Exemplo 8: obter o conteúdo MIME bruto de um anexo de item de convite de reunião em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="ff37d-230">Example 8: Get the MIME raw contents of a meeting invitation item attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="ff37d-231">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff37d-231">Request</span></span>

<span data-ttu-id="ff37d-232">Aqui está um exemplo da solicitação para obter o conteúdo bruto de um convite de reunião (do tipo [eventMessage](../resources/eventmessage.md) ) que foi anexado a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="ff37d-232">Here is an example of the request to get the raw contents of a meeting invitation (of the [eventMessage](../resources/eventmessage.md) type) that has been attached to a message.</span></span> <span data-ttu-id="ff37d-233">A entidade **eventMessage** é baseada no tipo de **mensagem** .</span><span class="sxs-lookup"><span data-stu-id="ff37d-233">The **eventMessage** entity is based on the **message** type.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_value_message_attachment",
  "sampleKeys": ["AAMkAGUzY5QKiAAA=","AAMkAGUzY5QKiAAABEgAQAK8ktgiIO19OqkvUZAqLmyQ="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKiAAA=/attachments/AAMkAGUzY5QKiAAABEgAQAK8ktgiIO19OqkvUZAqLmyQ=/$value
```

#### <a name="response"></a><span data-ttu-id="ff37d-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff37d-234">Response</span></span>
<span data-ttu-id="ff37d-235">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff37d-235">Here is an example of the response.</span></span> 

<span data-ttu-id="ff37d-236">O corpo da resposta inclui o anexo **eventMessage** no formato MIME.</span><span class="sxs-lookup"><span data-stu-id="ff37d-236">The response body includes the **eventMessage** attachment in MIME format.</span></span> <span data-ttu-id="ff37d-237">O corpo do **eventMessage** é truncado por brevidade.</span><span class="sxs-lookup"><span data-stu-id="ff37d-237">The body of the  **eventMessage** is truncated for brevity.</span></span> <span data-ttu-id="ff37d-238">O corpo completo da mensagem é retornado de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff37d-238">The full message body is returned from an actual call.</span></span>

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
