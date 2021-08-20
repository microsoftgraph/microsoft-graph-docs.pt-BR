---
title: Faça o upload de documentos utilizando a API de Impressão Universal do Microsoft Graph
description: A Impressão Universal é uma solução de impressão moderna que as organizações podem utilizar para gerenciar sua infraestrutura de impressão por meio de serviços em nuvem da Microsoft.
author: nilakhan
localization_priority: Priority
ms.prod: universal-print
ms.custom: scenarios:getting-started
ms.openlocfilehash: 78f876cdd2269dac9f9b68915f59d9ae2dd0b51d
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58265809"
---
# <a name="upload-documents-using-the-microsoft-graph-universal-print-api"></a>Faça o upload de documentos utilizando a API de Impressão Universal do Microsoft Graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../api-reference/includes/cloudprinting-pricing-disclaimer.md)]

Para imprimir um documento utilizando a API de Impressão Universal no Microsoft Graph, você [cria um trabalho de impressão](/graph/api/printershare-post-jobs), faz o upload do documento e, em seguida, [inicia o trabalho de impressão](/graph/api/printjob-start). Este artigo descreve como fazer o upload de um documento, que começa com [ a criação de uma sessão de upload ](/graph/api/printdocument-createuploadsession).

Para fazer o upload de um arquivo, ou de parte de um arquivo, seu aplicativo faz uma solicitação PUT para o valor **uploadUrl** recebido na resposta **createUploadSession**. Você pode fazer o upload de todo o arquivo ou dividi-lo em vários intervalos de bytes, desde que o máximo de bytes em qualquer solicitação seja inferior a 10 MB.

É possível fazer o upload dos segmentos do arquivo em qualquer ordem e o upload pode ser feito em paralelo, com até quatro solicitações simultâneas. Quando todos os segmentos binários de um documento são carregados, o arquivo binário é vinculado a **printDocument**.

## <a name="http-request"></a>Solicitação HTTP

Faça uma solicitação PUT para o valor **uploadUrl** recebido na resposta **createUploadSession**.

### <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição   |
|:--------------|:--------------|
| Intervalo do conteúdo | bytes {startByteIndex}-{endByteIndex}/{documentSizeInBytes}. Obrigatório.|
| Comprimento do Conteúdo | {contentLength} Obrigatório.|

### <a name="request-body"></a>Corpo da solicitação
O corpo da solicitação é um blob binário que contém os bytes do documento que são especificados como um intervalo de bytes **inclusivo** no cabeçalho `Content-Range`. 

### <a name="example"></a>Exemplo

```http
PUT https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}
Content-Range: bytes=0-72796/4533322
Content-Length: 72797

<bytes 0-72796 of the file>

```

Aqui, 0 e 72796 são os índices inicial e final do segmento de arquivo, e 4533322 é o tamanho do documento.
## <a name="http-response"></a>Resposta HTTP:

Quando a solicitação for concluída, o servidor responderá com `202 Accepted` se houver mais intervalos de bytes que precisem ser carregados.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
  "nextExpectedRanges": ["72797-4533321"]
}
```

O aplicativo pode usar o valor de **nextExpectedRanges** para determinar onde iniciar o próximo intervalo de bytes. Você pode ver vários intervalos especificados, indicando as partes do arquivo que o servidor ainda não recebeu. A propriedade **nextExpectedRanges** indica intervalos do arquivo que não foram recebidos, e não um padrão para como seu aplicativo deve carregar o arquivo.

<!-- { "blockType": "ignored", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
  "nextExpectedRanges": [
  "72797-72897",
  "78929-4533322"
  ]
}
```

### <a name="remarks"></a>Comentários

* Em falhas, quando o cliente envia um fragmento que o servidor já recebeu, o servidor responderá com `HTTP 416 Requested Range Not Satisfiable`. Você pode [solicitar o status de upload](#get-the-upload-session) para obter uma lista mais detalhada dos intervalos ausentes.
* A inclusão do cabeçalho de `Authorizatio` ao fazer a chamada `PUT` pode resultar em uma resposta `HTTP 401 Unauthorized`. O Cabeçalho de Autorização e o token de portador devem ser enviados apenas durante a criação da sessão de upload. Ele não deve ser incluído ao enviar dados para a sessão de upload.

## <a name="completing-a-file"></a>Concluindo um arquivo

Quando o último intervalo de bytes de um arquivo for recebido, o servidor responderá com um `HTTP 201 Created`. O corpo da resposta também incluirá o conjunto de propriedades para o **printDocument** associado.

### <a name="request"></a>Solicitação
<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-final", "scopes": "printjob.readwrite" } -->
```http
PUT https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}
Content-Length: 10
Content-Range: bytes 4533312-4533321/4533322

<final bytes of the file>
```

### <a name="response"></a>Resposta
<!-- { "blockType": "response", "@odata.type": "microsoft.graph.printDocument", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
   "id": "9001bcd9-e36a-4f51-bfc6-140c3ad7f9f7",
   "documentName": "TestFile.pdf",
   "contentType": "application/pdf", 
   "size": 4533322
}
```

>**Observação:** A sessão de upload é excluída após a conclusão do upload do documento.

## <a name="get-the-upload-session"></a>Obter a sessão de upload

Para obter a sessão de upload, envie uma solicitação GET para a URL de upload. 

### <a name="request"></a>Solicitação
<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->

```http
GET https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}
```

### <a name="response"></a>Resposta

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
  "nextExpectedRanges": [
  "72797-72897",
  "78929-4533322"
  ]
}
```
## <a name="code-examples-create-upload-session-and-upload-documents"></a>Exemplos de código: Criar sessão de upload e carregar documentos
 
# <a name="c"></a>[C#](#tab/csharp)

```csharp

            GraphServiceClient graphClient = new GraphServiceClient( authProvider );

            var properties = new PrintDocumentUploadProperties
            {
                DocumentName = "TestFile.pdf",
                ContentType = "application/pdf",
                Size = 4533322
            };

            var uploadSession = await graphClient.Print.Printers["{printer-id}"].Jobs["{printJob-id}"].Documents["{printDocument-id}"]
                .CreateUploadSession(properties)
                .Request()
                .PostAsync()

            // if using Graph SDK, maxSliceSize should in multiples of 320 KiB
            int maxSliceSize = 320 * 1024;
            var fileUploadTask =
                new LargeFileUploadTask<PrintDocument>(uploadSession, fileStream, maxSliceSize);

            // Create a callback that is invoked after each slice is uploaded
            IProgress<long> progress = new Progress<long>(prog =>
            {
                Console.WriteLine($"Uploaded {prog} bytes of {fileStream.Length} bytes");
            });

            // Upload the file

            var uploadResult = await fileUploadTask.UploadAsync(progress);
```

# <a name="javascript"></a>[JavaScript](#tab/javascript)

```javascript

    const options = {
      authProvider,
    };
    const client = Client.init(options);
   
    const fileName = "test.txt";
    const file = fs.readFileSync(`./${fileName}`);
    const stats = fs.statSync(`./${fileName}`);
    const requestUrl ="https://graph.microsoft.com/v1.0/print/shares/{id}/jobs/{id}/documents/{id}/createuploadsession"
    const payload = {
        "properties": {
            "documentName": fileName,
            "contentType": "application/pdf",
            "size": stats.size
        }
    }
    const uploadSession = await LargeFileUploadTask.createUploadSession(client, requestUrl, payload);

    // Create FileUpload object. 
    /* Note:
     * As alternatives to using a javascript `File` object to create a `FileUpload`, 
     * you can use a `ReadStream` object to create a `StreamUpload`.
     * const readStream = fs.createReadStream(`./test/sample_files/${fileName}`);
     * const fileObject = new StreamUpload(readStream, fileName, totalsize);
     * OR
     * you can also create a custom implementation of the `FileObject` interface.
     * FileUpload and StreamUpload classes are available in 3.0.0 version of the Microsoft Graph JS client library.
     */
    const fileObject = new FileUpload(file, file.name, file.size);
     
    // Create LargeFileUploadTask object and start the upload() task
    const task = new LargeFileUploadTask(client, fileObject, uploadSession);
    const uploadResponse = await task.upload();
```
---

## <a name="cancel-the-upload-session"></a>Cancelar a sessão de upload

Para cancelar uma sessão de upload, envie uma solicitação DELETE para a URL de upload. Isso deve ser usado em cenários em que o upload é interrompido; por exemplo, se o usuário cancelar a transferência.

Os arquivos temporários e a sessão de carregamento que os acompanha são automaticamente limpos decorrido o valor de **expirationDateTime**.

### <a name="request"></a>Solicitação

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-cancel", "scopes": "printjob.readwrite" } -->

```http
DELETE https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}
```

### <a name="response"></a>Resposta

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```
