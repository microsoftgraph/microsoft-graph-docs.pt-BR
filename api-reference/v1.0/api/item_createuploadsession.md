# <a name="upload-large-files-with-an-upload-session"></a>Carregar arquivos grandes com uma sessão de upload

Crie uma sessão de upload para permitir que seu aplicativo carregue arquivos até o tamanho máximo de arquivo. Uma sessão de upload permite que seu aplicativo carregue intervalos do arquivo em solicitações de API sequenciais, permitindo que a transferência seja retomada se uma conexão for interrompida enquanto o upload estiver em andamento.

Para carregar um arquivo usando uma sessão de upload, duas etapas são obrigatórias:

1. [Criar uma sessão de upload](#create-an-upload-session)
2. [Carregar bytes na sessão de upload](#upload-bytes-to-the-upload-session)

## <a name="prerequisites"></a>Pré-requisitos
Um dos seguintes **escopos** é obrigatório para executar esta API:

* Files.ReadWrite
* Files.ReadWrite.All
* Sites.ReadWrite.All

> **Observação**: A permissão de aplicativo Files.ReadWrite.All ainda não tem suporte nessa API. O suporte completo está planejado para breve. 

## <a name="create-an-upload-session"></a>Criar uma sessão de upload

Para iniciar o upload de um arquivo grande, seu aplicativo deve primeiro solicitar uma nova sessão de upload. Isso cria um local de armazenamento temporário no qual os bytes do arquivo serão salvos até que este seja totalmente carregado. Depois que o último byte do arquivo for carregado, a sessão de upload será concluída, e o arquivo final aparecerá na pasta de destino.

### <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root:/{path-to-item}:/createUploadSession
POST /me/drive/items/{parent-item-id}:/{filename}:/createUploadSession
```

### <a name="request-body"></a>Corpo da solicitação
Nenhum corpo de solicitação é obrigatório. No entanto, você pode especificar um corpo de solicitação para fornecer dados adicionais sobre o arquivo que está sendo carregado.

Por exemplo, para controlar o comportamento se o nome do arquivo já estiver em uso, você pode especificar a propriedade de comportamento conflitante no corpo da solicitação.

```json
{
    "item": {
        "@microsoft.graph.conflictBehavior": "rename"
    }
}
```

### <a name="optional-request-headers"></a>Cabeçalhos de solicitação opcionais

| Nome       | Valor | Descrição                                                                                                                                                            |
|:-----------|:------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| *if-match* | etag  | Se esse cabeçalho de solicitação for incluído, e a eTag (ou cTag) fornecida não corresponder à etag atual no item, uma resposta de erro `412 Precondition Failed` será retornada. |


### <a name="response"></a>Resposta
A resposta a essa solicitação fornecerá os detalhes da [uploadSession](../resources/uploadsession.md) recém-criada, que inclui a URL usada para carregar as partes do arquivo. 

### <a name="example"></a>Exemplo

<!-- {
  "blockType": "request",
  "name": "driveItem_createUploadSession"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root:/{item-path}:/createUploadSession
```

#### <a name="response-example"></a>Exemplo de resposta
Veja a seguir um exemplo da resposta.

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

## <a name="upload-bytes-to-the-upload-session"></a>Carregar bytes na sessão de upload

Para carregar o arquivo, ou uma parte do arquivo, o aplicativo faz uma solicitação PUT ao valor de **uploadUrl** recebido na de **createUploadSession**. Você pode carregar o arquivo inteiro ou dividi-lo em fragmentos, desde que o máximo de bytes em qualquer solicitação específica seja menor que 60 MiB. Os fragmentos do arquivo devem ser carregados sequencialmente em ordem. O upload de fragmentos fora de ordem resultará em um erro.

**Observação:** Se seu aplicativo dividir um arquivo em vários fragmentos, o tamanho de cada fragmento **DEVERÁ** ser um múltiplo de 320 KiB. Usar um tamanho de fragmento que não divide uniformemente por 320 resultará em erros ao confirmar alguns arquivos.

### <a name="example"></a>Exemplo

Este exemplo está carregando os primeiros 26 bytes de um arquivo 128 bytes. O cabeçalho **Content-Length** especifica o tamanho da solicitação atual. O cabeçalho **Content-Range** indica o intervalo de bytes no arquivo geral que essa solicitação representa. O tamanho total do arquivo deve ser conhecido antes que você possa carregar seu primeiro fragmento.

<!-- { "blockType": "request", "name": "upload-fragment-piece", "scopes": "files.readwrite" } -->
```
PUT https://tenant-my.sharepoint.com/alkjl1kjklna
Content-Length: 26
Content-Range: bytes 0-25/128

<bytes 0-25 of the file>
```

**Importante:** Seu aplicativo deve garantir que o tamanho total do arquivo especificado no cabeçalho **Content-Range** seja o mesmo para todas as solicitações. Se um fragmento declarar um tamanho de arquivo diferente, a solicitação falhará.

#### <a name="response-example"></a>Exemplo de resposta
<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["26-"]
}
```

O aplicativo pode usar o valor de **nextExpectedRanges** para determinar onde iniciar o próximo fragmento. É possível ver vários intervalos especificados, indicando partes do arquivo que o servidor ainda não recebeu. Isso é útil quando você precisa retomar uma transferência que foi interrompida, e seu cliente não tem certeza sobre o estado no serviço.

Você sempre deve determinar o tamanho do fragmento de acordo com as práticas recomendadas a seguir. Não suponha que **nextExpectedRanges** retornará intervalos de tamanho apropriado para um fragmento de upload. A propriedade **nextExpectedRanges** indica intervalos do arquivo que não foram recebidos, e não um padrão para como você deve carregar esse arquivo.

**Observações:**

* A propriedade `nextExpectedRanges` nem sempre listará todos os intervalos ausentes.
* Em gravações de fragmento bem-sucedidas, ela retornará o próximo intervalo do qual começar (ex: "523-").
* Em falhas quando o cliente enviou um fragmento que o servidor já havia recebido, o servidor responderá com `HTTP 416 Requested Range Not Satisfiable`. Você pode [solicitar o status do upload](#resuming-an-in-progress-upload) para obter uma lista mais detalhada dos intervalos que estão faltando.
* Incluindo o cabeçalho de autorização, fazer a chamada de `PUT` pode resultar em uma resposta `HTTP 401 Unauthoized`. O cabeçalho de autorização e o token de portador só devem ser enviados ao emitir o `POST` durante a primeira etapa. Não deve ser incluído ao emitir o `PUT`.   


## <a name="completing-a-file"></a>Concluindo um arquivo

Quando o último fragmento de um arquivo for recebido, o servidor responderá com um `HTTP 201 Created` ou `HTTP 200 OK`. O corpo da resposta também incluirá o conjunto de propriedades padrão para o **driveItem** que representa o arquivo concluído.

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
**Observação:** A resposta do item é truncada para clareza de documentação.

## <a name="cancel-an-upload-session"></a>Cancelar uma sessão de upload

Para cancelar uma sessão de upload, envie uma solicitação DELETE para a URL de upload. Isso limpa o arquivo temporário que contém os dados anteriormente carregados. Isso deve ser usado em cenários em que o upload é interrompido, por exemplo, se o usuário cancelar a transferência.

Os arquivos temporários e a sessão de upload que os acompanha são automaticamente limpos decorrido o valor de **expirationDateTime**.

### <a name="example"></a>Exemplo

A solicitação DELETE fará com que a sessão de upload expire imediatamente e removerá qualquer byte anteriormente carregado.

<!-- { "blockType": "request", "name": "upload-fragment-cancel", "scopes": "files.readwrite" } -->
```http
DELETE https://tenant-my.sharepoint.com/alkjl1kjklna
```

#### <a name="response-example"></a>Exemplo de resposta

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 204 No Content
```

## <a name="resuming-an-in-progress-upload"></a>Retomando um upload em andamento

Se uma solicitação de upload for desconectada ou falhar antes de ser concluída, todos os seus bytes serão ignorados. Isso pode ocorrer quando a conexão entre seu aplicativo e o serviço é interrompida. Se isso ocorrer, seu aplicativo ainda poderá retomar a transferência do fragmento anteriormente concluído.

Para descobrir quais intervalos de bytes foram recebidos anteriormente, seu aplicativo pode solicitar o status de uma sessão de upload.

### <a name="example"></a>Exemplo
Confira o status do upload enviando uma solicitação GET para `uploadUrl`.

<!-- { "blockType": "request", "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->
```
GET https://tenant-my.sharepoint.com/alkjl1kjklna
```

O servidor responderá com uma lista de intervalos de bytes ausentes que precisam ser carregados e com a hora de expiração da sessão de upload.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->
```http
HTTP/1.1 200 OK

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["12345-"]
}
```

### <a name="upload-remaining-data"></a>Carregar os dados restantes
Agora que o seu aplicativo sabe de onde começar o upload, retome o upload seguindo as etapas em [Carregar bytes na sessão de upload](#upload-bytes-to-the-upload-session).


## <a name="best-practices"></a>Práticas recomendadas

* Retome ou repita uploads que falharam devido a interrupções de conexão ou erros 5xx, como:
  * `500 Internal Server Error`
  * `502 Bad Gateway`
  * `503 Service Unavailable`
  * `504 Gateway Timeout`
* Use uma estratégia de retirada exponencial se erros de servidor 5xx forem retornados ao retomar ou repetir solicitações de upload.
* Para outros erros, você não deve usar uma estratégia de retirada exponencial, mas sim limitar o número de tentativas de repetição feitas.
* Lide com erros `404 Not Found` ao fazer uploads retomáveis reiniciando o upload inteiro.
* Use transferências de arquivos retomáveis para arquivos com mais de 10 MiB (10 \* 1.024 \* 1.024 bytes).
* Um tamanho de fragmento de 10 MiB para conexões estável de alta velocidade é ideal. Para conexões mais lentas ou menos confiáveis, você pode obter melhores resultados com um tamanho de fragmento menor. O tamanho do fragmento recomendado é entre 5 e 10 MiB.
* Use um tamanho de fragmento que seja múltiplo de 320 KiB (320 \* 1.024 bytes). Uma falha ao usar um tamanho de fragmento que seja múltiplo de 320 KiB pode resultar na falha de transferências de arquivos grandes após o upload do último fragmento.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upload item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
