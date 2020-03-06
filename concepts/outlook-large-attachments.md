---
title: Anexar arquivos grandes a mensagens do Outlook
description: Dependendo do tamanho do arquivo, você pode escolher uma de duas maneiras de anexar um arquivo a uma mensagem.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 5f6f54adf38c0f2827b587e6646df4cb3549a204
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448568"
---
# <a name="attach-large-files-to-outlook-messages-as-attachments-preview"></a>Anexar arquivos grandes às mensagens do Outlook como anexos (visualização)

Dependendo do tamanho do arquivo, você pode escolher uma das duas maneiras de anexar um arquivo a uma [mensagem](/graph/api/resources/message?view=graph-rest-beta):

- Se o tamanho do arquivo for menor que 3 MB, você poderá executar um único [POST na propriedade de navegação de anexos da mensagem](/graph/api/message-post-attachments?view=graph-rest-beta). A resposta `POST` bem-sucedida inclui a ID do arquivo anexado à mensagem.
- Se o tamanho do arquivo estiver entre 3 MB e 150 MB, crie uma sessão de carregamento e use o `PUT` iteradamente para carregar intervalos de bytes do arquivo até que você carregue todo o arquivo. Um cabeçalho na resposta `PUT` finalizada com êxito inclui uma URL com a ID do anexo. 

Para anexar vários arquivos a uma mensagem, escolha a abordagem de cada arquivo com base em seu tamanho e anexe-os individualmente.

Este artigo usa um exemplo para ilustrar a segunda abordagem. O exemplo cria e usa uma sessão de carregamento para adicionar um anexo de arquivo grande (com tamanho acima de 3 MB) a uma mensagem específica. Depois de carregar o arquivo inteiro, ele recebe uma URL que contém uma identificação para o arquivo em anexo, com o qual ele pode fazer outras operações, como obter os metadados do anexo de arquivo.

> [!IMPORTANT] 
> Esteja atento a um [problema conhecido](known-issues.md#attaching-large-files-to-messages)se você estiver anexando arquivos de grande tamanho a uma mensagem em uma caixa de correio delegada ou compartilhada.

## <a name="step-1-create-an-upload-session"></a>Etapa 1: Criar uma sessão de upload

[Criar uma sessão de carregamento](/graph/api/attachment-createuploadsession?view=graph-rest-beta) para anexar um arquivo a uma mensagem. Especifique o arquivo no parâmetro de entrada **AttachmentItem**.

Uma operação bem-sucedida retorna `HTTP 201 Created` e uma nova instância[uploadSession](/graph/api/resources/uploadsession?view=graph-rest-beta), que contém uma URL opaca que você pode usar em operações `PUT` subseqüentes para carregar partes do arquivo. A **uploadSession** fornece um local de armazenamento temporário onde os bytes do arquivo são salvos até que você tenha carregado o arquivo completo.

Verifique se solicitou `Mail.ReadWrite`permissão para criar **uploadSession**. A URL opaca, retornada na propriedade **uploadUrl** do novo **uploadSession** é pré-autenticada e contém o token de autorização apropriado para consultas `PUT` subsequentes no domínio `https://outlook.office.com`. Esse token expira por **expirationDateTime**. Não Personalize essa URL para as operações `PUT`.

O objeto**uploadSession** na resposta também inclui a propriedade **nextExpectedRanges**, que indica que o local inicial de carregamento deve ser byte 0.

### <a name="example-request-create-an-upload-session"></a>Solicitação de exemplo: criar uma sessão de carregamento

# <a name="http"></a>[HTTP](#tab/http)
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/walkthrough-create-uploadsession-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/walkthrough-create-uploadsession-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/walkthrough-create-uploadsession-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="example-response-get-an-uploadsession-object"></a>Exemplo de resposta: Obtenha um objeto uploadSession
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


## <a name="step-2-use-the-upload-session-to-upload-a-range-of-bytes-of-the-file"></a>Etapa 2: Usar a sessão de carregamento para carregar um intervalo de bytes do arquivo

Para carregar o arquivo, ou uma parte do arquivo, faça uma solicitação `PUT` para o valor da propriedade **uploadUrl** retornado como parte de **uploadSession** na etapa 1. Você pode carregar todo o arquivo ou dividi-lo em vários intervalos de bytes. Para melhorar o desempenho, mantenha cada intervalo de bytes com menos de 4 MB.

Especifique os cabeçalhos e corpo da solicitação conforme é descrito abaixo.

### <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Tipo | Descrição|
|:---------------|:--------|:----------|
| Content-Length | Int32 | O número de bytes sendo carregados nesta operação. Para melhorar o desempenho, mantenha o limite superior do número de bytes para cada operação `PUT` em 4 MB. Obrigatório. |
| Intervalo de conteúdo | Cadeia de Caracteres | O intervalo de bytes baseado em 0 do arquivo que está sendo carregado nesta operação, expresso no formato `bytes {start}-{end}/{total}`. Obrigatório. |
| Content-Type | Cadeia de Caracteres  | O tipo MIME. Especifique`application/octet-stream`. Obrigatório. |

Não especifique um cabeçalho da solicitação`Authorization`. A consulta `PUT` usa uma URL pré-existente da propriedade **uploadUrl**, que permite o acesso ao domínio `https://outlook.office.com`.

### <a name="request-body"></a>Corpo da solicitação

Especificar os bytes reais do arquivo a ser anexado, que estão no intervalo de local especificado pelo cabeçalho da solicitação`Content-Range`.

### <a name="response"></a>Resposta
Um carregamento bem-sucedido retorna `HTTP 200 OK` e um objeto **uploadSession**. Observe o seguinte no objeto de resposta:

- A propriedade **ExpirationDateTime** indica a data/hora de vencimento para o token de autenticação inserido no valor da propriedade **uploadUrl**. Essa data/hora de vencimento permanece a mesma que foi retornada pela **uploadSession** inicial na etapa 1.
- **NextExpectedRanges** especifica o próximo local do byte para começar o carregamento a partir de `"NextExpectedRanges":["2097152"]`, por exemplo. Você deve carregar os bytes em um arquivo na ordem.
<!-- The **NextExpectedRanges** specifies one or more byte ranges, each indicating the starting point of a subsequent `PUT` request:

  - On a successful upload, this property returns the next range to start from, for example, `"NextExpectedRanges":["2097152"]`.
  - If a portion of a byte range has not uploaded successfully, this property includes the byte range with the start and end locations, for example, `"NextExpectedRanges":["1998457-2097094"]`.
-->
- A propriedade **uploadUrl** não é retornada explicitamente, pois todas as operações `PUT` de uma sessão de carregamento usam a mesma URL retornada ao criar a sessão (etapa 1).

### <a name="example-request-first-upload"></a>Solicitação de exemplo: primeiro carregamento
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

### <a name="example-response-get-the-start-of-the-next-byte-range-that-the-server-expects"></a>Resposta de exemplo: obter o início do próximo intervalo de bytes esperado pelo servidor
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


## <a name="step-3-continue-uploading-byte-ranges-until-the-entire-file-has-been-uploaded"></a>Etapa 3: continuar carregando intervalos de bytes até que todo o arquivo tenha sido carregado

Após o carregamento inicial na etapa 2, continue a carregar a parte restante do arquivo, usando uma solicitação `PUT` semelhante, conforme descrito na etapa 2, antes que você atinja a data/hora de vencimento da sessão. Use a coleção **NextExpectedRanges** para determinar onde começar o próximo intervalo de bytes a ser carregado. É possível ver vários intervalos especificados, indicando partes do arquivo que o servidor ainda não recebeu. Isso é útil quando você precisa retomar uma transferência que foi interrompida, e seu cliente não tem certeza sobre o estado no serviço.

Quando o último byte do arquivo for carregado com êxito, a operação de `PUT` final retornará `HTTP 201 Created` e um cabeçalho `Location` que indica a URL para o anexo de arquivo no domínio `https://outlook.office.com`. Você pode obter a ID do anexo na URL e salvá-la para uso posterior. Dependendo do seu cenário, você pode usar essa ID para [obter os metadados do anexo](/graph/api/attachment-get?view=graph-rest-beta)ou [remover o anexo da mensagem](/graph/api/attachment-delete?view=graph-rest-beta) usando o ponto de extremidade do Microsoft Graph.

O exemplo a seguir mostra como carregar o último intervalo de bytes do arquivo.

### <a name="example-request-final-upload"></a>Solicitação de exemplo: carregamento final
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

### <a name="example-response-get-the-location-response-header-to-save-the-attachment-id"></a>Resposta de exemplo: obter o cabeçalho de resposta do local para salvar a ID do anexo

Na URL especificada pelo cabeçalho da resposta `Location`, salve a ID do anexo (`AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=`) para uso posterior.

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 201 Created

Location: https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/Attachments('AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=')
Content-Length: 0
```

## <a name="step-4-optional-get-the-file-attachment-from-the-message"></a>Etapa 4 (opcional): obter o arquivo em anexo da mensagem

Como sempre, [obter um anexo](/graph/api/attachment-get?view=graph-rest-beta) a partir de uma mensagem não é tecnicamente limitado pelo tamanho do anexo.

No entanto, obter um anexo de arquivo grande no formato base64-encoded afeta o desempenho da API. Se você espera um anexo grande:

- Como uma alternativa para obter o conteúdo do anexo no formato base64, você pode [obter os dados brutos do arquivo em anexo](/graph/api/attachment-get#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message?view=graph-rest-1.0).
- Para [obter os metadados do anexo de arquivo](/graph/api/attachment-get?view=graph-rest-beta#example-1-get-the-properties-of-a-file-attachment), acrescente um parâmetro `$select` para incluir somente as propriedades de metadados desejadas, excluindo a propriedade **contentBytes** que retorna o arquvo em anexo no formato base64.

### <a name="example-request-get-the-file-attachment-metadata"></a>Solicitação de exemplo: obter os metadados do arquivo em anexo

O exemplo a seguir mostra o remetente usando um parâmetro `$select` para obter todos os metadados de um arquivo em anexo em uma mensagem, exceto o **contentBytes**.

<!-- {
  "blockType": "request",
  "name": "walkthrough_get_attachment",
  "sampleKeys": ["a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47", "AAMkADI5MAAIT3drCAAA=", "AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0="]
}-->
```http
GET https://graph.microsoft.com/api/v1.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/Attachments('AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=')?$select=lastModifiedDateTime,name,contentType,size,isInline
```

### <a name="example-response"></a>Resposta de exemplo

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

## <a name="alternative-cancel-the-upload-session"></a>Alternativa: cancelar a sessão de carregamento

Em qualquer momento antes da sessão de carregamento expirar, se for preciso cancelar o carregamento, você poderá usar a mesma URL opaca inicial para excluir a sessão de carregamento. Uma operação bem-sucedida retorna `HTTP 204 No Content`.

### <a name="example-request-cancel-an-upload-session"></a>Solicitação de exemplo: cancelar uma sessão de carregamento

<!-- {
  "blockType": "ignored"
}-->
```http
DELETE https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
```

### <a name="example-response"></a>Resposta de exemplo

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 204 No content
```
## <a name="errors"></a>Erros

### <a name="errorattachmentsizeshouldnotbelessthanminimumsize"></a>ErrorAttachmentSizeShouldNotBeLessThanMinimumSize

Este erro é devolvido ao tentar [criar uma sessão de upload](/graph/api/attachment-createuploadsession?view=graph-rest-beta) para anexar um arquivo menor que 3 MB. Se o tamanho do arquivo for menor que 3 MB, execute um único [POST na propriedade de navegação de anexos da mensagem](/graph/api/message-post-attachments?view=graph-rest-beta). A resposta `POST` bem-sucedida inclui a ID do arquivo anexado à mensagem.

