---
title: Faça o upload de documentos utilizando a API de Impressão Universal do Microsoft Graph
description: A Impressão Universal é uma solução de impressão moderna que as organizações podem utilizar para gerenciar sua infraestrutura de impressão por meio de serviços em nuvem da Microsoft.
author: nilakhan
localization_priority: Priority
ms.prod: universal-print
ms.custom: scenarios:getting-started
ms.openlocfilehash: c51d027a0e76f24f6ec4788ae1429adcc29f2948
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766312"
---
# <a name="upload-documents-using-the-microsoft-graph-universal-print-api"></a>Faça o upload de documentos utilizando a API de Impressão Universal do Microsoft Graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../api-reference/includes/cloudprinting-pricing-disclaimer.md)]

Para imprimir um documento utilizando a API de Impressão Universal no Microsoft Graph, você [cria um trabalho de impressão](/graph/api/printershare-post-jobs), faz o upload do documento e, em seguida, [inicia o trabalho de impressão](/graph/api/printjob-start). Este artigo descreve como fazer o upload de um documento, que começa com [ a criação de uma sessão de upload ](/graph/api/printdocument-createuploadsession).

Para fazer o upload de um arquivo, ou de parte de um arquivo, seu aplicativo faz uma solicitação PUT para o valor **uploadUrl** recebido na resposta **createUploadSession**.
Você pode fazer o upload de todo o arquivo ou dividi-lo em vários intervalos de bytes, desde que o máximo de bytes em qualquer solicitação seja inferior a 10 MB.

É possível fazer o upload dos segmentos do arquivo em qualquer ordem e o upload pode ser feito em paralelo, com até quatro solicitações simultâneas. Quando todos os segmentos binários do documento são carregados, o arquivo binário é vinculado ao **printDocument**.

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
### <a name="http-response"></a>Resposta HTTP:

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

* Em falhas quando o cliente enviou um fragmento que o servidor já havia recebido, o servidor responderá com `HTTP 416 Requested Range Not Satisfiable`. Você pode [solicitar o status do upload](#get-the-upload-session) para obter uma lista mais detalhada dos intervalos que estão faltando.
* Incluir o Cabeçalho de Autorização ao emitir a chamada `PUT`pode resultar em uma resposta`HTTP 401 Unauthorized`. O Cabeçalho de Autorização e o token do portador devem ser enviados apenas durante a criação da sessão de upload. Não deve ser incluído ao enviar dados para a sessão de upload.

## <a name="completing-a-file"></a>Concluindo um arquivo

Quando o último intervalo de bytes de um arquivo for recebido, o servidor responderá com um `HTTP 201 Created`. O corpo da resposta também incluirá o conjunto de propriedades para o **printDocument** associado.

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-final", "scopes": "printjob.readwrite" } -->

```http
PUT https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}
Content-Length: 10
Content-Range: bytes 4533312-4533321/4533322

<final bytes of the file>
```

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

## <a name="get-the-upload-session"></a>Obtenha a sessão de upload

Para obter a sessão de upload, envie uma solicitação GET para o URL de upload. 

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

## <a name="cancel-the-upload-session"></a>Cancelar a sessão de upload

Para cancelar uma sessão de upload, envie uma solicitação DELETE para o URL de upload. Isso deve ser usado em cenários em que o upload é interrompido, por exemplo, se o usuário cancelar a transferência.

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
