---
title: Anexar arquivos a uma Tarefa Pendente
description: Saiba como anexar grandes arquivos a uma Tarefa Pendente da Microsoft e como escolher a abordagem certa para anexar um arquivo a uma tarefa.
author: avijityadav
ms.localizationpriority: high
ms.prod: outlook
ms.openlocfilehash: 2d4c66a6e6e2438f1d7b7aafc6555ab701d1883a
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671357"
---
# <a name="attach-files-to-a-to-do-task"></a>Anexar arquivos a uma Tarefa Pendente

Usando a API de Tarefas Pendentes no Microsoft Graph, você pode anexar arquivos de até 25 MB a uma [Tarefa Pendente](/graph/api/resources/todotask). Dependendo do tamanho do arquivo, escolha uma das duas maneiras de anexar o arquivo:
- Para anexar arquivos de qualquer tamanho, crie uma sessão de upload e use `PUT` iteradamente para carregar intervalos de bytes do arquivo até que você carregue todo o arquivo. Um cabeçalho na resposta `PUT` finalizada com êxito inclui uma URL com a ID do anexo.
- Se o tamanho do arquivo for menor que 3 MB, faça uma única `POST` na propriedade de navegação dos **anexos** de uma **Tarefa Pendente**; veja como fazer isto [para uma tarefa](/graph/api/todotask-post-attachments). A resposta `POST` bem-sucedida inclui a ID de anexo do arquivo.

Este artigo ilustra a primeira abordagem. Você aprenderá passo a passo como criar e usar uma sessão de upload para adicionar um arquivo anexo a uma tarefa.
## <a name="step-1-create-an-upload-session"></a>Etapa 1: criar uma sessão de carregamento

[Criar uma sessão de upload](/graph/api/taskfileattachment-createuploadsession) para anexar para uma **Tarefa pendente**. Especifique o arquivo no parâmetro de entrada [attachmentInfo](/graph/api/resources/attachmentinfo).

Uma operação bem-sucedida retorna `HTTP 201 Created` e uma nova instância[uploadSession](/graph/api/resources/uploadsession), que contém uma URL opaca que você pode usar em operações `PUT` subseqüentes para carregar partes do arquivo. A **uploadSession** fornece um local de armazenamento temporário onde os bytes do arquivo são salvos até que você tenha carregado o arquivo completo.

O objeto **uploadSession** na resposta também inclui a propriedade **nextExpectedRanges**, que indica que a localização inicial de upload deve ser de `0` bytes.

### <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Tasks.ReadWrite|
|Delegado (conta pessoal da Microsoft)|Tasks.ReadWrite|
|Aplicativo|Sem suporte.|

### <a name="example-create-an-upload-session-for-a-todotask"></a>Exemplo: criar uma sessão de upload para uma Tarefa pendente

#### <a name="request"></a>Solicitação

O seguinte é um exemplo de uma solicitação para criar uma sessão de upload.
<!-- {
  "blockType": "request",
  "name": "todo_attachment_walkthrough_createuploadsession"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/todo/lists/AAMDiFkfh=/tasks/AAMkADliMm=/attachments/createUploadSession
Content-Type: application/json

{
  "attachmentInfo": {
    "@odata.type": "microsoft.graph.attachmentInfo",
    "attachmentType": "file",
    "name": "flower",
    "size": 3483322
  }
}
```

#### <a name="response"></a>Resposta
O seguinte exemplo mostra o recurso **uploadSession** devolvido para a tarefa no corpo de réplica.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://graph.microsoft.com/beta/users/6f9a2a92-8527-4d64-837e-b5312852f36d/todo/lists/AAMDiFkfh=/tasks/AAMkADliMm=/attachmentSessions/AAMkADliMm=",
    "expirationDateTime": "2022-06-09T10:45:27.4324526Z",
    "nextExpectedRanges": [
        "0-"
    ]
}
```

## <a name="step-2-use-the-upload-session-to-upload-a-range-of-bytes-of-the-file"></a>Etapa 2: usar a sessão de carregamento para carregar um intervalo de bytes do arquivo

Para carregar o arquivo, ou uma parte do arquivo, faça uma solicitação `PUT` à URL retornada na etapa 1 na propriedade **uploadUrl** do recurso **uploadSession**. Você pode carregar todo o arquivo ou dividi-lo em vários intervalos de bytes. Cada intervalo de bytes precisa ser inferior a 4 MB.

Especifique os cabeçalhos de solicitação e o corpo da solicitação, conforme descrito nas seções a seguir.

### <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Tipo | Descrição|
|:---------------|:--------|:----------|
|Autorização | Cadeia de caracteres | {token} de portador. Obrigatório. |
| Content-Length | Int32 | O número de bytes sendo carregados nesta operação. O limite superior do número de bytes para cada operação `PUT` é de 4 MB. A solicitação falhará para qualquer coisa superior a 4 MB. Obrigatório. |
| Intervalo de conteúdo | Cadeia de Caracteres | O intervalo de bytes baseado em 0 do arquivo que está sendo carregado nesta operação, expresso no formato `bytes {start}-{end}/{total}`. Requerido. |
| Content-Type | Cadeia de Caracteres  | O tipo MIME. Especifique`application/octet-stream`. Obrigatório. |


### <a name="request-body"></a>Corpo da solicitação

Especificar os bytes reais do arquivo a ser anexado, que estão no intervalo de local especificado pelo cabeçalho da solicitação`Content-Range`.

### <a name="response"></a>Resposta
Um upload bem-sucedido devolve um código de resposta `HTTP 200 OK` e um objeto **uploadSession**. Observe o seguinte no objeto de resposta:

- O valor da propriedade **expirationDateTime** permanece o mesmo que foi devolvido pela **uploadSession** inicial na etapa 1.
- O **nextExpectedRanges** especifica o próximo local do byte para iniciar o carregamento, por exemplo, `"nextExpectedRanges":["2097152"]`. Você deve carregar os bytes em um arquivo na ordem.
<!-- The **nextExpectedRanges** specifies one or more byte ranges, each indicating the starting point of a subsequent `PUT` request:

  - On a successful upload, this property returns the next range to start from, for example, `"nextExpectedRanges":["2097152"]`.
  - If a portion of a byte range has not uploaded successfully, this property includes the byte range with the start and end locations, for example, `"nextExpectedRanges":["1998457-2097094"]`.
-->
- A propriedade **uploadUrl** não é devolvida explicitamente, pois todas as operações `PUT` de uma sessão de upload usam a mesma URL devolvida quando você cria a sessão (etapa 1).

### <a name="example-first-upload-to-the-todotask"></a>Exemplo: primeiro upload para a Tarefa pendente

#### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação.

<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://graph.microsoft.com/beta/users/6f9a2a92-8527-4d64-837e-b5312852f36d/todo/lists/AAMDiFkfh=/tasks/AAMkADliMm=/attachmentSessions/AAMkADliMm=/content
Content-Type: application/octet-stream
Content-Length: 2097152
Content-Range: bytes 0-2097151/3483322

{
  <bytes 0-2097151 of the file to be attached, in binary format>
}
```

#### <a name="response"></a>Resposta

O seguinte é um exemplo da resposta que mostra na propriedade **nextExpectedRanges** o início do próximo intervalo de bytes que o servidor espera.
<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "ExpirationDateTime":"2022-06-09T10:45:27.4324526Z",
  "NextExpectedRanges":["2097152"]
}
```

## <a name="step-3-continue-uploading-byte-ranges-until-the-entire-file-has-been-uploaded"></a>Etapa 3: continuar carregando intervalos de bytes até que todo o arquivo tenha sido carregado

Após o carregamento inicial na etapa 2, continue a carregar a parte restante do arquivo, usando uma solicitação `PUT` semelhante, conforme descrito na etapa 2, antes que você atinja a data/hora de vencimento da sessão. Use a coleção **nextExpectedRanges** para determinar onde iniciar o próximo intervalo de bytes a ser carregado. Você pode ver vários intervalos especificados, indicando as partes do arquivo que o servidor ainda não recebeu. Isso é útil quando você precisa retomar uma transferência que foi interrompida, e seu cliente não tem certeza sobre o estado no serviço.

Quando o último byte do arquivo for carregado com êxito, a `PUT`operação final devolve um `HTTP 201 Created` código de resposta final e um `Location` cabeçalho que indica a URL para o anexo de arquivo. Você pode obter a ID do anexo na URL e salvá-la para uso posterior.

Os seguintes exemplos mostram como carregar o último intervalo de bytes do arquivo para a **Tarefa pendente** das etapas anteriores.

### <a name="example-final-upload-to-the-todotask"></a>Exemplo: último upload para a Tarefa pendente

#### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação.

<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://graph.microsoft.com/beta/users/6f9a2a92-8527-4d64-837e-b5312852f36d/todo/lists/AAMDiFkfh=/tasks/AAMkADliMm=/attachmentSessions/AAMkADliMm=/content
Content-Type: application/octet-stream
Content-Length: 1386170
Content-Range: bytes 2097152-3483321/3483322

{
  <bytes 2097152-3483321 of the file to be attached, in binary format>
}
```

#### <a name="response"></a>Resposta
O seguinte é um exemplo da resposta que mostra um `Location` cabeçalho de resposta do qual você pode salvar a ID do anexo (`AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=`) para uso posterior.

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 201 Created

Location: https://graph.microsoft.com/beta/users/6f9a2a92-8527-4d64-837e-b5312852f36d/todo/lists/AAMDiFkfh=/tasks/AAMkADliMm=/Attachments/AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=
Content-Length: 0
```

## <a name="alternative-step-cancel-the-upload-session"></a>Etapa alternativa: cancelar a sessão de upload
Em qualquer momento antes da sessão de upload expirar, se você tiver que cancelar o upload, você pode usar a mesma URL inicial para excluir a sessão de upload. Uma operação bem-sucedida retorna um código de resposta HTTP `204 No Content`.

### <a name="example-cancel-the-upload-session"></a>Exemplo: cancelar a sessão de upload

#### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação.

<!-- {
  "blockType": "ignored"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/6f9a2a92-8527-4d64-837e-b5312852f36d/todo/lists/AAMDiFkfh=/tasks/AAMkADliMm=/attachmentSessions/AAMkADliMm=
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 204 No content
```

