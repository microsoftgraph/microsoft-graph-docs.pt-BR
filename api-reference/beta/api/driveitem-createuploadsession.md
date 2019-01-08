---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Upload de arquivos retomável
ms.openlocfilehash: b4519de2a4fb417ce8a0b4524fff6d60547be7ec
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748434"
---
# <a name="upload-large-files-with-an-upload-session"></a><span data-ttu-id="64759-102">Carregar arquivos grandes com uma sessão de upload</span><span class="sxs-lookup"><span data-stu-id="64759-102">Upload large files with an upload session</span></span>

> <span data-ttu-id="64759-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="64759-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64759-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="64759-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="64759-p102">Crie uma sessão de upload para permitir que seu aplicativo carregue arquivos até o tamanho máximo de arquivo. Uma sessão de upload permite que seu aplicativo carregue intervalos do arquivo em solicitações de API sequenciais, permitindo que a transferência seja retomada se uma conexão for interrompida enquanto o upload estiver em andamento.</span><span class="sxs-lookup"><span data-stu-id="64759-p102">Create an upload session to allow your app to upload files up to the maximum file size. An upload session allows your app to upload ranges of the file in sequential API requests, which allows the transfer to be resumed if a connection is dropped while the upload is in progress.</span></span>

<span data-ttu-id="64759-107">Para carregar um arquivo usando uma sessão de upload, duas etapas são obrigatórias:</span><span class="sxs-lookup"><span data-stu-id="64759-107">To upload a file using an upload session, there are two steps:</span></span>

1. [<span data-ttu-id="64759-108">Criar uma sessão de upload</span><span class="sxs-lookup"><span data-stu-id="64759-108">Create an upload session</span></span>](#create-an-upload-session)
2. [<span data-ttu-id="64759-109">Carregar bytes na sessão de upload</span><span class="sxs-lookup"><span data-stu-id="64759-109">Upload bytes to the upload session</span></span>](#upload-bytes-to-the-upload-session)

## <a name="permissions"></a><span data-ttu-id="64759-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="64759-110">Permissions</span></span>

<span data-ttu-id="64759-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64759-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64759-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64759-113">Permission type</span></span>      | <span data-ttu-id="64759-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64759-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64759-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64759-115">Delegated (work or school account)</span></span> | <span data-ttu-id="64759-116">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64759-116">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="64759-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64759-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64759-118">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64759-118">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="64759-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64759-119">Application</span></span> | <span data-ttu-id="64759-120">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64759-120">Sites.ReadWrite.All</span></span> |

## <a name="create-an-upload-session"></a><span data-ttu-id="64759-121">Criar uma sessão de carregamento</span><span class="sxs-lookup"><span data-stu-id="64759-121">Create an upload session</span></span>

<span data-ttu-id="64759-122">Para começar um carregamento de arquivos grandes, seu aplicativo deverá solicitar primeiro uma nova sessão de carregamento.</span><span class="sxs-lookup"><span data-stu-id="64759-122">To begin a large file upload, your app must first request a new upload session.</span></span>
<span data-ttu-id="64759-123">Isso cria um local de armazenamento temporário onde os bytes do arquivo serão salvo até que o arquivo completo é carregado.</span><span class="sxs-lookup"><span data-stu-id="64759-123">This creates a temporary storage location where the bytes of the file will be saved until the complete file is uploaded.</span></span>
<span data-ttu-id="64759-124">Depois que o último byte do arquivo foram carregado a sessão de carregamento é concluída e o final do arquivo é mostrada na pasta de destino.</span><span class="sxs-lookup"><span data-stu-id="64759-124">Once the last byte of the file has been uploaded the upload session is completed and the final file is shown in the destination folder.</span></span>
<span data-ttu-id="64759-125">Como alternativa, você pode adiar final criação do arquivo no destino até que você faça explicitamente uma solicitação para completar o carregamento, definindo o `deferCommit` propriedade nos argumentos solicitação.</span><span class="sxs-lookup"><span data-stu-id="64759-125">Alternatively, you can defer final creation of the file in the destination until you explicitly make a request to complete the upload, by setting the `deferCommit` property in the request arguments.</span></span>

### <a name="http-request"></a><span data-ttu-id="64759-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64759-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createUploadSession
POST /groups/{groupId}/drive/items/{itemId}/createUploadSession
POST /me/drive/items/{itemId}/createUploadSession
POST /sites/{siteId}/drive/items/{itemId}/createUploadSession
POST /users/{userId}/drive/items/{itemId}/createUploadSession
```

### <a name="request-body"></a><span data-ttu-id="64759-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64759-127">Request body</span></span>

<span data-ttu-id="64759-128">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64759-128">No request body is required.</span></span>
<span data-ttu-id="64759-129">No entanto, você pode especificar propriedades no corpo da solicitação, fornecendo dados adicionais sobre o arquivo que está sendo carregado e personalizando a semântica da operação de carregamento.</span><span class="sxs-lookup"><span data-stu-id="64759-129">However, you can specify properties in the request body providing additional data about the file being uploaded and customizing the semantics of the upload operation.</span></span>

<span data-ttu-id="64759-130">Por exemplo, o `item` propriedade permite definir os seguintes parâmetros:<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.driveItemUploadableProperties" } --></span><span class="sxs-lookup"><span data-stu-id="64759-130">For example, the `item` property allows setting the following parameters: <!-- { "blockType": "resource", "@odata.type": "microsoft.graph.driveItemUploadableProperties" } --></span></span>
```json
{
  "@microsoft.graph.conflictBehavior": "rename | fail | overwrite",
  "description": "description",
  "name": "filename.txt"
}
```

<span data-ttu-id="64759-131">O exemplo a seguir controla o comportamento se o nome do arquivo já é utilizado e também especifica que o final do arquivo não deve ser criada até que seja feita a uma solicitação de conclusão explícita:</span><span class="sxs-lookup"><span data-stu-id="64759-131">The following example controls the behavior if the filename is already taken, and also specifies that the final file should not be created until an explicit completion request is made:</span></span>

<!-- { "blockType": "ignored" } -->
```json
{
  "item": {
    "@microsoft.graph.conflictBehavior": "rename"
  },
  "deferCommit": true
}
```

### <a name="optional-request-headers"></a><span data-ttu-id="64759-132">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="64759-132">Optional request headers</span></span>

| <span data-ttu-id="64759-133">Nome</span><span class="sxs-lookup"><span data-stu-id="64759-133">Name</span></span>       | <span data-ttu-id="64759-134">Valor</span><span class="sxs-lookup"><span data-stu-id="64759-134">Value</span></span> | <span data-ttu-id="64759-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="64759-135">Description</span></span>                                                                                                                                                            |
|:-----------|:------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="64759-136">*if-match*</span><span class="sxs-lookup"><span data-stu-id="64759-136">*if-match*</span></span> | <span data-ttu-id="64759-137">etag</span><span class="sxs-lookup"><span data-stu-id="64759-137">etag</span></span>  | <span data-ttu-id="64759-138">Se esse cabeçalho de solicitação for incluído e a eTag (ou cTag) fornecida não corresponder à eTag atual no item, uma resposta de erro `412 Precondition Failed` será retornada.</span><span class="sxs-lookup"><span data-stu-id="64759-138">If this request header is included and the eTag (or cTag) provided does not match the current etag on the item, a `412 Precondition Failed` error response is returned.</span></span> |

## <a name="parameters"></a><span data-ttu-id="64759-139">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="64759-139">Parameters</span></span>

| <span data-ttu-id="64759-140">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="64759-140">Parameter</span></span>            | <span data-ttu-id="64759-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="64759-141">Type</span></span>                          | <span data-ttu-id="64759-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="64759-142">Description</span></span>
|:---------------------|:------------------------------|:---------------------------------
| <span data-ttu-id="64759-143">item</span><span class="sxs-lookup"><span data-stu-id="64759-143">item</span></span>                 | <span data-ttu-id="64759-144">driveItemUploadableProperties</span><span class="sxs-lookup"><span data-stu-id="64759-144">driveItemUploadableProperties</span></span> | <span data-ttu-id="64759-145">Dados sobre o arquivo que está sendo carregado</span><span class="sxs-lookup"><span data-stu-id="64759-145">Data about the file being uploaded</span></span>
| <span data-ttu-id="64759-146">deferCommit</span><span class="sxs-lookup"><span data-stu-id="64759-146">deferCommit</span></span>          | <span data-ttu-id="64759-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="64759-147">Boolean</span></span>                       | <span data-ttu-id="64759-148">Se definido como true, final de criação do arquivo no destino exigirá uma solicitação explícita.</span><span class="sxs-lookup"><span data-stu-id="64759-148">If set to true, final creation of the file in the destination will require an explicit request.</span></span> <span data-ttu-id="64759-149">Somente em OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="64759-149">Only on OneDrive for Business.</span></span>

## <a name="item-properties"></a><span data-ttu-id="64759-150">Propriedades do item</span><span class="sxs-lookup"><span data-stu-id="64759-150">Item properties</span></span>

| <span data-ttu-id="64759-151">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64759-151">Property</span></span>             | <span data-ttu-id="64759-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="64759-152">Type</span></span>               | <span data-ttu-id="64759-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="64759-153">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="64759-154">description</span><span class="sxs-lookup"><span data-stu-id="64759-154">description</span></span>          | <span data-ttu-id="64759-155">String</span><span class="sxs-lookup"><span data-stu-id="64759-155">String</span></span>             | <span data-ttu-id="64759-156">Fornece uma descrição do usuário visíveis do item.</span><span class="sxs-lookup"><span data-stu-id="64759-156">Provides a user-visible description of the item.</span></span> <span data-ttu-id="64759-157">Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="64759-157">Read-write.</span></span> <span data-ttu-id="64759-158">Somente em OneDrive pessoal.</span><span class="sxs-lookup"><span data-stu-id="64759-158">Only on OneDrive Personal.</span></span>
| <span data-ttu-id="64759-159">name</span><span class="sxs-lookup"><span data-stu-id="64759-159">name</span></span>                 | <span data-ttu-id="64759-160">String</span><span class="sxs-lookup"><span data-stu-id="64759-160">String</span></span>             | <span data-ttu-id="64759-p108">O nome do item (nome do arquivo e extensão). Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="64759-p108">The name of the item (filename and extension). Read-write.</span></span>

### <a name="request"></a><span data-ttu-id="64759-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64759-163">Request</span></span>

<span data-ttu-id="64759-164">A resposta a essa solicitação fornecerá os detalhes da [uploadSession](../resources/uploadsession.md) recém-criada, que inclui a URL usada para carregar as partes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="64759-164">The response to this request will provide the details of the newly created [uploadSession](../resources/uploadsession.md), which includes the URL used for uploading the parts of the file.</span></span> 

<!-- { "blockType": "request", "name": "upload-fragment-create-session", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drive/root:/{item-path}:/createUploadSession
Content-Type: application/json

{
  "item": {
    "@odata.type": "microsoft.graph.driveItemUploadableProperties",
    "@microsoft.graph.conflictBehavior": "rename",
    "name": "largefile.dat"
  }
}
```

### <a name="response"></a><span data-ttu-id="64759-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="64759-165">Response</span></span>

<span data-ttu-id="64759-166">A resposta a essa solicitação, se tiver êxito, fornecerá os detalhes sobre o local para onde o restante das solicitações deve ser enviado como um recurso [UploadSession](../resources/uploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="64759-166">The response to this request, if successful, will provide the details for where the remainder of the requests should be sent as an [UploadSession](../resources/uploadsession.md) resource.</span></span>

<span data-ttu-id="64759-167">Esse recurso fornece detalhes sobre onde o intervalo de bytes do arquivo deve ser carregado e quando a sessão de carregamento expira.</span><span class="sxs-lookup"><span data-stu-id="64759-167">This resource provides details about where the byte range of the file should be uploaded and when the upload session expires.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession",
       "optionalProperties": [ "nextExpectedRanges" ]  } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "uploadUrl": "https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337",
  "expirationDateTime": "2015-01-29T09:21:55.523Z"
}
```

## <a name="upload-bytes-to-the-upload-session"></a><span data-ttu-id="64759-168">Carregar bytes na sessão de carregamento</span><span class="sxs-lookup"><span data-stu-id="64759-168">Upload bytes to the upload session</span></span>

<span data-ttu-id="64759-169">Para carregar o arquivo, ou uma parte do arquivo, o aplicativo faz uma solicitação PUT ao valor de **uploadUrl** recebido na resposta de **createUploadSession**.</span><span class="sxs-lookup"><span data-stu-id="64759-169">To upload the file, or a portion of the file, your app makes a PUT request to the **uploadUrl** value received in the **createUploadSession** response.</span></span>
<span data-ttu-id="64759-170">Você pode carregar o arquivo inteiro ou dividi-lo em vários intervalos de byte, desde que o máximo de bytes em qualquer solicitação específica seja menor que 60 MiB.</span><span class="sxs-lookup"><span data-stu-id="64759-170">You can upload the entire file, or split the file into multiple byte ranges, as long as the maximum bytes in any given request is less than 60 MiB.</span></span>

<span data-ttu-id="64759-171">Os fragmentos do arquivo devem ser carregados sequencialmente na ordem.</span><span class="sxs-lookup"><span data-stu-id="64759-171">The fragments of the file must be uploaded sequentially in order.</span></span>
<span data-ttu-id="64759-172">O upload de fragmentos fora de ordem resultará em um erro.</span><span class="sxs-lookup"><span data-stu-id="64759-172">Uploading fragments out of order will result in an error.</span></span>

<span data-ttu-id="64759-173">**Observação:** se seu aplicativo dividir um arquivo em vários intervalos de byte, o tamanho de cada intervalo de bytes **DEVE** ser um múltiplo de 320 KiB (327.680 bytes).</span><span class="sxs-lookup"><span data-stu-id="64759-173">**Note:** If your app splits a file into multiple byte ranges, the size of each byte range **MUST** be a multiple of 320 KiB (327,680 bytes).</span></span> <span data-ttu-id="64759-174">Usar um tamanho de fragmento que não divide uniformemente por 320 KiB resultará em erros ao confirmar alguns arquivos.</span><span class="sxs-lookup"><span data-stu-id="64759-174">Using a fragment size that does not divide evenly by 320 KiB will result in errors committing some files.</span></span>

### <a name="example"></a><span data-ttu-id="64759-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64759-175">Example</span></span>

<span data-ttu-id="64759-176">Neste exemplo, o aplicativo está carregando os primeiros 26 bytes de um arquivo de 128 bytes.</span><span class="sxs-lookup"><span data-stu-id="64759-176">In this example, the app is uploading the first 26 bytes of a 128 byte file.</span></span>

* <span data-ttu-id="64759-177">O cabeçalho **Content-Length** especifica o tamanho da solicitação atual.</span><span class="sxs-lookup"><span data-stu-id="64759-177">The **Content-Length** header specifies the size of the current request.</span></span>
* <span data-ttu-id="64759-178">O cabeçalho **Content-Range** indica o intervalo de bytes no arquivo geral que essa solicitação representa.</span><span class="sxs-lookup"><span data-stu-id="64759-178">The **Content-Range** header indicates the range of bytes in the overall file that this request represents.</span></span>
* <span data-ttu-id="64759-179">O tamanho total do arquivo precisa ser conhecido antes que você possa carregar seu primeiro fragmento.</span><span class="sxs-lookup"><span data-stu-id="64759-179">The total length of the file is known before you can upload the first fragment of the file.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-piece", "scopes": "files.readwrite" } -->

```http
PUT https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
Content-Length: 26
Content-Range: bytes 0-25/128

<bytes 0-25 of the file>
```

<span data-ttu-id="64759-180">**Importante:** seu aplicativo deve garantir que o tamanho total do arquivo especificado no cabeçalho **Content-Range** seja o mesmo para todas as solicitações.</span><span class="sxs-lookup"><span data-stu-id="64759-180">**Important:** Your app must ensure the total file size specified in the **Content-Range** header is the same for all requests.</span></span>
<span data-ttu-id="64759-181">Se um intervalo de bytes declarar um tamanho de arquivo diferente, a solicitação falhará.</span><span class="sxs-lookup"><span data-stu-id="64759-181">If a byte range declares a different file size, the request will fail.</span></span>

### <a name="response"></a><span data-ttu-id="64759-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="64759-182">Response</span></span>

<span data-ttu-id="64759-183">Quando a solicitação for concluída, o servidor responderá com `202 Accepted` se houver mais intervalos de bytes que precisem ser carregados.</span><span class="sxs-lookup"><span data-stu-id="64759-183">When the request is complete, the server will respond with `202 Accepted` if there are more byte ranges that need to be uploaded.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["26-"]
}
```

<span data-ttu-id="64759-184">O aplicativo pode usar o valor de **nextExpectedRanges** para determinar onde iniciar o próximo intervalo de bytes.</span><span class="sxs-lookup"><span data-stu-id="64759-184">Your app can use the **nextExpectedRanges** value to determine where to start the next byte range.</span></span>
<span data-ttu-id="64759-185">É possível ver vários intervalos especificados, indicando partes do arquivo que o servidor ainda não recebeu.</span><span class="sxs-lookup"><span data-stu-id="64759-185">You may see multiple ranges specified, indicating parts of the file that the server has not yet received.</span></span> <span data-ttu-id="64759-186">Isso é útil quando você precisa retomar uma transferência que foi interrompida, e seu cliente não tem certeza sobre o estado do serviço.</span><span class="sxs-lookup"><span data-stu-id="64759-186">This is useful if you need to resume a transfer that was interrupted and your client is unsure of the state on the service.</span></span>

<span data-ttu-id="64759-187">Você sempre deve determinar o tamanho dos intervalos de byte de acordo com as práticas recomendadas a seguir.</span><span class="sxs-lookup"><span data-stu-id="64759-187">You should always determine the size of your byte ranges according to the best practices below.</span></span> <span data-ttu-id="64759-188">Não suponha que **nextExpectedRanges** retornará intervalos de tamanho apropriado para carregar um intervalo de bytes.</span><span class="sxs-lookup"><span data-stu-id="64759-188">Do not assume that **nextExpectedRanges** will return reanges of proper size for a byte range to upload.</span></span>
<span data-ttu-id="64759-189">A propriedade **nextExpectedRanges** indica intervalos do arquivo que não foram recebidos, e não um padrão para como seu aplicativo deve carregar o arquivo.</span><span class="sxs-lookup"><span data-stu-id="64759-189">The **nextExpectedRanges** property indicates ranges of the file that have not been received and not a pattern for how your app should upload the file.</span></span>

<!-- { "blockType": "ignored", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": [
  "12345-55232",
  "77829-99375"
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="64759-190">Comentários</span><span class="sxs-lookup"><span data-stu-id="64759-190">Remarks</span></span>

* <span data-ttu-id="64759-191">A propriedade `nextExpectedRanges` nem sempre listará todos os intervalos ausentes.</span><span class="sxs-lookup"><span data-stu-id="64759-191">The `nextExpectedRanges` property won't always list all of the missing ranges.</span></span>
* <span data-ttu-id="64759-p115">Em gravações de fragmento bem-sucedidas, ela retornará o próximo intervalo do qual começar (ex: "523-").</span><span class="sxs-lookup"><span data-stu-id="64759-p115">On successful fragment writes, it will return the next range to start from (eg. "523-").</span></span>
* <span data-ttu-id="64759-p116">Em falhas quando o cliente enviou um fragmento que o servidor já havia recebido, o servidor responderá com `HTTP 416 Requested Range Not Satisfiable`. Você pode [solicitar o status do upload](#resuming-an-in-progress-upload) para obter uma lista mais detalhada dos intervalos que estão faltando.</span><span class="sxs-lookup"><span data-stu-id="64759-p116">On failures when the client sent a fragment the server had already received, the server will respond with `HTTP 416 Requested Range Not Satisfiable`. You can [request upload status](#resuming-an-in-progress-upload) to get a more detailed list of missing ranges.</span></span>
* <span data-ttu-id="64759-p117">Incluindo o cabeçalho de autorização, fazer a chamada de `PUT` pode resultar em uma resposta `HTTP 401 Unauthorized`. O cabeçalho de autorização e o token de portador só devem ser enviados ao emitir o `POST` durante a primeira etapa. Não deve ser incluído ao emitir o `PUT`.</span><span class="sxs-lookup"><span data-stu-id="64759-p117">Including the Authorization header when issuing the `PUT` call may result in a `HTTP 401 Unauthorized` response. The Authorization header and bearer token should only be sent when issuing the `POST` during the first step. It should be not be included when issueing the `PUT`.</span></span>

## <a name="completing-a-file"></a><span data-ttu-id="64759-199">Concluir um arquivo</span><span class="sxs-lookup"><span data-stu-id="64759-199">Completing a file</span></span>

<span data-ttu-id="64759-200">Se `deferCommit` for falso ou não definidas, e depois o carregamento é preenchido automaticamente quando o intervalo de bytes final do arquivo é COLOCADO para a URL de carregamento.</span><span class="sxs-lookup"><span data-stu-id="64759-200">If `deferCommit` is false or unset, then the upload is automatically completed when the final byte range of the file is PUT to the upload URL.</span></span>
<span data-ttu-id="64759-201">Se `deferCommit` seja verdadeira, após o intervalo de bytes final do arquivo for COLOCADO para a URL de carregamento, o carregamento deve ser concluído explicitamente por uma solicitação POST final para o carregamento url com conteúdo de comprimento zero.</span><span class="sxs-lookup"><span data-stu-id="64759-201">If `deferCommit` is true, then after the final byte range of the file is PUT to the upload URL, the upload should be explicitly completed by a final POST request to the upload url with zero-length content.</span></span>

<span data-ttu-id="64759-202">Quando o carregamento é concluído, o servidor responderá à solicitação final com um `HTTP 201 Created` ou `HTTP 200 OK`.</span><span class="sxs-lookup"><span data-stu-id="64759-202">When the upload is completed, the server will respond to the final request with an `HTTP 201 Created` or `HTTP 200 OK`.</span></span>
<span data-ttu-id="64759-203">O corpo da resposta também incluirá o conjunto de propriedades padrão para o **driveItem** que representa o arquivo concluído.</span><span class="sxs-lookup"><span data-stu-id="64759-203">The response body will also include the default property set for the **driveItem** representing the completed file.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-final", "scopes": "files.readwrite" } -->

```
PUT https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
Content-Length: 21
Content-Range: bytes 101-127/128

<final bytes of the file>
```

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "912310013A123",
  "name": "largefile.vhd",
  "size": 128,
  "file": { }
}
```


<!-- { "blockType": "request", "opaqueUrl": true, "name": "commit-upload", "scopes": "files.readwrite" } -->

```
POST https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
Content-Length: 0
```

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "912310013A123",
  "name": "largefile.vhd",
  "size": 128,
  "file": { }
}
```

## <a name="handling-upload-conflicts"></a><span data-ttu-id="64759-204">Tratamento de conflitos de carregamento</span><span class="sxs-lookup"><span data-stu-id="64759-204">Handling upload conflicts</span></span>

<span data-ttu-id="64759-205">Se ocorrer um conflito depois do carregamento do arquivo (por exemplo, um item com o mesmo nome foi criado durante a sessão de carregamento), será retornado um erro quando o último intervalo de bytes for carregado.</span><span class="sxs-lookup"><span data-stu-id="64759-205">If a conflict occurs after the file is uploaded (for example, an item with the same name was created during the upload session), an error is returned when the last byte range is uploaded.</span></span>

```http
HTTP/1.1 409 Conflict
Content-Type: application/json

{
  "error":
  {
    "code": "upload_name_conflict",
    "message": "Another file exists with the same name as the uploaded session. You can redirect the upload session to use a new filename by calling PUT with the new metadata and @microsoft.graph.sourceUrl attribute.",
  }
}
```

## <a name="cancel-the-upload-session"></a><span data-ttu-id="64759-206">Cancelar a sessão de carregamento</span><span class="sxs-lookup"><span data-stu-id="64759-206">Cancel the upload session</span></span>

<span data-ttu-id="64759-p120">Para cancelar uma sessão de upload, envie uma solicitação DELETE para a URL de upload. Isso limpa o arquivo temporário que contém os dados anteriormente carregados. Isso deve ser usado em cenários em que o upload é interrompido, por exemplo, se o usuário cancelar a transferência.</span><span class="sxs-lookup"><span data-stu-id="64759-p120">To cancel an upload session send a DELETE request to the upload URL. This cleans up the temporary file holding the data previously uploaded. This should be used in scenarios where the upload is aborted, for example, if the user cancels the transfer.</span></span>

<span data-ttu-id="64759-210">Os arquivos temporários e a sessão de carregamento que os acompanha são automaticamente limpos decorrido o valor de **expirationDateTime**.</span><span class="sxs-lookup"><span data-stu-id="64759-210">Temporary files and their accompanying upload session are automatically cleaned up after the **expirationDateTime** has passed.</span></span>
<span data-ttu-id="64759-211">Arquivos temporários não podem ser excluídos imediatamente após o período de expiração.</span><span class="sxs-lookup"><span data-stu-id="64759-211">Temporary files may not be deleted immedately after the expiration time has elapsed.</span></span>

### <a name="request"></a><span data-ttu-id="64759-212">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64759-212">Request</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-cancel", "scopes": "files.readwrite" } -->

```http
DELETE https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
```

### <a name="response"></a><span data-ttu-id="64759-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="64759-213">Response</span></span>

<span data-ttu-id="64759-214">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="64759-214">The following example shows the response.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

## <a name="resuming-an-in-progress-upload"></a><span data-ttu-id="64759-215">Retomando um upload em andamento</span><span class="sxs-lookup"><span data-stu-id="64759-215">Resuming an in-progress upload</span></span>

<span data-ttu-id="64759-p122">Se uma solicitação de upload for desconectada ou falhar antes de ser concluída, todos os seus bytes serão ignorados. Isso pode ocorrer quando a conexão entre seu aplicativo e o serviço é interrompida. Se isso ocorrer, seu aplicativo ainda poderá retomar a transferência do fragmento anteriormente concluído.</span><span class="sxs-lookup"><span data-stu-id="64759-p122">If an upload request is disconnected or fails before the request is completed, all bytes in that request are ignored. This can occur if the connection between your app and the service is dropped. If this occurs, your app can still resume the file transfer from the previously completed fragment.</span></span>

<span data-ttu-id="64759-219">Para descobrir quais intervalos de bytes foram recebidos anteriormente, seu aplicativo pode solicitar o status de uma sessão de upload.</span><span class="sxs-lookup"><span data-stu-id="64759-219">To find out which byte ranges have been received previously, your app can request the status of an upload session.</span></span>

### <a name="example"></a><span data-ttu-id="64759-220">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64759-220">Example</span></span>

<span data-ttu-id="64759-221">Confira o status do upload enviando uma solicitação GET para `uploadUrl`.</span><span class="sxs-lookup"><span data-stu-id="64759-221">Query the status of the upload by sending a GET request to the `uploadUrl`.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->

```
GET https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF86633784148bb98a1zjcUhf7b0mpUadahs
```

<span data-ttu-id="64759-222">O servidor responderá com uma lista de intervalos de bytes ausentes que precisam ser carregados e com a hora de expiração da sessão de upload.</span><span class="sxs-lookup"><span data-stu-id="64759-222">The server will respond with a list of missing byte ranges that need to be uploaded and the expiration time for the upload session.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["12345-"]
}
```

### <a name="upload-remaining-data"></a><span data-ttu-id="64759-223">Carregar os dados restantes</span><span class="sxs-lookup"><span data-stu-id="64759-223">Upload remaining data</span></span>

<span data-ttu-id="64759-224">Agora que o seu aplicativo sabe de onde começar o upload, retome o upload seguindo as etapas em [Carregar bytes na sessão de upload](#upload-bytes-to-the-upload-session).</span><span class="sxs-lookup"><span data-stu-id="64759-224">Now that your app knows where to start the upload from, resume the upload by following the steps in [upload bytes to the upload session](#upload-bytes-to-the-upload-session).</span></span>

## <a name="handle-upload-errors"></a><span data-ttu-id="64759-225">Tratar erros de carregamento</span><span class="sxs-lookup"><span data-stu-id="64759-225">Handle upload errors</span></span>

<span data-ttu-id="64759-226">Quando o último intervalo de bytes de um arquivo for carregado, talvez ocorra um erro.</span><span class="sxs-lookup"><span data-stu-id="64759-226">When the last byte range of a file is uploaded, it is possible for an error to occur.</span></span> <span data-ttu-id="64759-227">Isso pode acontecer devido a um conflito de nomes ou a uma limitação de cota excedida.</span><span class="sxs-lookup"><span data-stu-id="64759-227">This can be due to a name conflict or quota limitation being exceeded.</span></span>
<span data-ttu-id="64759-228">A sessão de carregamento será preservada até a expiração, o que permite que seu aplicativo recupere o carregamento confirmando explicitamente a sessão de carregamento.</span><span class="sxs-lookup"><span data-stu-id="64759-228">The upload session will be preserved until the expiration time, which allows your app to recover the upload by explicitly committing the upload session.</span></span>

<span data-ttu-id="64759-229">Para confirmar manualmente a sessão de carregamento, o aplicativo deve fazer uma solicitação PUT com um novo recurso **driveItem**, que será usado ao confirmar a sessão de carregamento.</span><span class="sxs-lookup"><span data-stu-id="64759-229">To explicitly commit the upload session, your app must make a PUT request with a new **driveItem** resource that will be used when committing the upload session.</span></span>
<span data-ttu-id="64759-230">Essa nova solicitação deve corrigir a origem do erro que gerou o erro de carregamento original.</span><span class="sxs-lookup"><span data-stu-id="64759-230">This new request should correct the source of error that generated the original upload error.</span></span>

<span data-ttu-id="64759-231">Para indicar que o aplicativo está confirmando uma sessão de carregamento existente, a solicitação PUT deve incluir a propriedade `@microsoft.graph.sourceUrl` com o valor de sua URL de sessão de carregamento.</span><span class="sxs-lookup"><span data-stu-id="64759-231">To indicate that your app is committing an existing upload session, the PUT request must include the `@microsoft.graph.sourceUrl` property with the value of your upload session URL.</span></span>

<!-- { "blockType": "ignored", "name": "explicit-upload-commit", "scopes": "files.readwrite", "tags": "service.graph" } -->

```http
PUT /me/drive/root:/{path_to_parent}
Content-Type: application/json
If-Match: {etag or ctag}

{
  "name": "largefile.vhd",
  "@microsoft.graph.conflictBehavior": "rename",
  "@microsoft.graph.sourceUrl": "{upload session URL}"
}
```

<span data-ttu-id="64759-232">**Observação:** você pode usar os cabeçalhos `@microsoft.graph.conflictBehavior` e `if-match` conforme esperado nessa chamada.</span><span class="sxs-lookup"><span data-stu-id="64759-232">**Note:** You can use the `@microsoft.graph.conflictBehavior` and `if-match` headers as expected in this call.</span></span>

### <a name="response"></a><span data-ttu-id="64759-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="64759-233">Response</span></span>

<span data-ttu-id="64759-234">Se o arquivo puder ser confirmado usando os novos metadados, uma resposta `HTTP 201 Created` ou `HTTP 200 OK` será retornada com os metadados de Item para o arquivo carregado.</span><span class="sxs-lookup"><span data-stu-id="64759-234">If the file can be committed using the new metadata, an `HTTP 201 Created` or `HTTP 200 OK` response will be returned with the Item metadata for the uploaded file.</span></span>

<!-- { "blockType": "ignored", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "912310013A123",
  "name": "largefile.vhd",
  "size": 128,
  "file": { }
}
```

## <a name="best-practices"></a><span data-ttu-id="64759-235">Práticas recomendadas</span><span class="sxs-lookup"><span data-stu-id="64759-235">Best practices</span></span>

* <span data-ttu-id="64759-236">Retome ou repita uploads que falharam devido a interrupções de conexão ou erros 5xx, como:</span><span class="sxs-lookup"><span data-stu-id="64759-236">Resume or retry uploads that fail due to connection interruptions or any 5xx errors, including:</span></span>
  * `500 Internal Server Error`
  * `502 Bad Gateway`
  * `503 Service Unavailable`
  * `504 Gateway Timeout`
* <span data-ttu-id="64759-237">Use uma estratégia de retirada exponencial se erros de servidor 5xx forem retornados ao retomar ou repetir solicitações de upload.</span><span class="sxs-lookup"><span data-stu-id="64759-237">Use an exponential back off strategy if any 5xx server errors are returned when resuming or retrying upload requests.</span></span>
* <span data-ttu-id="64759-238">Para outros erros, você não deve usar uma estratégia de retirada exponencial, mas sim limitar o número de tentativas de repetição feitas.</span><span class="sxs-lookup"><span data-stu-id="64759-238">For other errors, you should not use an exponential back off strategy but limit the number of retry attempts made.</span></span>
* <span data-ttu-id="64759-239">Lide com erros `404 Not Found` ao fazer carregamentos retomáveis reiniciando todo o carregamento.</span><span class="sxs-lookup"><span data-stu-id="64759-239">Handle `404 Not Found` errors when doing resumable uploads by starting the entire upload over.</span></span> <span data-ttu-id="64759-240">Isso indica que a sessão de carregamento não existe mais.</span><span class="sxs-lookup"><span data-stu-id="64759-240">This indicates the upload session no longer exists.</span></span>
* <span data-ttu-id="64759-241">Use transferências de arquivos retomáveis para arquivos com mais de 10 MiB (10.485.760 bytes).</span><span class="sxs-lookup"><span data-stu-id="64759-241">Use resumable file transfers for files larger than 10 MiB (10,485,760 bytes).</span></span>
* <span data-ttu-id="64759-242">Um tamanho de intervalo de bytes de 10 MiB para conexões estáveis de alta velocidade é ideal.</span><span class="sxs-lookup"><span data-stu-id="64759-242">A byte range size of 10 MiB for stable high speed connections is optimal.</span></span> <span data-ttu-id="64759-243">Para conexões mais lentas ou menos confiáveis, você pode obter melhores resultados com um tamanho de fragmento menor.</span><span class="sxs-lookup"><span data-stu-id="64759-243">For slower or less reliable connections you may get better results from a smaller fragment size.</span></span> <span data-ttu-id="64759-244">O tamanho do fragmento recomendado é entre 5 MiB e 10 MiB.</span><span class="sxs-lookup"><span data-stu-id="64759-244">The recommended fragment size is between 5-10 MiB.</span></span>
* <span data-ttu-id="64759-245">Use um tamanho de intervalo de bytes que seja múltiplo de 320 KiB (327.680 bytes).</span><span class="sxs-lookup"><span data-stu-id="64759-245">Use a byte range size that is a multiple of 320 KiB (327,680 bytes).</span></span> <span data-ttu-id="64759-246">Uma falha ao usar um tamanho de fragmento que seja múltiplo de 320 KiB pode resultar na falha de transferências de arquivos grandes após o carregamento do último intervalo de bytes.</span><span class="sxs-lookup"><span data-stu-id="64759-246">Failing to use a fragment size that is a multiple of 320 KiB can result in large file transfers failing after the last byte range is uploaded.</span></span>

## <a name="error-responses"></a><span data-ttu-id="64759-247">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="64759-247">Error responses</span></span>

<span data-ttu-id="64759-248">Confira o tópico [Respostas de erro][error-response] para saber detalhes sobre como os erros são retornados.</span><span class="sxs-lookup"><span data-stu-id="64759-248">See the [Error Responses][error-response] topic for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Upload large files using an upload session.",
  "keywords": "upload,large file,fragment,BITS",
  "section": "documentation"
} -->
