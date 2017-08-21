# <a name="upload-large-files-with-an-upload-session"></a><span data-ttu-id="1e1b0-101">Carregar arquivos grandes com uma sessão de upload</span><span class="sxs-lookup"><span data-stu-id="1e1b0-101">Upload large files with an upload session</span></span>

<span data-ttu-id="1e1b0-p101">Crie uma sessão de upload para permitir que seu aplicativo carregue arquivos até o tamanho máximo de arquivo. Uma sessão de upload permite que seu aplicativo carregue intervalos do arquivo em solicitações de API sequenciais, permitindo que a transferência seja retomada se uma conexão for interrompida enquanto o upload estiver em andamento.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-p101">Create an upload session to allow your app to upload files up to the maximum file size. An upload session allows your app to upload ranges of the file in sequental API requests, which allows the transfer to be resumed if a connection is dropped while the upload is in progress.</span></span>

<span data-ttu-id="1e1b0-104">Para carregar um arquivo usando uma sessão de upload, duas etapas são obrigatórias:</span><span class="sxs-lookup"><span data-stu-id="1e1b0-104">To upload a file using an upload session, there are two steps:</span></span>

1. [<span data-ttu-id="1e1b0-105">Criar uma sessão de upload</span><span class="sxs-lookup"><span data-stu-id="1e1b0-105">Create an upload session</span></span>](#create-an-upload-session)
2. [<span data-ttu-id="1e1b0-106">Carregar bytes na sessão de upload</span><span class="sxs-lookup"><span data-stu-id="1e1b0-106">Upload bytes to the upload session</span></span>](#upload-bytes-to-the-upload-session)

## <a name="prerequisites"></a><span data-ttu-id="1e1b0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1e1b0-107">Prerequisites</span></span>
<span data-ttu-id="1e1b0-108">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="1e1b0-108">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="1e1b0-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e1b0-109">Files.ReadWrite</span></span>
* <span data-ttu-id="1e1b0-110">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e1b0-110">Files.ReadWrite.All</span></span>
* <span data-ttu-id="1e1b0-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e1b0-111">Sites.ReadWrite.All</span></span>

> <span data-ttu-id="1e1b0-p102">**Observação**: A permissão de aplicativo Files.ReadWrite.All ainda não tem suporte nessa API. O suporte completo está planejado para breve.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-p102">**Note**: The Files.ReadWrite.All application permission is not yet supported on this API. Full support is planned soon.</span></span> 

## <a name="create-an-upload-session"></a><span data-ttu-id="1e1b0-114">Criar uma sessão de upload</span><span class="sxs-lookup"><span data-stu-id="1e1b0-114">Create an upload session</span></span>

<span data-ttu-id="1e1b0-p103">Para iniciar o upload de um arquivo grande, seu aplicativo deve primeiro solicitar uma nova sessão de upload. Isso cria um local de armazenamento temporário no qual os bytes do arquivo serão salvos até que este seja totalmente carregado. Depois que o último byte do arquivo for carregado, a sessão de upload será concluída, e o arquivo final aparecerá na pasta de destino.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-p103">To begin a large file upload, your app must first request a new upload session. This creates a temporary storage location where the bytes of the file will be saved until the complete file is uploaded. Once the last byte of the file has been uploaded the upload session is completed and the final file is shown in the destination folder.</span></span>

### <a name="http-request"></a><span data-ttu-id="1e1b0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e1b0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root:/{path-to-item}:/createUploadSession
POST /me/drive/items/{parent-item-id}:/{filename}:/createUploadSession
```

### <a name="request-body"></a><span data-ttu-id="1e1b0-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e1b0-119">Request body</span></span>
<span data-ttu-id="1e1b0-p104">Nenhum corpo de solicitação é obrigatório. No entanto, você pode especificar um corpo de solicitação para fornecer dados adicionais sobre o arquivo que está sendo carregado.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-p104">No request body is required. However, you can specify a request body to provide additional data about the file being uploaded.</span></span>

<span data-ttu-id="1e1b0-122">Por exemplo, para controlar o comportamento se o nome do arquivo já estiver em uso, você pode especificar a propriedade de comportamento conflitante no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-122">For example, to control the behavior if the filename is already taken, you can specify the conflict behavior property in the body of the request.</span></span>

```json
{
    "item": {
        "@microsoft.graph.conflictBehavior": "rename"
    }
}
```

### <a name="optional-request-headers"></a><span data-ttu-id="1e1b0-123">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="1e1b0-123">Optional request headers</span></span>

| <span data-ttu-id="1e1b0-124">Nome</span><span class="sxs-lookup"><span data-stu-id="1e1b0-124">Name</span></span>       | <span data-ttu-id="1e1b0-125">Valor</span><span class="sxs-lookup"><span data-stu-id="1e1b0-125">Value</span></span> | <span data-ttu-id="1e1b0-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e1b0-126">Description</span></span>                                                                                                                                                            |
|:-----------|:------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="1e1b0-127">*if-match*</span><span class="sxs-lookup"><span data-stu-id="1e1b0-127">*if-match*</span></span> | <span data-ttu-id="1e1b0-128">etag</span><span class="sxs-lookup"><span data-stu-id="1e1b0-128">etag</span></span>  | <span data-ttu-id="1e1b0-129">Se esse cabeçalho de solicitação for incluído, e a eTag (ou cTag) fornecida não corresponder à etag atual no item, uma resposta de erro `412 Precondition Failed` será retornada.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-129">If this request header is included and the eTag (or cTag) provided does not match the current etag on the item, a `412 Precondition Failed` errr response is returned.</span></span> |


### <a name="response"></a><span data-ttu-id="1e1b0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e1b0-130">Response</span></span>
<span data-ttu-id="1e1b0-131">A resposta a essa solicitação fornecerá os detalhes da [uploadSession](../resources/uploadsession.md) recém-criada, que inclui a URL usada para carregar as partes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-131">The response to this request will provide the details of the newly created [uploadSession](../resources/uploadsession.md), which includes the URL used for uploading the parts of the file.</span></span> 

### <a name="example"></a><span data-ttu-id="1e1b0-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e1b0-132">Example</span></span>

<!-- {
  "blockType": "request",
  "name": "driveItem_createUploadSession"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root:/{item-path}:/createUploadSession
```

##### <a name="response"></a><span data-ttu-id="1e1b0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e1b0-133">Response</span></span> 

<span data-ttu-id="1e1b0-134">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-134">The following example shows the formula bar</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "uploadUrl": "https://tenant-my.sharepoint.com/alkjl1kjklna",
  "expirationDateTime": "2020-08-24T10:58:00Z",
  "nextExpectedRanges": ["0-"]
}
```

## <a name="upload-bytes-to-the-upload-session"></a><span data-ttu-id="1e1b0-135">Carregar bytes na sessão de upload</span><span class="sxs-lookup"><span data-stu-id="1e1b0-135">Upload bytes to the upload session</span></span>

<span data-ttu-id="1e1b0-p105">Para carregar o arquivo, ou uma parte do arquivo, o aplicativo faz uma solicitação PUT ao valor de **uploadUrl** recebido na de **createUploadSession**. Você pode carregar o arquivo inteiro ou dividi-lo em fragmentos, desde que o máximo de bytes em qualquer solicitação específica seja menor que 60 MiB. Os fragmentos do arquivo devem ser carregados sequencialmente em ordem. O upload de fragmentos fora de ordem resultará em um erro.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-p105">To upload the file, or a portion of the file, your app makes a PUT request to the **uploadUrl** value received in the **createUploadSession** response. You can upload the entire file, or split the file into fragments, as long as the maximum bytes in any given request is less than 60 MiB. The fragments of the file must be uploaded sequentally in order. Uploading fragments out of order will result in an error.</span></span>

<span data-ttu-id="1e1b0-p106">**Observação:** Se seu aplicativo dividir um arquivo em vários fragmentos, o tamanho de cada fragmento **DEVERÁ** ser um múltiplo de 320 KiB. Usar um tamanho de fragmento que não divide uniformemente por 320 resultará em erros ao confirmar alguns arquivos.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-p106">**Note:** If your app splits a file into multiple fragments, the size of each fragment **MUST** be a multiple of 320 KiB. Using a fragment size that does not divide evenly by 320 will result in errors committing some files.</span></span>

### <a name="example"></a><span data-ttu-id="1e1b0-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e1b0-142">Example</span></span>

<span data-ttu-id="1e1b0-p107">Este exemplo está carregando os primeiros 26 bytes de um arquivo 128 bytes. O cabeçalho **Content-Length** especifica o tamanho da solicitação atual. O cabeçalho **Content-Range** indica o intervalo de bytes no arquivo geral que essa solicitação representa. O tamanho total do arquivo deve ser conhecido antes que você possa carregar seu primeiro fragmento.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-p107">This example is uploading the first 26 bytes of a 128 byte file. The **Content-Length** header specifies the size of the current request. The **Content-Range** header indicates the range of bytes in the overall file that this request represents. The total length of the file must be known before you can upload the first fragment of the file.</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-piece", "scopes": "files.readwrite" } -->
```
PUT https://tenant-my.sharepoint.com/alkjl1kjklna
Content-Length: 26
Content-Range: bytes 0-25/128

<bytes 0-25 of the file>
```

<span data-ttu-id="1e1b0-p108">**Importante:** Seu aplicativo deve garantir que o tamanho total do arquivo especificado no cabeçalho **Content-Range** seja o mesmo para todas as solicitações. Se um fragmento declarar um tamanho de arquivo diferente, a solicitação falhará.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-p108">**Important:** Your app must ensure the total file size specified in the **Content-Range** header is the same for all requests. If a fragment declares a different file size, the request will fail.</span></span>

##### <a name="response"></a><span data-ttu-id="1e1b0-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e1b0-149">Response</span></span>

<span data-ttu-id="1e1b0-150">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-150">The following example shows the formula bar</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["26-"]
}
```

<span data-ttu-id="1e1b0-p109">O aplicativo pode usar o valor de **nextExpectedRanges** para determinar onde iniciar o próximo fragmento. É possível ver vários intervalos especificados, indicando partes do arquivo que o servidor ainda não recebeu. Isso é útil quando você precisa retomar uma transferência que foi interrompida, e seu cliente não tem certeza sobre o estado no serviço.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-p109">Your app can use the **nextExpectedRanges** value to determine where to start the next fragment. You may see multiple ranges specified, indicating parts of the file that the server has not yet received. This is useful if you need to resume a transfer that was interrupted and your client is unsure of the state on the service.</span></span>

<span data-ttu-id="1e1b0-p110">Você sempre deve determinar o tamanho do fragmento de acordo com as práticas recomendadas a seguir. Não suponha que **nextExpectedRanges** retornará intervalos de tamanho apropriado para um fragmento de upload. A propriedade **nextExpectedRanges** indica intervalos do arquivo que não foram recebidos, e não um padrão para como você deve carregar esse arquivo.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-p110">You should always determine the fragment size according to the best practices below. Do not assume that **nextExpectedRanges** will return reanges of proper size for an upload fragment. The **nextExpectedRanges** property indicates ranges of the file that have not been received and not a pattern for how you should upload the file.</span></span>

<span data-ttu-id="1e1b0-157">**Observações:**</span><span class="sxs-lookup"><span data-stu-id="1e1b0-157">**Notes:**</span></span>

* <span data-ttu-id="1e1b0-158">A propriedade `nextExpectedRanges` nem sempre listará todos os intervalos ausentes.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-158">The `nextExpectedRanges` property won't always list all of the missing ranges.</span></span>
* <span data-ttu-id="1e1b0-p111">Em gravações de fragmento bem-sucedidas, ela retornará o próximo intervalo do qual começar (ex: "523-").</span><span class="sxs-lookup"><span data-stu-id="1e1b0-p111">On successful fragment writes, it will return the next range to start from (eg. "523-").</span></span>
* <span data-ttu-id="1e1b0-p112">Em falhas quando o cliente enviou um fragmento que o servidor já havia recebido, o servidor responderá com `HTTP 416 Requested Range Not Satisfiable`. Você pode [solicitar o status do upload](#resuming-an-in-progress-upload) para obter uma lista mais detalhada dos intervalos que estão faltando.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-p112">On failures when the client sent a fragment the server had already received, the server will respond with `HTTP 416 Requested Range Not Satisfiable`. You can [request upload status](#resuming-an-in-progress-upload) to get a more detailed list of missing ranges.</span></span>
* <span data-ttu-id="1e1b0-p113">Incluindo o cabeçalho de autorização, fazer a chamada de `PUT` pode resultar em uma resposta `HTTP 401 Unauthoized`. O cabeçalho de autorização e o token de portador só devem ser enviados ao emitir o `POST` durante a primeira etapa. Não deve ser incluído ao emitir o `PUT`.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-p113">Including the Authorization header when issuing the `PUT` call may result in a `HTTP 401 Unauthoized` response. The Authoization header and bearer token should only be sent when issueing the `POST` during the first step. It should be not be included when issueing the `PUT`.</span></span>   


## <a name="completing-a-file"></a><span data-ttu-id="1e1b0-166">Concluindo um arquivo</span><span class="sxs-lookup"><span data-stu-id="1e1b0-166">Completing a file</span></span>

<span data-ttu-id="1e1b0-p114">Quando o último fragmento de um arquivo for recebido, o servidor responderá com um `HTTP 201 Created` ou `HTTP 200 OK`. O corpo da resposta também incluirá o conjunto de propriedades padrão para o **driveItem** que representa o arquivo concluído.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-p114">When the last fragment of a file is received the server will response with an `HTTP 201 Created` or `HTTP 200 OK`. The response body will also include the default property set for the **driveItem** representing the completed file.</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-final", "scopes": "files.readwrite" } -->
```
PUT https://tenant-my.sharepoint.com/alkjl1kjklna
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
<span data-ttu-id="1e1b0-169">**Observação:** A resposta do item é truncada para clareza de documentação.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-169">**Note:** The item response is truncated for documentation clarity.</span></span>

## <a name="cancel-an-upload-session"></a><span data-ttu-id="1e1b0-170">Cancelar uma sessão de upload</span><span class="sxs-lookup"><span data-stu-id="1e1b0-170">Cancel an upload session</span></span>

<span data-ttu-id="1e1b0-p115">Para cancelar uma sessão de upload, envie uma solicitação DELETE para a URL de upload. Isso limpa o arquivo temporário que contém os dados anteriormente carregados. Isso deve ser usado em cenários em que o upload é interrompido, por exemplo, se o usuário cancelar a transferência.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-p115">To cancel an upload session send a DELETE request to the upload URL. This cleans up the temporary file holding the data previously uploaded. This should be used in scenarios where the upload is aborted, for example, if the user cancels the transfer.</span></span>

<span data-ttu-id="1e1b0-174">Os arquivos temporários e a sessão de upload que os acompanha são automaticamente limpos decorrido o valor de **expirationDateTime**.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-174">Temporary files and their accompanying upload session are automatically cleaned up after the **expirationDateTime** has passed.</span></span>

### <a name="example"></a><span data-ttu-id="1e1b0-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e1b0-175">Example</span></span>

<span data-ttu-id="1e1b0-176">A solicitação DELETE fará com que a sessão de upload expire imediatamente e removerá qualquer byte anteriormente carregado.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-176">The DELETE request will immedately expire the upload session and remove any previously uploaded bytes.</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-cancel", "scopes": "files.readwrite" } -->
```http
DELETE https://tenant-my.sharepoint.com/alkjl1kjklna
```

##### <a name="response"></a><span data-ttu-id="1e1b0-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e1b0-177">Response</span></span> 

<span data-ttu-id="1e1b0-178">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-178">The following example shows the formula bar</span></span>

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 204 No Content
```

## <a name="resuming-an-in-progress-upload"></a><span data-ttu-id="1e1b0-179">Retomando um upload em andamento</span><span class="sxs-lookup"><span data-stu-id="1e1b0-179">Resuming an in-progress upload</span></span>

<span data-ttu-id="1e1b0-p116">Se uma solicitação de upload for desconectada ou falhar antes de ser concluída, todos os seus bytes serão ignorados. Isso pode ocorrer quando a conexão entre seu aplicativo e o serviço é interrompida. Se isso ocorrer, seu aplicativo ainda poderá retomar a transferência do fragmento anteriormente concluído.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-p116">If an upload request is disconnected or fails before the request is completed, all bytes in that request are ignored. This can occur if the connection between your app and the service is dropped. If this occurs, your app can still resume the file transfer from the previously completed fragment.</span></span>

<span data-ttu-id="1e1b0-183">Para descobrir quais intervalos de bytes foram recebidos anteriormente, seu aplicativo pode solicitar o status de uma sessão de upload.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-183">To find out which byte ranges have been received previously, your app can request the status of an upload session.</span></span>

### <a name="example"></a><span data-ttu-id="1e1b0-184">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e1b0-184">Example</span></span>
<span data-ttu-id="1e1b0-185">Confira o status do upload enviando uma solicitação GET para `uploadUrl`.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-185">Query the status of the upload by sending a GET request to the `uploadUrl`.</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->
```
GET https://tenant-my.sharepoint.com/alkjl1kjklna
```

<span data-ttu-id="1e1b0-186">O servidor responderá com uma lista de intervalos de bytes ausentes que precisam ser carregados e com a hora de expiração da sessão de upload.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-186">The server will respond with a list of missing byte ranges that need to be uploaded and the expiration time for the upload session.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->
```http
HTTP/1.1 200 OK

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["12345-"]
}
```

### <a name="upload-remaining-data"></a><span data-ttu-id="1e1b0-187">Carregar os dados restantes</span><span class="sxs-lookup"><span data-stu-id="1e1b0-187">Upload remaining data</span></span>
<span data-ttu-id="1e1b0-188">Agora que o seu aplicativo sabe de onde começar o upload, retome o upload seguindo as etapas em [Carregar bytes na sessão de upload](#upload-bytes-to-the-upload-session).</span><span class="sxs-lookup"><span data-stu-id="1e1b0-188">Now that your app knows where to start the upload from, resume the upload by following the steps in [upload bytes to the upload session](#upload-bytes-to-the-upload-session).</span></span>


## <a name="best-practices"></a><span data-ttu-id="1e1b0-189">Práticas recomendadas</span><span class="sxs-lookup"><span data-stu-id="1e1b0-189">Best practices</span></span>

* <span data-ttu-id="1e1b0-190">Retome ou repita uploads que falharam devido a interrupções de conexão ou erros 5xx, como:</span><span class="sxs-lookup"><span data-stu-id="1e1b0-190">Resume or retry uploads that fail due to connection interruptions or any 5xx errors, including:</span></span>
  * `500 Internal Server Error`
  * `502 Bad Gateway`
  * `503 Service Unavailable`
  * `504 Gateway Timeout`
* <span data-ttu-id="1e1b0-191">Use uma estratégia de retirada exponencial se erros de servidor 5xx forem retornados ao retomar ou repetir solicitações de upload.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-191">Use an exponential back off strategy if any 5xx server errors are returned when resuming or retrying upload requests.</span></span>
* <span data-ttu-id="1e1b0-192">Para outros erros, você não deve usar uma estratégia de retirada exponencial, mas sim limitar o número de tentativas de repetição feitas.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-192">For other errors, you should not use an exponential back off strategy but limit the number of retry attempts made.</span></span>
* <span data-ttu-id="1e1b0-193">Lide com erros `404 Not Found` ao fazer uploads retomáveis reiniciando o upload inteiro.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-193">Handle `404 Not Found` errors when doing resumable uploads by starting the entire upload over.</span></span>
* <span data-ttu-id="1e1b0-194">Use transferências de arquivos retomáveis para arquivos com mais de 10 MiB (10 \* 1.024 \* 1.024 bytes).</span><span class="sxs-lookup"><span data-stu-id="1e1b0-194">Use resumable file transfers for files larger than 10 MiB (10 \* 1024 \* 1024 bytes).</span></span>
* <span data-ttu-id="1e1b0-p117">Um tamanho de fragmento de 10 MiB para conexões estável de alta velocidade é ideal. Para conexões mais lentas ou menos confiáveis, você pode obter melhores resultados com um tamanho de fragmento menor. O tamanho do fragmento recomendado é entre 5 e 10 MiB.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-p117">A fragment size of 10 MiB for stable high speed connections is optimal. For slower or less reliable connections you may get better results from a smaller fragment size. The recommended fragment size is between 5-10 MiB.</span></span>
* <span data-ttu-id="1e1b0-p118">Use um tamanho de fragmento que seja múltiplo de 320 KiB (320 \* 1.024 bytes). Uma falha ao usar um tamanho de fragmento que seja múltiplo de 320 KiB pode resultar na falha de transferências de arquivos grandes após o upload do último fragmento.</span><span class="sxs-lookup"><span data-stu-id="1e1b0-p118">Use a fragment size that is a multiple of 320 KiB (320 \* 1024 bytes). Failing to use a fragment size that is a multiple of 320 KiB can result in large file transfers failing after the last fragment is uploaded.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upload item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
