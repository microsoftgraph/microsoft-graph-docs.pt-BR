---
title: Anexar arquivos grandes a mensagens ou eventos do Outlook
description: Dependendo do tamanho do arquivo, você pode escolher uma das duas maneiras de anexar um arquivo a uma mensagem ou evento.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 40bcc849c497c2d75b1fa16a11f6133309494303
ms.sourcegitcommit: ff3fd4ead2b864ce6abb79915a0488d0562347f8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2020
ms.locfileid: "46524300"
---
# <a name="attach-large-files-to-outlook-messages-or-events"></a><span data-ttu-id="48865-103">Anexar arquivos grandes a mensagens ou eventos do Outlook</span><span class="sxs-lookup"><span data-stu-id="48865-103">Attach large files to Outlook messages or events</span></span>

<span data-ttu-id="48865-104">Usando a API do Microsoft Graph, é possível anexar arquivos de até 150 MB a uma [mensagem](/graph/api/resources/message?view=graph-rest-1.0) ou item de [evento](/graph/api/resources/event?view=graph-rest-1.0) do Outlook.</span><span class="sxs-lookup"><span data-stu-id="48865-104">Using the Microsoft Graph API, you can attach files up to 150 MB to an Outlook [message](/graph/api/resources/message?view=graph-rest-1.0) or [event](/graph/api/resources/event?view=graph-rest-1.0) item.</span></span> <span data-ttu-id="48865-105">Dependendo do tamanho do arquivo, escolha uma das duas maneiras de anexar o arquivo:</span><span class="sxs-lookup"><span data-stu-id="48865-105">Depending on the file size, choose one of two ways to attach the file:</span></span>
- <span data-ttu-id="48865-106">Se o tamanho do arquivo for menor que 3 MB, faça uma única POSTAGEM na propriedade de navegação dos **anexos** do item do Outlook; veja como fazer isso para uma [mensagem](/graph/api/message-post-attachments?view=graph-rest-1.0) ou [evento](/graph/api/event-post-attachments?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="48865-106">If the file size is under 3 MB, do a single POST on the **attachments** navigation property of the Outlook item; see how to do this [for a message](/graph/api/message-post-attachments?view=graph-rest-1.0) or [for an event](/graph/api/event-post-attachments?view=graph-rest-1.0).</span></span> <span data-ttu-id="48865-107">A resposta `POST` bem-sucedida inclui a ID de anexo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="48865-107">The successful `POST` response includes the ID of the file attachment.</span></span>
- <span data-ttu-id="48865-108">Se o tamanho do arquivo estiver entre 3 MB e 150 MB, crie uma sessão de carregamento e use o `PUT` iteradamente para carregar intervalos de bytes do arquivo até que você carregue todo o arquivo.</span><span class="sxs-lookup"><span data-stu-id="48865-108">If the file size is between 3MB and 150MB, create an upload session, and iteratively use `PUT` to upload ranges of bytes of the file until you have uploaded the entire file.</span></span> <span data-ttu-id="48865-109">Um cabeçalho na resposta `PUT` finalizada com êxito inclui uma URL com a ID do anexo.</span><span class="sxs-lookup"><span data-stu-id="48865-109">A header in the final successful `PUT` response includes a URL with the attachment ID.</span></span>

<span data-ttu-id="48865-110">Para anexar vários arquivos a uma mensagem, escolha a abordagem de cada arquivo com base em seu tamanho e anexe-os individualmente.</span><span class="sxs-lookup"><span data-stu-id="48865-110">To attach multiple files to a message, choose the approach for each file based on its file size and attach the files individually.</span></span>

<span data-ttu-id="48865-111">Este artigo ilustra a segunda abordagem passo a passo, criando e usando uma sessão de carregamento para adicionar um anexo de arquivo grande (de tamanho superior a 3MB) a um item do Outlook.</span><span class="sxs-lookup"><span data-stu-id="48865-111">This article illustrates the second approach step by step, creating and using an upload session to add a large file attachment (of size over 3MB) to an Outlook item.</span></span> <span data-ttu-id="48865-112">Cada etapa mostra o código correspondente de uma mensagem e de um evento.</span><span class="sxs-lookup"><span data-stu-id="48865-112">Each step shows the corresponding code for a message and for an event.</span></span> <span data-ttu-id="48865-113">Ao carregar o arquivo inteiro com êxito, o artigo exibe a obtenção de um cabeçalho de resposta contendo uma ID para o anexo do arquivo e, em seguida, o uso dessa ID de anexo para obter o conteúdo bruto do anexo ou metadados do anexo.</span><span class="sxs-lookup"><span data-stu-id="48865-113">Upon successfully uploading the entire file, the article shows getting a response header that contains an ID for the file attachment, and then using that attachment ID to get the raw attachment content or attachment metadata.</span></span> 

> [!IMPORTANT] 
> <span data-ttu-id="48865-114">Esteja atento a um [problema conhecido](known-issues.md#attaching-large-files-to-messages)se você estiver anexando arquivos de grande tamanho a uma mensagem ou evento em uma caixa de correio delegada ou compartilhada.</span><span class="sxs-lookup"><span data-stu-id="48865-114">Be aware of a [known issue](known-issues.md#attaching-large-files-to-messages) if you're attaching large files to a message or event in a shared or delegated mailbox.</span></span>

## <a name="step-1-create-an-upload-session"></a><span data-ttu-id="48865-115">Etapa 1: criar uma sessão de carregamento</span><span class="sxs-lookup"><span data-stu-id="48865-115">Step 1: Create an upload session</span></span>

<span data-ttu-id="48865-116">[Criar uma sessão de carregamento](/graph/api/attachment-createuploadsession?view=graph-rest-1.0) para anexar um arquivo a uma mensagem ou evento.</span><span class="sxs-lookup"><span data-stu-id="48865-116">[Create an upload session](/graph/api/attachment-createuploadsession?view=graph-rest-1.0) to attach a file to a message or event.</span></span> <span data-ttu-id="48865-117">Especifique o arquivo no parâmetro de entrada **AttachmentItem**.</span><span class="sxs-lookup"><span data-stu-id="48865-117">Specify the file in the input parameter **AttachmentItem**.</span></span>

<span data-ttu-id="48865-118">Uma operação bem-sucedida retorna `HTTP 201 Created` e uma nova instância[uploadSession](/graph/api/resources/uploadsession?view=graph-rest-1.0), que contém uma URL opaca que você pode usar em operações `PUT` subseqüentes para carregar partes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="48865-118">A successful operation returns `HTTP 201 Created` and a new [uploadSession](/graph/api/resources/uploadsession?view=graph-rest-1.0) instance, which contains an opaque URL that you can use in subsequent `PUT` operations to upload portions of the file.</span></span> <span data-ttu-id="48865-119">A **uploadSession** fornece um local de armazenamento temporário onde os bytes do arquivo são salvos até que você tenha carregado o arquivo completo.</span><span class="sxs-lookup"><span data-stu-id="48865-119">The **uploadSession** provides a temporary storage location where the bytes of the file are saved until you have uploaded the complete file.</span></span>

<span data-ttu-id="48865-120">Certifique-se de pedir permissão de `Mail.ReadWrite` para criar a **uploadSession** para uma mensagem e `Calendars.ReadWrite` para um evento.</span><span class="sxs-lookup"><span data-stu-id="48865-120">Make sure to request `Mail.ReadWrite` permission to create the **uploadSession** for a message, and `Calendars.ReadWrite` for an event.</span></span> <span data-ttu-id="48865-121">A URL opaca, retornada na propriedade **uploadUrl** do novo **uploadSession** é pré-autenticada e contém o token de autorização apropriado para consultas `PUT` subsequentes no domínio `https://outlook.office.com`.</span><span class="sxs-lookup"><span data-stu-id="48865-121">The opaque URL, returned in the **uploadUrl** property of the new **uploadSession**, is pre-authenticated and contains the appropriate authorization token for subsequent `PUT` queries in the `https://outlook.office.com` domain.</span></span> <span data-ttu-id="48865-122">Esse token expira por **expirationDateTime**.</span><span class="sxs-lookup"><span data-stu-id="48865-122">That token expires by **expirationDateTime**.</span></span> <span data-ttu-id="48865-123">Não Personalize essa URL para as operações `PUT`.</span><span class="sxs-lookup"><span data-stu-id="48865-123">Do not customize this URL for the `PUT` operations.</span></span>

<span data-ttu-id="48865-124">O objeto**uploadSession** na resposta também inclui a propriedade **nextExpectedRanges**, que indica que o local inicial de carregamento deve ser byte 0.</span><span class="sxs-lookup"><span data-stu-id="48865-124">The **uploadSession** object in the response also includes the **nextExpectedRanges** property, which indicates the initial upload starting location should be byte 0.</span></span>

### <a name="example-create-an-upload-session-for-a-message"></a><span data-ttu-id="48865-125">Exemplo: criar uma sessão de carregamento para uma mensagem</span><span class="sxs-lookup"><span data-stu-id="48865-125">Example: create an upload session for a message</span></span>

#### <a name="request"></a><span data-ttu-id="48865-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48865-126">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="48865-127">HTTP</span><span class="sxs-lookup"><span data-stu-id="48865-127">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "walkthrough_create_uploadsession_message",
  "sampleKeys": ["AAMkADI5MAAIT3drCAAA="]
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADI5MAAIT3drCAAA=/attachments/createUploadSession
Content-type: application/json

{
  "AttachmentItem": {
    "attachmentType": "file",
    "name": "flower",
    "size": 3483322
  }
}
```
# <a name="c"></a>[<span data-ttu-id="48865-128">C#</span><span class="sxs-lookup"><span data-stu-id="48865-128">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/walkthrough-create-uploadsession-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="48865-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48865-129">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/walkthrough-create-uploadsession-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="48865-130">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48865-130">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/walkthrough-create-uploadsession-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="48865-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="48865-131">Response</span></span>
<span data-ttu-id="48865-132">O exemplo de resposta a seguir mostra o recurso **uploadSession** retornado para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="48865-132">The following example response shows the **uploadSession** resource returned for the message.</span></span>

<!-- {
  "blockType": "response",
  "name": "walkthrough_create_uploadsession_message",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://outlook.office.com/api/v2.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI",
    "expirationDateTime": "2019-09-25T01:09:30.7671707Z",
    "nextExpectedRanges": [
        "0-"
    ]
}
```

### <a name="example-create-an-upload-session-for-an-event"></a><span data-ttu-id="48865-133">Exemplo: criar uma sessão de carregamento para uma evento</span><span class="sxs-lookup"><span data-stu-id="48865-133">Example: create an upload session for an event</span></span>
#### <a name="request"></a><span data-ttu-id="48865-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48865-134">Request</span></span> 


# <a name="http"></a>[<span data-ttu-id="48865-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="48865-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "walkthrough_create_uploadsession_event",
  "sampleKeys": ["AAMkADU5CCmSAAA="]
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/AAMkADU5CCmSAAA=/attachments/createUploadSession
Content-type: application/json

{
  "AttachmentItem": {
    "attachmentType": "file",
    "name": "flower",
    "size": 3483322
  }
}
```
# <a name="c"></a>[<span data-ttu-id="48865-136">C#</span><span class="sxs-lookup"><span data-stu-id="48865-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/walkthrough-create-uploadsession-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="48865-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48865-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/walkthrough-create-uploadsession-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="48865-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48865-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/walkthrough-create-uploadsession-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="48865-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="48865-139">Response</span></span>
<span data-ttu-id="48865-140">O exemplo de resposta a seguir mostra o recurso **uploadSession** retornado para o evento.</span><span class="sxs-lookup"><span data-stu-id="48865-140">The following example response shows the **uploadSession** resource returned for the event.</span></span>

<!-- {
  "blockType": "response",
  "name": "walkthrough_create_uploadsession_event",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://outlook.office.com/api/v2.0/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/AttachmentSessions('AAMkADU5RpAACJlCs8AAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIBtw",
    "expirationDateTime": "2020-02-22T02:46:56.7410786Z",
    "nextExpectedRanges": [
        "0-"
    ]
}

```


## <a name="step-2-use-the-upload-session-to-upload-a-range-of-bytes-of-the-file"></a><span data-ttu-id="48865-141">Etapa 2: usar a sessão de carregamento para carregar um intervalo de bytes do arquivo</span><span class="sxs-lookup"><span data-stu-id="48865-141">Step 2: Use the upload session to upload a range of bytes of the file</span></span>

<span data-ttu-id="48865-142">Para carregar o arquivo, ou uma parte do arquivo, faça uma solicitação `PUT` à URL retornada na etapa 1 na propriedade **uploadUrl** do recurso **uploadSession**.</span><span class="sxs-lookup"><span data-stu-id="48865-142">To upload the file, or a portion of the file, make a `PUT` request to the URL returned in step 1 in the **uploadUrl** property of the **uploadSession** resource.</span></span> <span data-ttu-id="48865-143">Você pode carregar todo o arquivo ou dividi-lo em vários intervalos de bytes.</span><span class="sxs-lookup"><span data-stu-id="48865-143">You can upload the entire file, or split the file into multiple byte ranges.</span></span> <span data-ttu-id="48865-144">Para melhorar o desempenho, mantenha cada intervalo de bytes com menos de 4 MB.</span><span class="sxs-lookup"><span data-stu-id="48865-144">For better performance, keep each byte range less than 4 MB.</span></span>

<span data-ttu-id="48865-145">Especifique os cabeçalhos e corpo da solicitação conforme é descrito abaixo.</span><span class="sxs-lookup"><span data-stu-id="48865-145">Specify request headers and request body as described below.</span></span>

### <a name="request-headers"></a><span data-ttu-id="48865-146">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48865-146">Request headers</span></span>

| <span data-ttu-id="48865-147">Nome</span><span class="sxs-lookup"><span data-stu-id="48865-147">Name</span></span>       | <span data-ttu-id="48865-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="48865-148">Type</span></span> | <span data-ttu-id="48865-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="48865-149">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="48865-150">Content-Length</span><span class="sxs-lookup"><span data-stu-id="48865-150">Content-Length</span></span> | <span data-ttu-id="48865-151">Int32</span><span class="sxs-lookup"><span data-stu-id="48865-151">Int32</span></span> | <span data-ttu-id="48865-152">O número de bytes sendo carregados nesta operação.</span><span class="sxs-lookup"><span data-stu-id="48865-152">The number of bytes being uploaded in this operation.</span></span> <span data-ttu-id="48865-153">Para melhorar o desempenho, mantenha o limite superior do número de bytes para cada operação `PUT` em 4 MB.</span><span class="sxs-lookup"><span data-stu-id="48865-153">For better performance, keep the upper limit of the number of bytes for each `PUT` operation to 4 MB.</span></span> <span data-ttu-id="48865-154">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48865-154">Required.</span></span> |
| <span data-ttu-id="48865-155">Intervalo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="48865-155">Content-Range</span></span> | <span data-ttu-id="48865-156">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="48865-156">String</span></span> | <span data-ttu-id="48865-157">O intervalo de bytes baseado em 0 do arquivo que está sendo carregado nesta operação, expresso no formato `bytes {start}-{end}/{total}`.</span><span class="sxs-lookup"><span data-stu-id="48865-157">The 0-based byte range of the file being uploaded in this operation, expressed in the format `bytes {start}-{end}/{total}`.</span></span> <span data-ttu-id="48865-158">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48865-158">Required.</span></span> |
| <span data-ttu-id="48865-159">Content-Type</span><span class="sxs-lookup"><span data-stu-id="48865-159">Content-Type</span></span> | <span data-ttu-id="48865-160">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="48865-160">String</span></span>  | <span data-ttu-id="48865-161">O tipo MIME.</span><span class="sxs-lookup"><span data-stu-id="48865-161">The MIME type.</span></span> <span data-ttu-id="48865-162">Especifique`application/octet-stream`.</span><span class="sxs-lookup"><span data-stu-id="48865-162">Specify `application/octet-stream`.</span></span> <span data-ttu-id="48865-163">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48865-163">Required.</span></span> |

<span data-ttu-id="48865-164">Não especifique um cabeçalho da solicitação`Authorization`.</span><span class="sxs-lookup"><span data-stu-id="48865-164">Do not specify an `Authorization` request header.</span></span> <span data-ttu-id="48865-165">A consulta `PUT` usa uma URL pré-existente da propriedade **uploadUrl**, que permite o acesso ao domínio `https://outlook.office.com`.</span><span class="sxs-lookup"><span data-stu-id="48865-165">The `PUT` query uses a pre-authenticated URL from the **uploadUrl** property, that allows access to the `https://outlook.office.com` domain.</span></span>

### <a name="request-body"></a><span data-ttu-id="48865-166">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48865-166">Request body</span></span>

<span data-ttu-id="48865-167">Especificar os bytes reais do arquivo a ser anexado, que estão no intervalo de local especificado pelo cabeçalho da solicitação`Content-Range`.</span><span class="sxs-lookup"><span data-stu-id="48865-167">Specify the actual bytes of the file to be attached, that are in the location range specified by the `Content-Range` request header.</span></span>

### <a name="response"></a><span data-ttu-id="48865-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="48865-168">Response</span></span>
<span data-ttu-id="48865-169">Um carregamento bem-sucedido retorna `HTTP 200 OK` e um objeto **uploadSession**.</span><span class="sxs-lookup"><span data-stu-id="48865-169">A successful upload returns `HTTP 200 OK` and an **uploadSession** object.</span></span> <span data-ttu-id="48865-170">Observe o seguinte no objeto de resposta:</span><span class="sxs-lookup"><span data-stu-id="48865-170">Note the following in the response object:</span></span>

- <span data-ttu-id="48865-171">A propriedade **ExpirationDateTime** indica a data/hora de vencimento para o token de autenticação inserido no valor da propriedade **uploadUrl**.</span><span class="sxs-lookup"><span data-stu-id="48865-171">The **ExpirationDateTime** property indicates the expiration date/time for the auth token embedded in the **uploadUrl** property value.</span></span> <span data-ttu-id="48865-172">Essa data/hora de vencimento permanece a mesma que foi retornada pela **uploadSession** inicial na etapa 1.</span><span class="sxs-lookup"><span data-stu-id="48865-172">This expiration date/time remains the same as returned by the initial **uploadSession** in step 1.</span></span>
- <span data-ttu-id="48865-173">**NextExpectedRanges** especifica o próximo local do byte para começar o carregamento a partir de `"NextExpectedRanges":["2097152"]`, por exemplo.</span><span class="sxs-lookup"><span data-stu-id="48865-173">The **NextExpectedRanges** specifies the next byte location to start uploading from, for example, `"NextExpectedRanges":["2097152"]`.</span></span> <span data-ttu-id="48865-174">Você deve carregar os bytes em um arquivo na ordem.</span><span class="sxs-lookup"><span data-stu-id="48865-174">You must upload bytes in a file in order.</span></span>
<!-- The **NextExpectedRanges** specifies one or more byte ranges, each indicating the starting point of a subsequent `PUT` request:

  - On a successful upload, this property returns the next range to start from, for example, `"NextExpectedRanges":["2097152"]`.
  - If a portion of a byte range has not uploaded successfully, this property includes the byte range with the start and end locations, for example, `"NextExpectedRanges":["1998457-2097094"]`.
-->
- <span data-ttu-id="48865-175">A propriedade **uploadUrl** não é retornada explicitamente, pois todas as operações `PUT` de uma sessão de carregamento usam a mesma URL retornada ao criar a sessão (etapa 1).</span><span class="sxs-lookup"><span data-stu-id="48865-175">The **uploadUrl** property is not explicitly returned, because all `PUT` operations of an upload session use the same URL returned when creating the session (step 1).</span></span>

### <a name="example-first-upload-to-the-message"></a><span data-ttu-id="48865-176">Exemplo: primeiro carregamento na mensagem</span><span class="sxs-lookup"><span data-stu-id="48865-176">Example: first upload to the message</span></span>
#### <a name="request"></a><span data-ttu-id="48865-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48865-177">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://outlook.office.com/api/v2.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
Content-Type: application/octet-stream
Content-Length: 2097152
Content-Range: bytes 0-2097151/3483322

{
  <bytes 0-2097151 of the file to be attached, in binary format>
}
```

#### <a name="response"></a><span data-ttu-id="48865-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="48865-178">Response</span></span>

<span data-ttu-id="48865-179">O exemplo de resposta a seguir mostra na propriedade **NextExpectedRanges** o início do próximo intervalo de bytes que o servidor espera.</span><span class="sxs-lookup"><span data-stu-id="48865-179">The following example response shows in the **NextExpectedRanges** property the start of the next byte range that the server expects.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://outlook.office.com/api/v2.0/$metadata#Users('a8e8e219-4931-95c1-b73d-62626fd79c32%4072aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA%3D')/AttachmentSessions/$entity",
  "ExpirationDateTime":"2019-09-25T01:09:30.7671707Z",
  "NextExpectedRanges":["2097152"]
}
```

### <a name="example-first-upload-to-the-event"></a><span data-ttu-id="48865-180">Exemplo: primeiro carregamento na evento</span><span class="sxs-lookup"><span data-stu-id="48865-180">Example: first upload to the event</span></span>
#### <a name="request"></a><span data-ttu-id="48865-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48865-181">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://outlook.office.com/api/v2.0/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/AttachmentSessions('AAMkADU5RpAACJlCs8AAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIBtw
Content-Type: application/octet-stream
Content-Length: 2097152
Content-Range: bytes 0-2097151/3483322

{
  <bytes 0-2097151 of the file to be attached, in binary format>
}
```

#### <a name="response"></a><span data-ttu-id="48865-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="48865-182">Response</span></span>

<span data-ttu-id="48865-183">O exemplo de resposta a seguir mostra na propriedade **NextExpectedRanges** o início do próximo intervalo de bytes que o servidor espera.</span><span class="sxs-lookup"><span data-stu-id="48865-183">The following example response shows in the **NextExpectedRanges** property the start of the next byte range that the server expects.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://outlook.office.com/api/v2.0/$metadata#Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69%4098a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA%3D')/AttachmentSessions/$entity",
    "ExpirationDateTime":"2020-02-22T02:46:56.7410786Z",
    "NextExpectedRanges":["2097152"]
}
```


## <a name="step-3-continue-uploading-byte-ranges-until-the-entire-file-has-been-uploaded"></a><span data-ttu-id="48865-184">Etapa 3: continuar carregando intervalos de bytes até que todo o arquivo tenha sido carregado</span><span class="sxs-lookup"><span data-stu-id="48865-184">Step 3: Continue uploading byte ranges until the entire file has been uploaded</span></span>

<span data-ttu-id="48865-185">Após o carregamento inicial na etapa 2, continue a carregar a parte restante do arquivo, usando uma solicitação `PUT` semelhante, conforme descrito na etapa 2, antes que você atinja a data/hora de vencimento da sessão.</span><span class="sxs-lookup"><span data-stu-id="48865-185">Following the initial upload in step 2, continue to upload the remaining portion of the file, using a similar `PUT` request as described in step 2, before you reach the expiration date/time for the session.</span></span> <span data-ttu-id="48865-186">Use a coleção **NextExpectedRanges** para determinar onde começar o próximo intervalo de bytes a ser carregado.</span><span class="sxs-lookup"><span data-stu-id="48865-186">Use the **NextExpectedRanges** collection to determine where to start the next byte range to upload.</span></span> <span data-ttu-id="48865-187">É possível ver vários intervalos especificados, indicando partes do arquivo que o servidor ainda não recebeu.</span><span class="sxs-lookup"><span data-stu-id="48865-187">You may see multiple ranges specified, indicating parts of the file that the server has not yet received.</span></span> <span data-ttu-id="48865-188">Isso é útil quando você precisa retomar uma transferência que foi interrompida, e seu cliente não tem certeza sobre o estado no serviço.</span><span class="sxs-lookup"><span data-stu-id="48865-188">This is useful if you need to resume a transfer that was interrupted and your client is unsure of the state on the service.</span></span>

<span data-ttu-id="48865-189">Quando o último byte do arquivo for carregado com êxito, a operação de `PUT` final retornará `HTTP 201 Created` e um cabeçalho `Location` que indica a URL para o anexo de arquivo no domínio `https://outlook.office.com`.</span><span class="sxs-lookup"><span data-stu-id="48865-189">Once the last byte of the file has been successfully uploaded, the final `PUT` operation returns `HTTP 201 Created` and a `Location` header that indicates the URL to the file attachment in the `https://outlook.office.com` domain.</span></span> <span data-ttu-id="48865-190">Você pode obter a ID do anexo na URL e salvá-la para uso posterior.</span><span class="sxs-lookup"><span data-stu-id="48865-190">You can get the attachment ID from the URL and save it for later use.</span></span> <span data-ttu-id="48865-191">Dependendo do cenário, você pode usar essa ID para [obter os metadados do anexo](/graph/api/attachment-get?view=graph-rest-1.0)ou [remover o anexo do item do Outlook](/graph/api/attachment-delete?view=graph-rest-1.0) usando o ponto de extremidade do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="48865-191">Depending on your scenario, you can use that ID to [get the metadata of the attachment](/graph/api/attachment-get?view=graph-rest-1.0), or [remove the attachment from the Outlook item](/graph/api/attachment-delete?view=graph-rest-1.0) using the Microsoft Graph endpoint.</span></span>

<span data-ttu-id="48865-192">Os exemplos a seguir mostram o carregamento do último intervalo de bytes do arquivo na mensagem e no evento das etapas anteriores.</span><span class="sxs-lookup"><span data-stu-id="48865-192">The following examples show uploading the last byte range of the file to the message and to the event in the preceding steps.</span></span>

### <a name="example-final-upload-to-the-message"></a><span data-ttu-id="48865-193">Exemplo: último carregamento na mensagem</span><span class="sxs-lookup"><span data-stu-id="48865-193">Example: final upload to the message</span></span>
#### <a name="request"></a><span data-ttu-id="48865-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48865-194">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://outlook.office.com/api/v2.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
Content-Type: application/octet-stream
Content-Length: 1386170
Content-Range: bytes 2097152-3483321/3483322

{
  <bytes 2097152-3483321 of the file to be attached, in binary format>
}
```

#### <a name="response"></a><span data-ttu-id="48865-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="48865-195">Response</span></span>
<span data-ttu-id="48865-196">O exemplo de resposta a seguir mostra um cabeçalho de resposta de `Location` onde você pode salvar a ID do anexo (`AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=`) para uso posterior.</span><span class="sxs-lookup"><span data-stu-id="48865-196">The following example response shows a `Location` response header from which you can save the attachment ID (`AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=`) for later use.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 201 Created

Location: https://outlook.office.com/api/v2.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/Attachments('AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=')
Content-Length: 0
```

### <a name="example-final-upload-to-the-event"></a><span data-ttu-id="48865-197">Exemplo: último carregamento no evento</span><span class="sxs-lookup"><span data-stu-id="48865-197">Example: final upload to the event</span></span>
#### <a name="request"></a><span data-ttu-id="48865-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48865-198">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://outlook.office.com/api/v2.0/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/AttachmentSessions('AAMkADU5RpAACJlCs8AAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIBtw
Content-Type: application/octet-stream
Content-Length: 1386170
Content-Range: bytes 2097152-3483321/3483322

{
  <bytes 2097152-3483321 of the file to be attached, in binary format>
}
```

#### <a name="response"></a><span data-ttu-id="48865-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="48865-199">Response</span></span>
<span data-ttu-id="48865-200">O exemplo de resposta a seguir mostra um cabeçalho de resposta de `Location` onde você pode salvar a ID do anexo (`AAMkADU5CCmSAAANZAlYPeyQByv7Y=`) para uso posterior.</span><span class="sxs-lookup"><span data-stu-id="48865-200">The following example response shows a `Location` response header from which you can save the attachment ID (`AAMkADU5CCmSAAANZAlYPeyQByv7Y=`) for later use.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 201 Created

Location: https://outlook.office.com/api/v2.0/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/Attachments('AAMkADU5CCmSAAANZAlYPeyQByv7Y=')
Content-Length: 0
```

## <a name="step-4-optional-get-the-file-attachment-from-the-outlook-item"></a><span data-ttu-id="48865-201">Etapa 4 (opcional): obter o arquivo em anexo do item do Outlook</span><span class="sxs-lookup"><span data-stu-id="48865-201">Step 4 (optional): Get the file attachment from the Outlook item</span></span>

<span data-ttu-id="48865-202">Como sempre, [obter um anexo](/graph/api/attachment-get?view=graph-rest-1.0) a partir de um item do Outlook não é tecnicamente limitado pelo tamanho do anexo.</span><span class="sxs-lookup"><span data-stu-id="48865-202">As always, [getting an attachment](/graph/api/attachment-get?view=graph-rest-1.0) from an Outlook item is not technically limited by attachment size.</span></span>

<span data-ttu-id="48865-203">No entanto, obter um anexo de arquivo grande no formato base64-encoded afeta o desempenho da API.</span><span class="sxs-lookup"><span data-stu-id="48865-203">However, getting a large file attachment in base64-encoded format affects API performance.</span></span> <span data-ttu-id="48865-204">Se você espera um anexo grande:</span><span class="sxs-lookup"><span data-stu-id="48865-204">If you expect a large attachment:</span></span>

- <span data-ttu-id="48865-205">Como uma alternativa para obter o conteúdo do anexo no formato base64, você pode [obter os dados brutos do arquivo em anexo](/graph/api/attachment-get?view=graph-rest-1.0#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="48865-205">As an alternative to getting the attachment content in base64 format, you can [get the raw data of the file attachment](/graph/api/attachment-get?view=graph-rest-1.0#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message).</span></span>
- <span data-ttu-id="48865-206">Para [obter os metadados do anexo de arquivo](/graph/api/attachment-get?view=graph-rest-1.0#example-1-get-the-properties-of-a-file-attachment), acrescente um parâmetro `$select` para incluir somente as propriedades de metadados desejadas, excluindo a propriedade **contentBytes** que retorna o arquvo em anexo no formato base64.</span><span class="sxs-lookup"><span data-stu-id="48865-206">To [get the metadata of the file attachment](/graph/api/attachment-get?view=graph-rest-1.0#example-1-get-the-properties-of-a-file-attachment), append a `$select` parameter to include only those metadata properties you want, excluding the **contentBytes** property which returns the file attachment in base64 format.</span></span>

### <a name="example-get-the-raw-file-attached-to-the-event"></a><span data-ttu-id="48865-207">Exemplo: obter o arquivo bruto anexado ao evento</span><span class="sxs-lookup"><span data-stu-id="48865-207">Example: Get the raw file attached to the event</span></span>
<span data-ttu-id="48865-208">Seguindo o exemplo de evento e utilizando a ID do anexo retornada no cabeçalho de `Location` da etapa anterior, o próximo exemplo de solicitação mostra o uso de um parâmetro `$value` para obter os dados de conteúdo bruto do anexo.</span><span class="sxs-lookup"><span data-stu-id="48865-208">Following the event example and using the attachment ID returned in the `Location` header of the previous step, the next example request shows using a `$value` parameter to get the attachment raw content data.</span></span>

#### <a name="request"></a><span data-ttu-id="48865-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48865-209">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "walkthrough_get_attachment_raw",
  "sampleKeys": ["d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32", "AAMkADU5CCmSAAA=", "AAMkADU5CCmSAAANZAlYPeyQByv7Y="]
}-->
```http
GET https://graph.microsoft.com/v1.0/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/Attachments('AAMkADU5CCmSAAANZAlYPeyQByv7Y=')/$value
```

#### <a name="response"></a><span data-ttu-id="48865-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="48865-210">Response</span></span>

<!-- {
  "blockType": "ignored",
  "name": "walkthrough_get_attachment_raw",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
content-length: 3483322
Content-type: image/jpeg

{Raw bytes of the file}
```


### <a name="example-get-the-metadata-of-the-file-attached-to-the-message"></a><span data-ttu-id="48865-211">Exemplo: obter os metadados do arquivo anexado à mensagem</span><span class="sxs-lookup"><span data-stu-id="48865-211">Example: Get the metadata of the file attached to the message</span></span>
<span data-ttu-id="48865-212">Seguindo o exemplo da mensagem, o próximo exemplo de solicitação mostra o uso de um parâmetro `$select` para obter alguns dos metadados de um anexo de arquivo em uma mensagem, excluindo o **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="48865-212">Following the message example, the next example request shows using a `$select` parameter to get some of the metadata of a file attachment on a message, excluding **contentBytes**.</span></span>

#### <a name="request"></a><span data-ttu-id="48865-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48865-213">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "walkthrough_get_attachment_metadata",
  "sampleKeys": ["a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47", "AAMkADI5MAAIT3drCAAA=", "AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0="]
}-->
```http
GET https://graph.microsoft.com/api/v1.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/Attachments('AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=')?$select=lastModifiedDateTime,name,contentType,size,isInline
```

#### <a name="response"></a><span data-ttu-id="48865-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="48865-214">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "walkthrough_get_attachment_metadata",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('a8e8e219-4931-95c1-b73d-62626fd79c32%4072aa88bf-76f0-494f-91ab-2d7cd730db47')/messages('AAMkADI5MAAIT3drCAAA%3D')/attachments/$entity",
    "@odata.type": "#microsoft.graph.fileAttachment",
    "@odata.mediaContentType": "image/jpeg",
    "id": "AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=",
    "lastModifiedDateTime": "2019-09-24T23:27:43Z",
    "name": "flower",
    "contentType": "image/jpeg",
    "size": 3640066,
    "isInline": false
}
```


## <a name="alternative-cancel-the-upload-session"></a><span data-ttu-id="48865-215">Alternativa: cancelar a sessão de carregamento</span><span class="sxs-lookup"><span data-stu-id="48865-215">Alternative: Cancel the upload session</span></span>

<span data-ttu-id="48865-216">Em qualquer momento antes da sessão de carregamento expirar, se for preciso cancelar o carregamento, você poderá usar a mesma URL opaca inicial para excluir a sessão de carregamento.</span><span class="sxs-lookup"><span data-stu-id="48865-216">At any point of time before the upload session expires, if you have to cancel the upload, you can use the same initial opaque URL to delete the upload session.</span></span> <span data-ttu-id="48865-217">Uma operação bem-sucedida retorna `HTTP 204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="48865-217">A successful operation returns `HTTP 204 No Content`.</span></span>

### <a name="example-cancel-the-upload-session-for-the-message"></a><span data-ttu-id="48865-218">Exemplo: cancelar a sessão de carregamento da mensagem</span><span class="sxs-lookup"><span data-stu-id="48865-218">Example: cancel the upload session for the message</span></span>

#### <a name="request"></a><span data-ttu-id="48865-219">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48865-219">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
DELETE https://outlook.office.com/api/v2.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
```

#### <a name="response"></a><span data-ttu-id="48865-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="48865-220">Response</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 204 No content
```
## <a name="errors"></a><span data-ttu-id="48865-221">Erros</span><span class="sxs-lookup"><span data-stu-id="48865-221">Errors</span></span>

### <a name="errorattachmentsizeshouldnotbelessthanminimumsize"></a><span data-ttu-id="48865-222">ErrorAttachmentSizeShouldNotBeLessThanMinimumSize</span><span class="sxs-lookup"><span data-stu-id="48865-222">ErrorAttachmentSizeShouldNotBeLessThanMinimumSize</span></span>

<span data-ttu-id="48865-223">Este erro é devolvido ao tentar [criar uma sessão de upload](/graph/api/attachment-createuploadsession?view=graph-rest-1.0) para anexar um arquivo menor que 3 MB.</span><span class="sxs-lookup"><span data-stu-id="48865-223">This error is returned when attempting to [create an upload session](/graph/api/attachment-createuploadsession?view=graph-rest-1.0) to attach a file smaller than 3 MB.</span></span> <span data-ttu-id="48865-224">Se o tamanho do arquivo for menor que 3 MB, faça uma única POSTAGEM na propriedade de navegação dos **anexos** da [mensagem](/graph/api/message-post-attachments?view=graph-rest-1.0) ou do [evento](/graph/api/event-post-attachments?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="48865-224">If the file size is under 3 MB, you should do a single POST on the **attachments** navigation property [of the message](/graph/api/message-post-attachments?view=graph-rest-1.0) or [of the event](/graph/api/event-post-attachments?view=graph-rest-1.0).</span></span> <span data-ttu-id="48865-225">A resposta `POST` bem-sucedida inclui a ID do arquivo anexado à mensagem.</span><span class="sxs-lookup"><span data-stu-id="48865-225">The successful `POST` response includes the ID of the file attached to the message.</span></span>

