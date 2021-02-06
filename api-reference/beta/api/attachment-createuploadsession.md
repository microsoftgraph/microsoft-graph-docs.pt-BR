---
title: 'attachment: createUploadSession'
description: Crie uma sessão de upload para carregar iterativamente intervalos de um arquivo para anexar o arquivo à mensagem especificada.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a6856799c8532f3a0bf428dc7d417f9f29e921a9
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128929"
---
# <a name="attachment-createuploadsession"></a><span data-ttu-id="6bd16-103">attachment: createUploadSession</span><span class="sxs-lookup"><span data-stu-id="6bd16-103">attachment: createUploadSession</span></span>

<span data-ttu-id="6bd16-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bd16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6bd16-105">Crie uma sessão de upload que permita que um aplicativo carregue iterativamente intervalos de um arquivo, para anexar o arquivo a um item do Outlook.</span><span class="sxs-lookup"><span data-stu-id="6bd16-105">Create an upload session that allows an app to iteratively upload ranges of a file, so as to attach the file to an Outlook item.</span></span> <span data-ttu-id="6bd16-106">O item pode ser uma [mensagem ou](../resources/message.md) um [evento.](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="6bd16-106">The item can be a [message](../resources/message.md) or [event](../resources/event.md).</span></span>

<span data-ttu-id="6bd16-107">Use essa abordagem para anexar um arquivo se o tamanho do arquivo estiver entre 3 MB e 150 MB.</span><span class="sxs-lookup"><span data-stu-id="6bd16-107">Use this approach to attach a file if the file size is between 3 MB and 150 MB.</span></span> <span data-ttu-id="6bd16-108">Para anexar um arquivo menor que 3 MB, faça uma operação na propriedade de navegação de anexos do item do Outlook; veja como fazer isso para uma mensagem ou para `POST` [um evento.](event-post-attachments.md)  [](message-post-attachments.md)</span><span class="sxs-lookup"><span data-stu-id="6bd16-108">To attach a file that's smaller than 3 MB, do a `POST` operation on the **attachments** navigation property of the Outlook item; see how to do this [for a message](message-post-attachments.md) or [for an event](event-post-attachments.md).</span></span> 

<span data-ttu-id="6bd16-109">Como parte da resposta, essa ação retorna uma URL de carregamento que você pode usar em consultas `PUT` sequenciais subsequentes.</span><span class="sxs-lookup"><span data-stu-id="6bd16-109">As part of the response, this action returns an upload URL that you can use in subsequent sequential `PUT` queries.</span></span> <span data-ttu-id="6bd16-110">Os headers de solicitação `PUT` para cada operação permitem que você especifique o intervalo exato de bytes a serem carregados.</span><span class="sxs-lookup"><span data-stu-id="6bd16-110">Request headers for each `PUT` operation let you specify the exact range of bytes to be uploaded.</span></span> <span data-ttu-id="6bd16-111">Isso permite que a transferência seja retomada, caso a conexão de rede seja retirada durante o upload.</span><span class="sxs-lookup"><span data-stu-id="6bd16-111">This allows transfer to be resumed, in case the network connection is dropped during upload.</span></span> 

<span data-ttu-id="6bd16-112">Veja a seguir as etapas para anexar um arquivo a um item do Outlook usando uma sessão de upload:</span><span class="sxs-lookup"><span data-stu-id="6bd16-112">The following are the steps to attach a file to an Outlook item using an upload session:</span></span>

1. <span data-ttu-id="6bd16-113">Crie uma sessão de upload.</span><span class="sxs-lookup"><span data-stu-id="6bd16-113">Create an upload session.</span></span>
2. <span data-ttu-id="6bd16-114">Dentro dessa sessão de carregamento, carregue iterativamente intervalos de bytes (até 4 MB a cada vez) até que todos os bytes do arquivo tenham sido carregados e o arquivo seja anexado ao item especificado.</span><span class="sxs-lookup"><span data-stu-id="6bd16-114">Within that upload session, iteratively upload ranges of bytes (up to 4 MB each time) until all the bytes of the file have been uploaded, and the file is attached to the specified item.</span></span>
3. <span data-ttu-id="6bd16-115">Salve a ID do anexo para acesso futuro.</span><span class="sxs-lookup"><span data-stu-id="6bd16-115">Save the ID for the attachment for future access.</span></span>
4. <span data-ttu-id="6bd16-116">Opcional: excluir a sessão de carregamento.</span><span class="sxs-lookup"><span data-stu-id="6bd16-116">Optional: Delete the upload session.</span></span>

<span data-ttu-id="6bd16-117">Veja [anexar arquivos grandes a mensagens ou eventos do Outlook](/graph/outlook-large-attachments) para ver um exemplo.</span><span class="sxs-lookup"><span data-stu-id="6bd16-117">See [attach large files to Outlook messages or events](/graph/outlook-large-attachments) for an example.</span></span>

> [!TIP]
> <span data-ttu-id="6bd16-118">O Exchange Online permite que os administradores personalizem o limite de tamanho de mensagens para caixas de correio do Microsoft 365, incluindo anexos de mensagens.</span><span class="sxs-lookup"><span data-stu-id="6bd16-118">Exchange Online lets administrators customize the message size limit for Microsoft 365 mailboxes,  including any message attachments.</span></span> <span data-ttu-id="6bd16-119">Por padrão, esse limite de tamanho de mensagem é de 35 MB.</span><span class="sxs-lookup"><span data-stu-id="6bd16-119">By default, this message size limit is 35 MB.</span></span> <span data-ttu-id="6bd16-120">Descubra como personalizar o [tamanho máximo da mensagem para](https://www.microsoft.com/microsoft-365/blog/2015/04/15/office-365-now-supports-larger-email-messages-up-to-150-mb) suportar anexos maiores do que o limite padrão para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="6bd16-120">Find out how to [customize the maximum message size](https://www.microsoft.com/microsoft-365/blog/2015/04/15/office-365-now-supports-larger-email-messages-up-to-150-mb) to support attachments larger than the default limit for your tenant.</span></span> 

> [!IMPORTANT] 
> <span data-ttu-id="6bd16-121">Esteja ciente de um [problema](/graph/known-issues#attaching-large-files-to-messages) conhecido se estiver anexando um arquivo grande a uma mensagem ou evento em uma caixa de correio compartilhada ou delegada.</span><span class="sxs-lookup"><span data-stu-id="6bd16-121">Be aware of a [known issue](/graph/known-issues#attaching-large-files-to-messages) if you're attaching a large file to a message or event in a shared or delegated mailbox.</span></span>


## <a name="permissions"></a><span data-ttu-id="6bd16-122">Permissões</span><span class="sxs-lookup"><span data-stu-id="6bd16-122">Permissions</span></span>

<span data-ttu-id="6bd16-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bd16-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6bd16-125">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6bd16-125">Permission type</span></span>                        | <span data-ttu-id="6bd16-126">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6bd16-126">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6bd16-127">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6bd16-127">Delegated (work or school account)</span></span>     | <span data-ttu-id="6bd16-128">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6bd16-128">Mail.ReadWrite</span></span> |
| <span data-ttu-id="6bd16-129">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6bd16-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6bd16-130">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6bd16-130">Mail.ReadWrite</span></span> |
| <span data-ttu-id="6bd16-131">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6bd16-131">Application</span></span>                            | <span data-ttu-id="6bd16-132">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6bd16-132">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6bd16-133">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6bd16-133">HTTP request</span></span>

<span data-ttu-id="6bd16-134">Para criar uma sessão de upload para anexar um arquivo a um **evento:**</span><span class="sxs-lookup"><span data-stu-id="6bd16-134">To create an upload session for attaching a file to an **event**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/attachments/createUploadSession
```

<span data-ttu-id="6bd16-135">Para criar uma sessão de upload para anexar um arquivo a uma **mensagem:**</span><span class="sxs-lookup"><span data-stu-id="6bd16-135">To create an upload session for attaching a file to a **message**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments/createUploadSession
```

## <a name="request-headers"></a><span data-ttu-id="6bd16-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6bd16-136">Request headers</span></span>

| <span data-ttu-id="6bd16-137">Nome</span><span class="sxs-lookup"><span data-stu-id="6bd16-137">Name</span></span>          | <span data-ttu-id="6bd16-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bd16-138">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6bd16-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="6bd16-139">Authorization</span></span> | <span data-ttu-id="6bd16-140">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="6bd16-140">Bearer {token}</span></span> |


## <a name="request-body"></a><span data-ttu-id="6bd16-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6bd16-141">Request body</span></span>

<span data-ttu-id="6bd16-142">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6bd16-142">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6bd16-143">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6bd16-143">Parameter</span></span>    | <span data-ttu-id="6bd16-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="6bd16-144">Type</span></span>        | <span data-ttu-id="6bd16-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bd16-145">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6bd16-146">AttachmentItem</span><span class="sxs-lookup"><span data-stu-id="6bd16-146">AttachmentItem</span></span>|[<span data-ttu-id="6bd16-147">attachmentItem</span><span class="sxs-lookup"><span data-stu-id="6bd16-147">attachmentItem</span></span>](../resources/attachmentitem.md)|<span data-ttu-id="6bd16-148">Representa atributos do item a ser carregado e anexado.</span><span class="sxs-lookup"><span data-stu-id="6bd16-148">Represents attributes of the item to be uploaded and attached.</span></span> <span data-ttu-id="6bd16-149">No mínimo, especifique o tipo de anexo ( `file` ), um nome e o tamanho do arquivo.</span><span class="sxs-lookup"><span data-stu-id="6bd16-149">At minimum, specify the attachment type (`file`), a name, and the size of the file.</span></span>|

## <a name="response"></a><span data-ttu-id="6bd16-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bd16-150">Response</span></span>

<span data-ttu-id="6bd16-151">Se bem-sucedido, este método retorna um código de resposta e um novo objeto `201 Created` [uploadSession](../resources/uploadsession.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6bd16-151">If successful, this method returns a `201 Created` response code and a new [uploadSession](../resources/uploadsession.md) object in the response body.</span></span>

><span data-ttu-id="6bd16-152">**Observação**:</span><span class="sxs-lookup"><span data-stu-id="6bd16-152">**Note**:</span></span> 
>
><span data-ttu-id="6bd16-153">A **propriedade uploadUrl** retornada como parte do objeto de resposta **uploadSession** é uma URL opaca para consultas subsequentes para carregar intervalos de `PUT` byte do arquivo.</span><span class="sxs-lookup"><span data-stu-id="6bd16-153">The **uploadUrl** property returned as part of the **uploadSession** response object is an opaque URL for subsequent `PUT` queries to upload byte ranges of the file.</span></span> <span data-ttu-id="6bd16-154">Ele contém o token de autorização apropriado para consultas `PUT` subsequentes que expiram **por expirationDateTime**.</span><span class="sxs-lookup"><span data-stu-id="6bd16-154">It contains the appropriate auth token for subsequent `PUT` queries that expire by **expirationDateTime**.</span></span> <span data-ttu-id="6bd16-155">Não personalize essa URL.</span><span class="sxs-lookup"><span data-stu-id="6bd16-155">Do not customize this URL.</span></span>
>
><span data-ttu-id="6bd16-156">A **propriedade nextExpectedRanges** especifica o próximo local de byte do arquivo a ser carregado, por exemplo, `"NextExpectedRanges":["2097152"]` .</span><span class="sxs-lookup"><span data-stu-id="6bd16-156">The **nextExpectedRanges** property specifies the next file byte location to upload from, for example, `"NextExpectedRanges":["2097152"]`.</span></span> <span data-ttu-id="6bd16-157">Você deve carregar os bytes em um arquivo na ordem.</span><span class="sxs-lookup"><span data-stu-id="6bd16-157">You must upload bytes in a file in order.</span></span>

<!-- The **nextExpectedRanges** property specifies one or more ranges of bytes that the server is still missing for the file. These ranges are zero-indexed and of the format `{start}-{end}`, unless if the server misses the remainder of the bytes from the start of that range, in which case the format is simply `{start}`.  -->


## <a name="examples"></a><span data-ttu-id="6bd16-158">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6bd16-158">Examples</span></span>

<span data-ttu-id="6bd16-159">O exemplo a seguir mostra como criar uma sessão de upload que você pode usar nas operações subsequentes de carregamento de arquivo para a mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="6bd16-159">The following example shows how to create an upload session that you can use in subsequent file upload operations to the specified message.</span></span>

### <a name="request"></a><span data-ttu-id="6bd16-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6bd16-160">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6bd16-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="6bd16-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "attachment_createuploadsession",
  "sampleKeys": ["AAMkADI5MAAIT3drCAAA="]
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADI5MAAIT3drCAAA=/attachments/createUploadSession
Content-type: application/json

{
  "AttachmentItem": {
    "attachmentType": "file",
    "name": "flower", 
    "size": 3483322
  }
}
```
# <a name="c"></a>[<span data-ttu-id="6bd16-162">C#</span><span class="sxs-lookup"><span data-stu-id="6bd16-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/attachment-createuploadsession-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6bd16-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6bd16-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/attachment-createuploadsession-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6bd16-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6bd16-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/attachment-createuploadsession-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6bd16-165">Java</span><span class="sxs-lookup"><span data-stu-id="6bd16-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/attachment-createuploadsession-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6bd16-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bd16-166">Response</span></span>

> <span data-ttu-id="6bd16-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6bd16-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "attachment_createuploadsession",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0uAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI",
    "expirationDateTime": "2019-09-25T01:09:30.7671707Z",
    "nextExpectedRanges": [
        "0-"
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attachment: createUploadSession",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


