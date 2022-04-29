---
title: Anexar arquivos grandes a mensagens ou eventos do Outlook
description: Dependendo do tamanho do arquivo, você pode escolher uma das duas maneiras de anexar um arquivo a uma mensagem ou evento.
author: abheek-das
ms.localizationpriority: high
ms.prod: outlook
ms.openlocfilehash: 582501205c106b3deaf0312f3db9c81488feb3de
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133045"
---
# <a name="attach-large-files-to-outlook-messages-or-events"></a>Anexar arquivos grandes a mensagens ou eventos do Outlook

Usando a API do Microsoft Graph, é possível anexar arquivos de até 150 MB a uma [mensagem](/graph/api/resources/message) ou item de [evento](/graph/api/resources/event) do Outlook. Dependendo do tamanho do arquivo, escolha uma das duas maneiras de anexar o arquivo:
- Se o tamanho do arquivo for inferior a 3 MB, faça um único POST na propriedade de navegação **attachments** do item do Outlook; veja como fazer isso [para uma mensagem](/graph/api/message-post-attachments) ou [para um evento](/graph/api/event-post-attachments). A resposta `POST` bem-sucedida inclui o ID do anexo do arquivo.
- Se o tamanho do arquivo estiver entre 3 MB e 150 MB, crie uma sessão de upload e use iterativamente `PUT` para carregar intervalos de bytes do arquivo até que você tenha carregado o arquivo inteiro. Um cabeçalho na resposta final `PUT` bem-sucedida inclui um URL com o ID do anexo.

Para anexar vários arquivos a uma mensagem, escolha a abordagem de cada arquivo com base em seu tamanho e anexe-os individualmente.

Este artigo ilustra a segunda abordagem passo a passo, criando e usando uma sessão de carregamento para adicionar um anexo de arquivo grande (de tamanho superior a 3MB) a um item do Outlook. Cada etapa mostra o código correspondente de uma mensagem e de um evento. Ao carregar o arquivo inteiro com êxito, o artigo exibe a obtenção de um cabeçalho de resposta contendo uma ID para o anexo do arquivo e, em seguida, o uso dessa ID de anexo para obter o conteúdo bruto do anexo ou metadados do anexo. 

> [!IMPORTANT] 
> Esteja atento a um [problema conhecido](known-issues.md#attaching-large-files-to-messages-with-delegated-permissions-can-fail)se você estiver anexando arquivos de grande tamanho a uma mensagem ou evento em uma caixa de correio delegada ou compartilhada.

## <a name="step-1-create-an-upload-session"></a>Etapa 1: criar uma sessão de carregamento

[Criar uma sessão de carregamento](/graph/api/attachment-createuploadsession) para anexar um arquivo a uma mensagem ou evento. Especifique o arquivo no parâmetro de entrada **AttachmentItem**.

Uma operação bem-sucedida retorna `HTTP 201 Created` e uma nova instância[uploadSession](/graph/api/resources/uploadsession), que contém uma URL opaca que você pode usar em operações `PUT` subseqüentes para carregar partes do arquivo. A **uploadSession** fornece um local de armazenamento temporário onde os bytes do arquivo são salvos até que você tenha carregado o arquivo completo.

O objeto **uploadSession** na resposta também inclui a propriedade **nextExpectedRanges**, que indica que o local inicial de carregamento deve ser byte 0.

### <a name="permissions"></a>Permissões
Certifique-se de pedir permissão de `Mail.ReadWrite` para criar a **uploadSession** para uma mensagem e `Calendars.ReadWrite` para um evento. 

A URL opaca, retornada na propriedade **uploadUrl** do novo **uploadSession** é pré-autenticada e contém o token de autorização apropriado para consultas `PUT` subsequentes no domínio `https://outlook.office.com`. Esse token expira por **expirationDateTime**. Não Personalize essa URL para as operações `PUT`.


### <a name="example-create-an-upload-session-for-a-message"></a>Exemplo: criar uma sessão de carregamento para uma mensagem

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/walkthrough-create-uploadsession-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/walkthrough-create-uploadsession-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/walkthrough-create-uploadsession-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/walkthrough-create-uploadsession-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
O exemplo de resposta a seguir mostra o recurso **uploadSession** retornado para a mensagem.

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

### <a name="example-create-an-upload-session-for-an-event"></a>Exemplo: criar uma sessão de carregamento para uma evento
#### <a name="request"></a>Solicitação 


# <a name="http"></a>[HTTP](#tab/http)
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/walkthrough-create-uploadsession-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/walkthrough-create-uploadsession-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/walkthrough-create-uploadsession-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/walkthrough-create-uploadsession-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta
O exemplo de resposta a seguir mostra o recurso **uploadSession** retornado para o evento.

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


## <a name="step-2-use-the-upload-session-to-upload-a-range-of-bytes-of-the-file"></a>Etapa 2: usar a sessão de carregamento para carregar um intervalo de bytes do arquivo

Para carregar o arquivo, ou uma parte do arquivo, faça uma solicitação `PUT` à URL retornada na etapa 1 na propriedade **uploadUrl** do recurso **uploadSession**. Você pode carregar todo o arquivo ou dividi-lo em vários intervalos de bytes. Para melhorar o desempenho, mantenha cada intervalo de bytes com menos de 4 MB.

Especifique os cabeçalhos e corpo da solicitação conforme é descrito abaixo.

### <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Tipo | Descrição|
|:---------------|:--------|:----------|
| Content-Length | Int32 | O número de bytes sendo carregados nesta operação. Para melhorar o desempenho, mantenha o limite superior do número de bytes para cada operação `PUT` em 4 MB. Obrigatório. |
| Intervalo de conteúdo | Cadeia de Caracteres | O intervalo de bytes baseado em 0 do arquivo que está sendo carregado nesta operação, expresso no formato `bytes {start}-{end}/{total}`. Requerido. |
| Content-Type | Cadeia de Caracteres  | O tipo MIME. Especifique`application/octet-stream`. Obrigatório. |

Não especifique um cabeçalho de solicitação `Authorization`. A consulta `PUT` usa um URL pré-autenticado da propriedade **uploadUrl**, que permite acesso ao domínio `https://outlook.office.com`.

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

### <a name="example-first-upload-to-the-message"></a>Exemplo: primeiro carregamento na mensagem
#### <a name="request"></a>Solicitação
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

#### <a name="response"></a>Resposta

O exemplo de resposta a seguir mostra na propriedade **NextExpectedRanges** o início do próximo intervalo de bytes que o servidor espera.
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

### <a name="example-first-upload-to-the-event"></a>Exemplo: primeiro carregamento na evento
#### <a name="request"></a>Solicitação
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

#### <a name="response"></a>Resposta

O exemplo de resposta a seguir mostra na propriedade **NextExpectedRanges** o início do próximo intervalo de bytes que o servidor espera.
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


## <a name="step-3-continue-uploading-byte-ranges-until-the-entire-file-has-been-uploaded"></a>Etapa 3: continuar carregando intervalos de bytes até que todo o arquivo tenha sido carregado

Após o carregamento inicial na etapa 2, continue a carregar a parte restante do arquivo, usando uma solicitação `PUT` semelhante, conforme descrito na etapa 2, antes que você atinja a data/hora de vencimento da sessão. Use a coleção **NextExpectedRanges** para determinar onde começar o próximo intervalo de bytes a ser carregado. É possível ver vários intervalos especificados, indicando partes do arquivo que o servidor ainda não recebeu. Isso é útil quando você precisa retomar uma transferência que foi interrompida, e seu cliente não tem certeza sobre o estado no serviço.

Quando o último byte do arquivo for carregado com êxito, a operação de `PUT` final retornará `HTTP 201 Created` e um cabeçalho `Location` que indica a URL para o anexo de arquivo no domínio `https://outlook.office.com`. Você pode obter a ID do anexo na URL e salvá-la para uso posterior. Dependendo do cenário, você pode usar essa ID para [obter os metadados do anexo](/graph/api/attachment-get)ou [remover o anexo do item do Outlook](/graph/api/attachment-delete) usando o ponto de extremidade do Microsoft Graph.

Os exemplos a seguir mostram o carregamento do último intervalo de bytes do arquivo na mensagem e no evento das etapas anteriores.

### <a name="example-final-upload-to-the-message"></a>Exemplo: último carregamento na mensagem
#### <a name="request"></a>Solicitação
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

#### <a name="response"></a>Resposta
O exemplo de resposta a seguir mostra um cabeçalho de resposta de `Location` onde você pode salvar a ID do anexo (`AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=`) para uso posterior.

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 201 Created

Location: https://outlook.office.com/api/v2.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/Attachments('AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=')
Content-Length: 0
```

### <a name="example-final-upload-to-the-event"></a>Exemplo: último carregamento no evento
#### <a name="request"></a>Solicitação
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

#### <a name="response"></a>Resposta
O exemplo de resposta a seguir mostra um cabeçalho de resposta de `Location` onde você pode salvar a ID do anexo (`AAMkADU5CCmSAAANZAlYPeyQByv7Y=`) para uso posterior.

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 201 Created

Location: https://outlook.office.com/api/v2.0/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/Attachments('AAMkADU5CCmSAAANZAlYPeyQByv7Y=')
Content-Length: 0
```

## <a name="step-4-optional-get-the-file-attachment-from-the-outlook-item"></a>Etapa 4 (opcional): obter o arquivo em anexo do item do Outlook

Como sempre, [obter um anexo](/graph/api/attachment-get) a partir de um item do Outlook não é tecnicamente limitado pelo tamanho do anexo.

No entanto, obter um anexo de arquivo grande no formato base64-encoded afeta o desempenho da API. Se você espera um anexo grande:

- Como uma alternativa para obter o conteúdo do anexo no formato base64, você pode [obter os dados brutos do arquivo em anexo](/graph/api/attachment-get#example-6-get-the-raw-contents-of-a-file-attachment-on-a-message).
- Para [obter os metadados do anexo de arquivo](/graph/api/attachment-get#example-1-get-the-properties-of-a-file-attachment), acrescente um parâmetro `$select` para incluir somente as propriedades de metadados desejadas, excluindo a propriedade **contentBytes** que retorna o arquvo em anexo no formato base64.

### <a name="example-get-the-raw-file-attached-to-the-event"></a>Exemplo: obter o arquivo bruto anexado ao evento
Seguindo o exemplo de evento e utilizando a ID do anexo retornada no cabeçalho de `Location` da etapa anterior, a solicitação de exemplo nesta seção mostra o uso de um parâmetro `$value` para obter os dados de conteúdo bruto do anexo.

#### <a name="permissions"></a>Permissões
Use a permissão delegada ou de aplicativo menos privilegiada, `Calendars.Read`, conforme apropriado, para esta operação. Para obter mais informações, consulte [permissões do calendário](permissions-reference.md#calendars-permissions).

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "ignored",
  "name": "walkthrough_get_attachment_raw",
  "sampleKeys": ["d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32", "AAMkADU5CCmSAAA=", "AAMkADU5CCmSAAANZAlYPeyQByv7Y="]
}-->
```http
GET https://graph.microsoft.com/v1.0/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/Attachments('AAMkADU5CCmSAAANZAlYPeyQByv7Y=')/$value
```

#### <a name="response"></a>Resposta

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


### <a name="example-get-the-metadata-of-the-file-attached-to-the-message"></a>Exemplo: obter os metadados do arquivo anexado à mensagem
Seguindo o exemplo da mensagem, a solicitação de exemplo de solicitação nesta seção mostra o uso de um parâmetro `$select` para obter alguns dos metadados de um anexo de arquivo em uma mensagem, excluindo o **contentBytes**.

#### <a name="permissions"></a>Permissões
Use a permissão delegada ou de aplicativo menos privilegiada, `Mail.Read`, conforme apropriado, para esta operação. Para obter mais informações, consulte [permissões de email](permissions-reference.md#mail-permissions).

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "walkthrough_get_attachment_metadata",
  "sampleKeys": ["a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47", "AAMkADI5MAAIT3drCAAA=", "AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0="]
}-->
```http
GET https://graph.microsoft.com/api/v1.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/Attachments('AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=')?$select=lastModifiedDateTime,name,contentType,size,isInline
```

#### <a name="response"></a>Resposta

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


## <a name="alternative-cancel-the-upload-session"></a>Alternativa: cancelar a sessão de carregamento

A qualquer momento antes que a sessão de upload expire, se você precisar cancelar o upload, poderá usar o mesmo URL opaco inicial para excluir a sessão de upload. Uma operação bem-sucedida retorna `HTTP 204 No Content`.

### <a name="permissions"></a>Permissões
Como a URL opaca inicial é pré-autenticada e contém o token de autorização apropriado para consultas subsequentes para essa sessão de carregamento, não especifique um cabeçalho de solicitação de autorização para essa operação.

### <a name="example-cancel-the-upload-session-for-the-message"></a>Exemplo: cancelar a sessão de carregamento da mensagem

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "ignored"
}-->
```http
DELETE https://outlook.office.com/api/v2.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 204 No content
```
## <a name="errors"></a>Erros

### <a name="errorattachmentsizeshouldnotbelessthanminimumsize"></a>ErrorAttachmentSizeShouldNotBeLessThanMinimumSize

Este erro é devolvido ao tentar [criar uma sessão de upload](/graph/api/attachment-createuploadsession) para anexar um arquivo menor que 3 MB. Se o tamanho do arquivo for menor que 3 MB, faça uma única POSTAGEM na propriedade de navegação dos **anexos** da [mensagem](/graph/api/message-post-attachments) ou do [evento](/graph/api/event-post-attachments). A resposta `POST` bem-sucedida inclui a ID do arquivo anexado à mensagem.

