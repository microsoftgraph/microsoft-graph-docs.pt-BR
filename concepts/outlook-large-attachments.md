---
title: Anexar arquivos grandes a mensagens do Outlook
description: Dependendo do tamanho do arquivo, você pode escolher uma de duas maneiras de anexar um arquivo a uma mensagem.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 74cc6ad4af5d649ca480c7b708b0716062e8d36a
ms.sourcegitcommit: 1a84f80798692fc0381b1acecfe023b3ce6ab02c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2020
ms.locfileid: "41953603"
---
# <a name="attach-large-files-to-outlook-messages-as-attachments-preview"></a><span data-ttu-id="26710-103">Anexar arquivos grandes às mensagens do Outlook como anexos (visualização)</span><span class="sxs-lookup"><span data-stu-id="26710-103">Attach large files to Outlook messages as attachments (preview)</span></span>

<span data-ttu-id="26710-104">Dependendo do tamanho do arquivo, você pode escolher uma das duas maneiras de anexar um arquivo a uma [mensagem](/graph/api/resources/message?view=graph-rest-beta):</span><span class="sxs-lookup"><span data-stu-id="26710-104">Depending on the size of the file, you can choose one of two ways to attach a file to a [message](/graph/api/resources/message?view=graph-rest-beta):</span></span>

- <span data-ttu-id="26710-105">Se o tamanho do arquivo é até 4 MB, você pode fazer um único [POST na propriedade de navegação de anexos da mensagem](/graph/api/message-post-attachments?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="26710-105">If the file size is under 4 MB, you can do a single [POST on the attachments navigation property of the message](/graph/api/message-post-attachments?view=graph-rest-beta).</span></span> <span data-ttu-id="26710-106">A resposta `POST` bem-sucedida inclui a ID do arquivo anexado à mensagem.</span><span class="sxs-lookup"><span data-stu-id="26710-106">The successful `POST` response includes the ID of the file attached to the message.</span></span>
- <span data-ttu-id="26710-107">Se o tamanho do arquivo estiver entre 3 MB e 150 MB, crie uma sessão de carregamento e use o `PUT` iteradamente para carregar intervalos de bytes do arquivo até que você carregue todo o arquivo.</span><span class="sxs-lookup"><span data-stu-id="26710-107">If the file size is between 3MB and 150MB, create an upload session, and iteratively use `PUT` to upload ranges of bytes of the file until you have uploaded the entire file.</span></span> <span data-ttu-id="26710-108">Um cabeçalho na resposta `PUT` finalizada com êxito inclui uma URL com a ID do anexo.</span><span class="sxs-lookup"><span data-stu-id="26710-108">A header in the final successful `PUT` response includes a URL with the attachment ID.</span></span>

<span data-ttu-id="26710-109">Este artigo usa um exemplo para ilustrar a segunda abordagem.</span><span class="sxs-lookup"><span data-stu-id="26710-109">This article uses an example to illustrate the second approach.</span></span> <span data-ttu-id="26710-110">O exemplo cria e usa uma sessão de carregamento para adicionar um anexo de arquivo grande (com tamanho acima de 3 MB) a uma mensagem específica.</span><span class="sxs-lookup"><span data-stu-id="26710-110">The example creates and uses an upload session to add a large file attachment (of size over 3MB) to a specific message.</span></span> <span data-ttu-id="26710-111">Depois de carregar o arquivo inteiro, ele recebe uma URL que contém uma identificação para o arquivo em anexo, com o qual ele pode fazer outras operações, como obter os metadados do anexo de arquivo.</span><span class="sxs-lookup"><span data-stu-id="26710-111">Upon successfully uploading the entire file, it gets a URL that contains an ID for the file attachment, with which it can do other operations such as getting the file attachment metadata.</span></span>

## <a name="step-1-create-an-upload-session"></a><span data-ttu-id="26710-112">Etapa 1: Criar uma sessão de upload</span><span class="sxs-lookup"><span data-stu-id="26710-112">Step 1: Create an upload session</span></span>

<span data-ttu-id="26710-113">[Criar uma sessão de carregamento](/graph/api/attachment-createuploadsession?view=graph-rest-beta) para anexar um arquivo a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="26710-113">[Create an upload session](/graph/api/attachment-createuploadsession?view=graph-rest-beta) to attach a file to a message.</span></span> <span data-ttu-id="26710-114">Especifique o arquivo no parâmetro de entrada **AttachmentItem**.</span><span class="sxs-lookup"><span data-stu-id="26710-114">Specify the file in the input parameter **AttachmentItem**.</span></span>

<span data-ttu-id="26710-115">Uma operação bem-sucedida retorna `HTTP 201 Created` e uma nova instância[uploadSession](/graph/api/resources/uploadsession?view=graph-rest-beta), que contém uma URL opaca que você pode usar em operações `PUT` subseqüentes para carregar partes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="26710-115">A successful operation returns `HTTP 201 Created` and a new [uploadSession](/graph/api/resources/uploadsession?view=graph-rest-beta) instance, which contains an opaque URL that you can use in subsequent `PUT` operations to upload portions of the file.</span></span> <span data-ttu-id="26710-116">A **uploadSession** fornece um local de armazenamento temporário onde os bytes do arquivo são salvos até que você tenha carregado o arquivo completo.</span><span class="sxs-lookup"><span data-stu-id="26710-116">The **uploadSession** provides a temporary storage location where the bytes of the file are saved until you have uploaded the complete file.</span></span>

<span data-ttu-id="26710-117">Verifique se solicitou `Mail.ReadWrite`permissão para criar **uploadSession**.</span><span class="sxs-lookup"><span data-stu-id="26710-117">Make sure to request `Mail.ReadWrite` permission to create the **uploadSession**.</span></span> <span data-ttu-id="26710-118">A URL opaca, retornada na propriedade **uploadUrl** do novo **uploadSession** é pré-autenticada e contém o token de autorização apropriado para consultas `PUT` subsequentes no domínio `https://outlook.office.com`.</span><span class="sxs-lookup"><span data-stu-id="26710-118">The opaque URL, returned in the **uploadUrl** property of the new **uploadSession**, is pre-authenticated and contains the appropriate authorization token for subsequent `PUT` queries in the `https://outlook.office.com` domain.</span></span> <span data-ttu-id="26710-119">Esse token expira por **expirationDateTime**.</span><span class="sxs-lookup"><span data-stu-id="26710-119">That token expires by **expirationDateTime**.</span></span> <span data-ttu-id="26710-120">Não Personalize essa URL para as operações `PUT`.</span><span class="sxs-lookup"><span data-stu-id="26710-120">Do not customize this URL for the `PUT` operations.</span></span>

<span data-ttu-id="26710-121">O objeto**uploadSession** na resposta também inclui a propriedade **nextExpectedRanges**, que indica que o local inicial de carregamento deve ser byte 0.</span><span class="sxs-lookup"><span data-stu-id="26710-121">The **uploadSession** object in the response also includes the **nextExpectedRanges** property, which indicates the initial upload starting location should be byte 0.</span></span>

### <a name="example-request-create-an-upload-session"></a><span data-ttu-id="26710-122">Solicitação de exemplo: criar uma sessão de carregamento</span><span class="sxs-lookup"><span data-stu-id="26710-122">Example request: create an upload session</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="26710-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="26710-123">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "walkthrough_create_uploadsession",
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="26710-124">C#</span><span class="sxs-lookup"><span data-stu-id="26710-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/walkthrough-create-uploadsession-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="26710-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26710-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/walkthrough-create-uploadsession-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="26710-126">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26710-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/walkthrough-create-uploadsession-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="example-response-get-an-uploadsession-object"></a><span data-ttu-id="26710-127">Exemplo de resposta: Obtenha um objeto uploadSession</span><span class="sxs-lookup"><span data-stu-id="26710-127">Example response: get an uploadSession object</span></span>
<!-- {
  "blockType": "response",
  "name": "walkthrough_create_uploadsession",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI",
    "expirationDateTime": "2019-09-25T01:09:30.7671707Z",
    "nextExpectedRanges": [
        "0-"
    ]
}
```


## <a name="step-2-use-the-upload-session-to-upload-a-range-of-bytes-of-the-file"></a><span data-ttu-id="26710-128">Etapa 2: Usar a sessão de carregamento para carregar um intervalo de bytes do arquivo</span><span class="sxs-lookup"><span data-stu-id="26710-128">Step 2: Use the upload session to upload a range of bytes of the file</span></span>

<span data-ttu-id="26710-129">Para carregar o arquivo, ou uma parte do arquivo, faça uma solicitação `PUT` para o valor da propriedade **uploadUrl** retornado como parte de **uploadSession** na etapa 1.</span><span class="sxs-lookup"><span data-stu-id="26710-129">To upload the file, or a portion of the file, make a `PUT` request to the **uploadUrl** property value returned as part of the **uploadSession** in step 1.</span></span> <span data-ttu-id="26710-130">Você pode carregar todo o arquivo ou dividi-lo em vários intervalos de bytes.</span><span class="sxs-lookup"><span data-stu-id="26710-130">You can upload the entire file, or split the file into multiple byte ranges.</span></span> <span data-ttu-id="26710-131">Para melhorar o desempenho, mantenha cada intervalo de bytes com menos de 4 MB.</span><span class="sxs-lookup"><span data-stu-id="26710-131">For better performance, keep each byte range less than 4 MB.</span></span>

<span data-ttu-id="26710-132">Especifique os cabeçalhos e corpo da solicitação conforme é descrito abaixo.</span><span class="sxs-lookup"><span data-stu-id="26710-132">Specify request headers and request body as described below.</span></span>

### <a name="request-headers"></a><span data-ttu-id="26710-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26710-133">Request headers</span></span>

| <span data-ttu-id="26710-134">Nome</span><span class="sxs-lookup"><span data-stu-id="26710-134">Name</span></span>       | <span data-ttu-id="26710-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="26710-135">Type</span></span> | <span data-ttu-id="26710-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="26710-136">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="26710-137">Content-Length</span><span class="sxs-lookup"><span data-stu-id="26710-137">Content-Length</span></span> | <span data-ttu-id="26710-138">Int32</span><span class="sxs-lookup"><span data-stu-id="26710-138">Int32</span></span> | <span data-ttu-id="26710-139">O número de bytes sendo carregados nesta operação.</span><span class="sxs-lookup"><span data-stu-id="26710-139">The number of bytes being uploaded in this operation.</span></span> <span data-ttu-id="26710-140">Para melhorar o desempenho, mantenha o limite superior do número de bytes para cada operação `PUT` em 4 MB.</span><span class="sxs-lookup"><span data-stu-id="26710-140">For better performance, keep the upper limit of the number of bytes for each `PUT` operation to 4 MB.</span></span> <span data-ttu-id="26710-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26710-141">Required.</span></span> |
| <span data-ttu-id="26710-142">Intervalo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="26710-142">Content-Range</span></span> | <span data-ttu-id="26710-143">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="26710-143">String</span></span> | <span data-ttu-id="26710-144">O intervalo de bytes baseado em 0 do arquivo que está sendo carregado nesta operação, expresso no formato `bytes {start}-{end}/{total}`.</span><span class="sxs-lookup"><span data-stu-id="26710-144">The 0-based byte range of the file being uploaded in this operation, expressed in the format `bytes {start}-{end}/{total}`.</span></span> <span data-ttu-id="26710-145">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26710-145">Required.</span></span> |
| <span data-ttu-id="26710-146">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26710-146">Content-Type</span></span> | <span data-ttu-id="26710-147">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="26710-147">String</span></span>  | <span data-ttu-id="26710-148">O tipo MIME.</span><span class="sxs-lookup"><span data-stu-id="26710-148">The MIME type.</span></span> <span data-ttu-id="26710-149">Especifique`application/octet-stream`.</span><span class="sxs-lookup"><span data-stu-id="26710-149">Specify `application/octet-stream`.</span></span> <span data-ttu-id="26710-150">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26710-150">Required.</span></span> |

<span data-ttu-id="26710-151">Não especifique um cabeçalho da solicitação`Authorization`.</span><span class="sxs-lookup"><span data-stu-id="26710-151">Do not specify an `Authorization` request header.</span></span> <span data-ttu-id="26710-152">A consulta `PUT` usa uma URL pré-existente da propriedade **uploadUrl**, que permite o acesso ao domínio `https://outlook.office.com`.</span><span class="sxs-lookup"><span data-stu-id="26710-152">The `PUT` query uses a pre-authenticated URL from the **uploadUrl** property, that allows access to the `https://outlook.office.com` domain.</span></span>

### <a name="request-body"></a><span data-ttu-id="26710-153">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26710-153">Request body</span></span>

<span data-ttu-id="26710-154">Especificar os bytes reais do arquivo a ser anexado, que estão no intervalo de local especificado pelo cabeçalho da solicitação`Content-Range`.</span><span class="sxs-lookup"><span data-stu-id="26710-154">Specify the actual bytes of the file to be attached, that are in the location range specified by the `Content-Range` request header.</span></span>

### <a name="response"></a><span data-ttu-id="26710-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="26710-155">Response</span></span>
<span data-ttu-id="26710-156">Um carregamento bem-sucedido retorna `HTTP 200 OK` e um objeto **uploadSession**.</span><span class="sxs-lookup"><span data-stu-id="26710-156">A successful upload returns `HTTP 200 OK` and an **uploadSession** object.</span></span> <span data-ttu-id="26710-157">Observe o seguinte no objeto de resposta:</span><span class="sxs-lookup"><span data-stu-id="26710-157">Note the following in the response object:</span></span>

- <span data-ttu-id="26710-158">A propriedade **ExpirationDateTime** indica a data/hora de vencimento para o token de autenticação inserido no valor da propriedade **uploadUrl**.</span><span class="sxs-lookup"><span data-stu-id="26710-158">The **ExpirationDateTime** property indicates the expiration date/time for the auth token embedded in the **uploadUrl** property value.</span></span> <span data-ttu-id="26710-159">Essa data/hora de vencimento permanece a mesma que foi retornada pela **uploadSession** inicial na etapa 1.</span><span class="sxs-lookup"><span data-stu-id="26710-159">This expiration date/time remains the same as returned by the initial **uploadSession** in step 1.</span></span>
- <span data-ttu-id="26710-160">**NextExpectedRanges** especifica o próximo local do byte para começar o carregamento a partir de `"NextExpectedRanges":["2097152"]`, por exemplo.</span><span class="sxs-lookup"><span data-stu-id="26710-160">The **NextExpectedRanges** specifies the next byte location to start uploading from, for example, `"NextExpectedRanges":["2097152"]`.</span></span> <span data-ttu-id="26710-161">Você deve carregar os bytes em um arquivo na ordem.</span><span class="sxs-lookup"><span data-stu-id="26710-161">You must upload bytes in a file in order.</span></span>
<!-- The **NextExpectedRanges** specifies one or more byte ranges, each indicating the starting point of a subsequent `PUT` request:

  - On a successful upload, this property returns the next range to start from, for example, `"NextExpectedRanges":["2097152"]`.
  - If a portion of a byte range has not uploaded successfully, this property includes the byte range with the start and end locations, for example, `"NextExpectedRanges":["1998457-2097094"]`.
-->
- <span data-ttu-id="26710-162">A propriedade **uploadUrl** não é retornada explicitamente, pois todas as operações `PUT` de uma sessão de carregamento usam a mesma URL retornada ao criar a sessão (etapa 1).</span><span class="sxs-lookup"><span data-stu-id="26710-162">The **uploadUrl** property is not explicitly returned, because all `PUT` operations of an upload session use the same URL returned when creating the session (step 1).</span></span>

### <a name="example-request-first-upload"></a><span data-ttu-id="26710-163">Solicitação de exemplo: primeiro carregamento</span><span class="sxs-lookup"><span data-stu-id="26710-163">Example request: first upload</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
Content-Type: application/octet-stream
Content-Length: 2097152
Content-Range: bytes 0-2097151/3483322

{
  <bytes 0-2097151 of the file to be attached, in binary format>
}
```

### <a name="example-response-get-the-start-of-the-next-byte-range-that-the-server-expects"></a><span data-ttu-id="26710-164">Resposta de exemplo: obter o início do próximo intervalo de bytes esperado pelo servidor</span><span class="sxs-lookup"><span data-stu-id="26710-164">Example response: get the start of the next byte range that the server expects</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://outlook.office.com/api/beta/$metadata#Users('a8e8e219-4931-95c1-b73d-62626fd79c32%4072aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA%3D')/AttachmentSessions/$entity",
  "ExpirationDateTime":"2019-09-25T01:09:30.7671707Z",
  "NextExpectedRanges":["2097152"]
}
```


## <a name="step-3-continue-uploading-byte-ranges-until-the-entire-file-has-been-uploaded"></a><span data-ttu-id="26710-165">Etapa 3: continuar carregando intervalos de bytes até que todo o arquivo tenha sido carregado</span><span class="sxs-lookup"><span data-stu-id="26710-165">Step 3: Continue uploading byte ranges until the entire file has been uploaded</span></span>

<span data-ttu-id="26710-166">Após o carregamento inicial na etapa 2, continue a carregar a parte restante do arquivo, usando uma solicitação `PUT` semelhante, conforme descrito na etapa 2, antes que você atinja a data/hora de vencimento da sessão.</span><span class="sxs-lookup"><span data-stu-id="26710-166">Following the initial upload in step 2, continue to upload the remaining portion of the file, using a similar `PUT` request as described in step 2, before you reach the expiration date/time for the session.</span></span> <span data-ttu-id="26710-167">Use a coleção **NextExpectedRanges** para determinar onde começar o próximo intervalo de bytes a ser carregado.</span><span class="sxs-lookup"><span data-stu-id="26710-167">Use the **NextExpectedRanges** collection to determine where to start the next byte range to upload.</span></span> <span data-ttu-id="26710-168">É possível ver vários intervalos especificados, indicando partes do arquivo que o servidor ainda não recebeu.</span><span class="sxs-lookup"><span data-stu-id="26710-168">You may see multiple ranges specified, indicating parts of the file that the server has not yet received.</span></span> <span data-ttu-id="26710-169">Isso é útil quando você precisa retomar uma transferência que foi interrompida, e seu cliente não tem certeza sobre o estado no serviço.</span><span class="sxs-lookup"><span data-stu-id="26710-169">This is useful if you need to resume a transfer that was interrupted and your client is unsure of the state on the service.</span></span>

<span data-ttu-id="26710-170">Quando o último byte do arquivo for carregado com êxito, a operação de `PUT` final retornará `HTTP 201 Created` e um cabeçalho `Location` que indica a URL para o anexo de arquivo no domínio `https://outlook.office.com`.</span><span class="sxs-lookup"><span data-stu-id="26710-170">Once the last byte of the file has been successfully uploaded, the final `PUT` operation returns `HTTP 201 Created` and a `Location` header that indicates the URL to the file attachment in the `https://outlook.office.com` domain.</span></span> <span data-ttu-id="26710-171">Você pode obter a ID do anexo na URL e salvá-la para uso posterior.</span><span class="sxs-lookup"><span data-stu-id="26710-171">You can get the attachment ID from the URL and save it for later use.</span></span> <span data-ttu-id="26710-172">Dependendo do seu cenário, você pode usar essa ID para [obter os metadados do anexo](/graph/api/attachment-get?view=graph-rest-beta)ou [remover o anexo da mensagem](/graph/api/attachment-delete?view=graph-rest-beta) usando o ponto de extremidade do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="26710-172">Depending on your scneario, you can use that ID to [get the metadata of the attachment](/graph/api/attachment-get?view=graph-rest-beta), or [remove the attachment from the message](/graph/api/attachment-delete?view=graph-rest-beta) using the Microsoft Graph endpoint.</span></span>

<span data-ttu-id="26710-173">O exemplo a seguir mostra como carregar o último intervalo de bytes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="26710-173">The following example shows uploading the last byte range of the file.</span></span>

### <a name="example-request-final-upload"></a><span data-ttu-id="26710-174">Solicitação de exemplo: carregamento final</span><span class="sxs-lookup"><span data-stu-id="26710-174">Example request: final upload</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
Content-Type: application/octet-stream
Content-Length: 1386170
Content-Range: bytes 2097152-3483321/3483322

{
  <bytes 2097152-3483321 of the file to be attached, in binary format>
}
```

### <a name="example-response-get-the-location-response-header-to-save-the-attachment-id"></a><span data-ttu-id="26710-175">Resposta de exemplo: obter o cabeçalho de resposta do local para salvar a ID do anexo</span><span class="sxs-lookup"><span data-stu-id="26710-175">Example response: get the Location response header to save the attachment ID</span></span>

<span data-ttu-id="26710-176">Na URL especificada pelo cabeçalho da resposta `Location`, salve a ID do anexo (`AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=`) para uso posterior.</span><span class="sxs-lookup"><span data-stu-id="26710-176">From the URL specified by the `Location` response header, save the attachment ID (`AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=`) for later use.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 201 Created

Location: https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/Attachments('AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=')
Content-Length: 0
```

## <a name="step-4-optional-get-the-file-attachment-from-the-message"></a><span data-ttu-id="26710-177">Etapa 4 (opcional): obter o arquivo em anexo da mensagem</span><span class="sxs-lookup"><span data-stu-id="26710-177">Step 4 (optional): Get the file attachment from the message</span></span>

<span data-ttu-id="26710-178">Como sempre, [obter um anexo](/graph/api/attachment-get?view=graph-rest-beta) a partir de uma mensagem não é tecnicamente limitado pelo tamanho do anexo.</span><span class="sxs-lookup"><span data-stu-id="26710-178">As always, [getting an attachment](/graph/api/attachment-get?view=graph-rest-beta) from a message is not technically limited by attachment size.</span></span>

<span data-ttu-id="26710-179">No entanto, obter um anexo de arquivo grande no formato base64-encoded afeta o desempenho da API.</span><span class="sxs-lookup"><span data-stu-id="26710-179">However, getting a large file attachment in base64-encoded format affects API performance.</span></span> <span data-ttu-id="26710-180">Se você espera um anexo grande:</span><span class="sxs-lookup"><span data-stu-id="26710-180">If you expect a large attachment:</span></span>

- <span data-ttu-id="26710-181">Como uma alternativa para obter o conteúdo do anexo no formato base64, você pode [obter os dados brutos do arquivo em anexo](/graph/api/attachment-get#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="26710-181">As an alternative to getting the attachment content in base64 format, you can [get the raw data of the file attachment](/graph/api/attachment-get#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message?view=graph-rest-1.0).</span></span>
- <span data-ttu-id="26710-182">Para [obter os metadados do anexo de arquivo](/graph/api/attachment-get?view=graph-rest-beta#example-1-get-the-properties-of-a-file-attachment), acrescente um parâmetro `$select` para incluir somente as propriedades de metadados desejadas, excluindo a propriedade **contentBytes** que retorna o arquvo em anexo no formato base64.</span><span class="sxs-lookup"><span data-stu-id="26710-182">To [get the metadata of the file attachment](/graph/api/attachment-get?view=graph-rest-beta#example-1-get-the-properties-of-a-file-attachment), append a `$select` parameter to include only those metadata properties you want, excluding the **contentBytes** property which returns the file attachment in base64 format.</span></span>

### <a name="example-request-get-the-file-attachment-metadata"></a><span data-ttu-id="26710-183">Solicitação de exemplo: obter os metadados do arquivo em anexo</span><span class="sxs-lookup"><span data-stu-id="26710-183">Example request: get the file attachment metadata</span></span>

<span data-ttu-id="26710-184">O exemplo a seguir mostra o remetente usando um parâmetro `$select` para obter todos os metadados de um arquivo em anexo em uma mensagem, exceto o **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="26710-184">The following example shows the sender using a `$select` parameter to get all the metadata of a file attachment on a message, except **contentBytes**.</span></span>

<!-- {
  "blockType": "request",
  "name": "walkthrough_get_attachment",
  "sampleKeys": ["a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47", "AAMkADI5MAAIT3drCAAA=", "AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0="]
}-->
```http
GET https://graph.microsoft.com/api/v1.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/Attachments('AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=')?$select=lastModifiedDateTime,name,contentType,size,isInline
```

### <a name="example-response"></a><span data-ttu-id="26710-185">Resposta de exemplo</span><span class="sxs-lookup"><span data-stu-id="26710-185">Example response</span></span>

<!-- {
  "blockType": "response",
  "name": "walkthrough_get_attachment",
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

## <a name="alternative-cancel-the-upload-session"></a><span data-ttu-id="26710-186">Alternativa: cancelar a sessão de carregamento</span><span class="sxs-lookup"><span data-stu-id="26710-186">Alternative: Cancel the upload session</span></span>

<span data-ttu-id="26710-187">Em qualquer momento antes da sessão de carregamento expirar, se for preciso cancelar o carregamento, você poderá usar a mesma URL opaca inicial para excluir a sessão de carregamento.</span><span class="sxs-lookup"><span data-stu-id="26710-187">At any point of time before the upload session expires, if you have to cancel the upload, you can use the same initial opaque URL to delete the upload session.</span></span> <span data-ttu-id="26710-188">Uma operação bem-sucedida retorna `HTTP 204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="26710-188">A successful operation returns `HTTP 204 No Content`.</span></span>

### <a name="example-request-cancel-an-upload-session"></a><span data-ttu-id="26710-189">Solicitação de exemplo: cancelar uma sessão de carregamento</span><span class="sxs-lookup"><span data-stu-id="26710-189">Example request: cancel an upload session</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
DELETE https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
```

### <a name="example-response"></a><span data-ttu-id="26710-190">Resposta de exemplo</span><span class="sxs-lookup"><span data-stu-id="26710-190">Example response</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 204 No content
```


