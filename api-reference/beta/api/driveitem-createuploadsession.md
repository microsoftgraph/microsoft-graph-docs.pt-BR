---
author: JeremyKelley
description: Crie uma sessão de upload para permitir que seu aplicativo carregue arquivos até o tamanho máximo de arquivo.
title: 'driveItem: createUploadSession'
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: apiPageType
ms.openlocfilehash: dfb6b231b0db8664b7c01fd81f2697f4387554b6
ms.sourcegitcommit: 4c8444b732b8d6d0de8a95f6666c42095f146266
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/08/2022
ms.locfileid: "62442642"
---
# <a name="driveitem-createuploadsession"></a>driveItem: createUploadSession

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie uma sessão de upload para permitir que seu aplicativo carregue arquivos até o tamanho máximo de arquivo.

Uma sessão de carregamento permite que seu aplicativo carregue intervalos do arquivo em solicitações de API sequenciais, o que permite que a transferência seja retomada se uma conexão for retirada enquanto o carregamento estiver em andamento.

Para carregar um arquivo usando uma sessão de carregamento:

1. [Criar uma sessão de upload](#create-an-upload-session)
2. [Carregar bytes na sessão de upload](#upload-bytes-to-the-upload-session)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Files.ReadWrite, Files.ReadWrite.All    |
|Aplicativo | Sites.ReadWrite.All |

## <a name="create-an-upload-session"></a>Criar uma sessão de upload

Para iniciar o upload de um arquivo grande, seu aplicativo deve primeiro solicitar uma nova sessão de upload.
Isso cria um local de armazenamento temporário no qual os bytes do arquivo serão salvos até que este seja totalmente carregado.
Depois que o último byte do arquivo for carregado, a sessão de upload será concluída, e o arquivo final aparecerá na pasta de destino.
Como alternativa, você pode adiar a criação final do arquivo no destino até que você tenha feito explicitamente uma solicitação para concluir o carregamento, definindo a propriedade `deferCommit` nos argumentos da solicitação.

### <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createUploadSession
POST /groups/{groupId}/drive/items/{itemId}/createUploadSession
POST /me/drive/items/{itemId}/createUploadSession
POST /sites/{siteId}/drive/items/{itemId}/createUploadSession
POST /users/{userId}/drive/items/{itemId}/createUploadSession
```

### <a name="request-body"></a>Corpo da solicitação

No entanto, você pode especificar propriedades no corpo da solicitação, fornecendo dados adicionais sobre o arquivo sendo carregado e personalizando a semântica da operação de carregamento.

Por exemplo, a propriedade `item` permite definir os seguintes parâmetros:
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.driveItemUploadableProperties" } -->
```json
{
  "@microsoft.graph.conflictBehavior": "fail (default) | replace | rename",
  "description": "description",
  "driveItemSource": { "@odata.type": "microsoft.graph.driveItemSource" },
  "fileSize": 1234,
  "name": "filename.txt",
  "mediaSource": { "@odata.type": "microsoft.graph.mediaSource" }
}
```

O exemplo a seguir controla o comportamento se o nome do arquivo já estiver sendo tirado e também especifica se o arquivo final não deve ser criado até que uma solicitação de conclusão explícita seja feita:

<!-- { "blockType": "ignored" } -->
```json
{
  "item": {
    "@microsoft.graph.conflictBehavior": "rename"
  },
  "deferCommit": true
}
```

### <a name="optional-request-headers"></a>Cabeçalhos de solicitação opcionais

| Nome       | Valor | Descrição                                                                                                                                                            |
|:-----------|:------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| *if-match* | etag  | Se esse cabeçalho de solicitação for incluído e a eTag (ou cTag) fornecida não corresponder à eTag atual no item, retornará uma resposta de erro `412 Precondition Failed`. |

## <a name="parameters"></a>Parâmetros

| Parâmetro            | Tipo                          | Descrição
|:---------------------|:------------------------------|:---------------------------------
| item                 | [driveItemUploadableProperties](../resources/driveItemUploadableProperties.md) | Dados sobre o arquivo sendo carregado
| deferCommit          | Booliano                       | Se definido como verdadeiro, a criação final do arquivo no destino exigirá uma solicitação explícita. Apenas no OneDrive for Business.

### <a name="request"></a>Solicitação

A resposta a essa solicitação fornecerá os detalhes da [uploadSession](../resources/uploadsession.md) recém-criada, que inclui a URL usada para carregar as partes do arquivo. 

>**Observação:** O {item-path} deve conter o nome do item especificado no corpo da solicitação.

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

### <a name="response"></a>Resposta

A resposta a essa solicitação, se tiver êxito, fornecerá os detalhes sobre o local para onde o restante das solicitações deve ser enviado como um recurso [UploadSession](../resources/uploadsession.md).

Esse recurso fornece detalhes sobre onde o intervalo de bytes do arquivo deve ser carregado e quando a sessão de carregamento expira.

Se o parâmetro `fileSize` for especificado e exceder a cota disponível, uma resposta `507 Insufficent Storage` será retornada e a sessão de carregamento não será criada.

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

## <a name="upload-bytes-to-the-upload-session"></a>Carregar bytes na sessão de upload

Para carregar o arquivo ou uma parte dele, seu aplicativo faz uma solicitação PUT para o valor **uploadUrl** recebido na resposta **createUploadSession**. Você pode carregar todo o arquivo ou dividi-lo em vários intervalos de bytes, desde que o máximo de bytes em qualquer solicitação seja inferior a 60 MiB.

Os fragmentos do arquivo devem ser carregados sequencialmente em ordem.
O upload de fragmentos fora de ordem resultará em um erro.

**Observação:** se seu aplicativo dividir um arquivo em vários intervalos de bytes, o tamanho de cada intervalo de bytes **DEVE** ser um múltiplo de 320 KiB (327.680 bytes). O uso de um tamanho de fragmento que não é dividido uniformemente por 320 KiB resultará em erros ao confirmar alguns arquivos.

### <a name="example"></a>Exemplo

Neste exemplo, o aplicativo está carregando os primeiros 26 bytes de um arquivo de 128 bytes.

* O cabeçalho **Content-Length** especifica o tamanho da solicitação atual.
* O cabeçalho **Content-Range** indica o intervalo de bytes no arquivo geral que essa solicitação representa.
* O tamanho total do arquivo precisa ser conhecido antes que você possa carregar seu primeiro fragmento.

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-piece", "scopes": "files.readwrite" } -->

```http
PUT https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
Content-Length: 26
Content-Range: bytes 0-25/128

<bytes 0-25 of the file>
```

**Importante:** seu aplicativo deve garantir que o tamanho total do arquivo especificado no cabeçalho **Content-Range** seja o mesmo para todas as solicitações. Se um intervalo de bytes declarar um tamanho de arquivo diferente, a solicitação falhará.

### <a name="response"></a>Resposta

Quando a solicitação for concluída, o servidor responderá com `202 Accepted` se houver mais intervalos de bytes que precisem ser carregados.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["26-"]
}
```

O aplicativo pode usar o valor **nextExpectedRanges** para determinar onde iniciar o próximo intervalo de bytes. É possível ver vários intervalos especificados, indicando partes do arquivo que o servidor ainda não recebeu. Isso é útil quando você precisará retomar uma transferência que foi interrompida e seu cliente não tem certeza sobre o estado do serviço.

Você sempre deve determinar o tamanho dos intervalos de bytes de acordo com as práticas recomendadas abaixo. Não suponha que **nextExpectedRanges** retornará intervalos de tamanho adequado para um intervalo de bytes a ser carregado. A propriedade **nextExpectedRanges** indica os intervalos do arquivo que não foram recebidos e não um padrão de como seu aplicativo deve carregar o arquivo.

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

## <a name="remarks"></a>Comentários

* A propriedade `nextExpectedRanges` nem sempre listará todos os intervalos ausentes.
* Em gravações de fragmento bem-sucedidas, ela retornará o próximo intervalo do qual começar (ex: "523-").
* Em falhas quando o cliente enviou um fragmento que o servidor já havia recebido, o servidor responderá com `HTTP 416 Requested Range Not Satisfiable`. Você pode [solicitar o status do upload](#resuming-an-in-progress-upload) para obter uma lista mais detalhada dos intervalos que estão faltando.
* Incluindo o cabeçalho de autorização, fazer a chamada de `PUT` pode resultar em uma resposta `HTTP 401 Unauthorized`. O cabeçalho de autorização e o token de portador só devem ser enviados ao emitir o `POST` durante a primeira etapa. Não deve ser incluído ao emitir o `PUT`.

## <a name="completing-a-file"></a>Concluindo um arquivo

Se `deferCommit` for falso ou não configurado, o carregamento será concluído automaticamente quando o intervalo de bytes final do arquivo for colocado na URL de carregamento.

Se `deferCommit` for verdadeiro, você pode concluir explicitamente o carregamento de duas maneiras:
- Após o intervalo de bytes final do arquivo ser colocado na URL de carregamento, envie uma solicitação final de POST para a URL de carregamento com conteúdo de comprimento zero (no momento, com suporte somente no OneDrive for Business e no SharePoint).
- Após o intervalo de bytes final do arquivo ser COLOCADO na URL de carregamento, envie uma solicitação final de PUT na mesma maneira que você [resolveria erros de carregamento](#handle-upload-errors) (no momento, com suporte somente no OneDrive for Business e no SharePoint).


Quando o carregamento for concluído, o servidor responderá à solicitação final com `HTTP 201 Created` ou `HTTP 200 OK`. O corpo da resposta também incluirá o conjunto de propriedades padrão do **driveItem** que representa o arquivo concluído.

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-final", "scopes": "files.readwrite" } -->

```http
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

```http
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

## <a name="handling-upload-conflicts"></a>Tratamento de conflitos de carregamento

Se ocorrer um conflito depois do carregamento do arquivo (por exemplo, um item com o mesmo nome foi criado durante a sessão de carregamento), será retornado um erro quando o último intervalo de bytes for carregado.

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

## <a name="cancel-the-upload-session"></a>Cancelar a sessão de upload

Para cancelar uma sessão de upload, envie uma solicitação DELETE para a URL de upload. Isso limpa o arquivo temporário que contém os dados anteriormente carregados. Isso deve ser usado em cenários em que o upload é interrompido, por exemplo, se o usuário cancelar a transferência.

Os arquivos temporários e a sessão de upload que os acompanha são automaticamente limpos decorrido o valor de **expirationDateTime**.
Arquivos temporários não podem ser excluídos imediatamente após o período de expiração.

### <a name="request"></a>Solicitação

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-cancel", "scopes": "files.readwrite" } -->

```http
DELETE https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
```

### <a name="response"></a>Resposta

O exemplo a seguir mostra a resposta.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

## <a name="resuming-an-in-progress-upload"></a>Retomando um upload em andamento

Se uma solicitação de upload for desconectada ou falhar antes de ser concluída, todos os seus bytes serão ignorados. Isso pode ocorrer quando a conexão entre seu aplicativo e o serviço é interrompida. Se isso ocorrer, seu aplicativo ainda poderá retomar a transferência do fragmento anteriormente concluído.

Para descobrir quais intervalos de bytes foram recebidos anteriormente, seu aplicativo pode solicitar o status de uma sessão de upload.

### <a name="example"></a>Exemplo

Confira o status do upload enviando uma solicitação GET para `uploadUrl`.

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->

```http
GET https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF86633784148bb98a1zjcUhf7b0mpUadahs
```

O servidor responderá com uma lista de intervalos de bytes ausentes que precisam ser carregados e com a hora de expiração da sessão de upload.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["12345-"]
}
```

### <a name="upload-remaining-data"></a>Carregar os dados restantes

Agora que o seu aplicativo sabe de onde começar o upload, retome o upload seguindo as etapas em [Carregar bytes na sessão de upload](#upload-bytes-to-the-upload-session).

## <a name="handle-upload-errors"></a>Tratar erros de carregamento

Quando o último intervalo de bytes de um arquivo é carregado, é possível que ocorra um erro. Isso pode ser devido a um conflito de nome ou limitação de cota excedida. A sessão de upload será preservada até o tempo de expiração, o que permite que seu aplicativo recupere o upload, confirmando explicitamente a sessão de upload.

Para confirmar manualmente a sessão de carregamento, o aplicativo deve fazer uma solicitação PUT com um novo recurso **driveItem**, que será usado ao confirmar a sessão de carregamento.
Essa nova solicitação deve corrigir a origem do erro que gerou o erro de carregamento original.

Para indicar que o aplicativo está confirmando uma sessão de carregamento existente, a solicitação PUT deve incluir a propriedade `@microsoft.graph.sourceUrl` com o valor de sua URL de sessão de carregamento.

<!-- { "blockType": "ignored", "name": "explicit-upload-commit", "scopes": "files.readwrite", "tags": "service.graph" } -->

```http
PUT /me/drive/root:/{path_to_file}
Content-Type: application/json
If-Match: {etag or ctag}

{
  "name": "largefile.vhd",
  "@microsoft.graph.conflictBehavior": "rename",
  "@microsoft.graph.sourceUrl": "{upload session URL}"
}
```

**Observação:** Você pode usar os cabeçalhos `@microsoft.graph.conflictBehavior` e `if-match` conforme esperado nessa chamada.

### <a name="response"></a>Resposta

Se o arquivo puder ser confirmado usando os novos metadados, uma resposta `HTTP 201 Created` ou `HTTP 200 OK` será retornada com os metadados de Item para o arquivo carregado.

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

## <a name="best-practices"></a>Práticas recomendadas

* Retome ou repita uploads que falharam devido a interrupções de conexão ou erros 5xx, como:
  * `500 Internal Server Error`
  * `502 Bad Gateway`
  * `503 Service Unavailable`
  * `504 Gateway Timeout`
* Use uma estratégia de retirada exponencial se erros de servidor 5xx forem retornados ao retomar ou repetir solicitações de upload.
* Para outros erros, você não deve usar uma estratégia de retirada exponencial, mas sim limitar o número de tentativas de repetição feitas.
* Lide com erros `404 Not Found` ao fazer uploads retomáveis reiniciando o upload inteiro. Isso indica que a sessão de carregamento não existe mais.
* Use transferências de arquivos retomáveis para arquivos com mais de 10 MiB (10.485.760 bytes).
* É ideial um tamanho de intervalo de bytes de 10 MiB para conexões estável de alta velocidade. Para conexões mais lentas ou menos confiáveis, você pode obter melhores resultados com um tamanho de fragmento menor. O tamanho do fragmento recomendado é entre 5 e 10 MiB.
* Use um tamanho de intervalo de bytes que seja múltiplo de 320 KiB (327.680 bytes). Uma falha ao usar um tamanho de fragmento que seja múltiplo de 320 KiB pode resultar na falha de transferências de arquivos grandes após o carregamento do último intervalo de bytes.

## <a name="error-responses"></a>Respostas de erros

Confira o tópico [Respostas de Erro][error-response] para saber detalhes sobre como os erros são retornados.

[driveItemSource]: ../resources/driveItemSource.md
[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md
[mediaSource]: ../resources/mediaSource.md

<!--
{
  "type": "#page.annotation",
  "description": "Upload large files using an upload session.",
  "keywords": "upload,large file,fragment,BITS",
  "section": "documentation",
  "suppressions": []
}
-->


