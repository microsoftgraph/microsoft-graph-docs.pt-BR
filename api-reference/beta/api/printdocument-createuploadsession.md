---
title: 'Documento de documentos: createUploadSession'
description: Criar uma sessão de carregamento para carregar com interseção intervalos de arquivos binários do arquivo de documentos.
localization_priority: Normal
author: nilakhan
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 47043b64806cfa9ef3a66026a60b84ae11112168
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704875"
---
# <a name="printdocument-createuploadsession"></a>Documento de documentos: createUploadSession

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Criar uma sessão de carregamento que permite que um aplicativo carregue intervalos de forma iterativa de um arquivo binário vinculado ao documento de impressão.

Como parte da resposta, esta ação retorna uma URL de upload que pode ser usada em consultas sequenciais subsequentes `PUT` . Os cabeçalhos de solicitação de cada `PUT` operação podem ser usados para especificar o intervalo exato de bytes a serem carregados. Isso permite que a transferência seja retomada, caso a conexão de rede seja interrompida durante o carregamento. 

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é necessária para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).
Além das permissões a seguir, o locatário do usuário ou do aplicativo deve ter uma assinatura de impressão universal ativa e ter uma permissão que conceda [obter impressora](printer-get.md) ou obter o acesso do [printerShare](printershare-get.md) , dependendo se a impressora ou o printerShare está sendo usado.

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | PrintJob. ReadWrite, PrintJob. ReadWrite. All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | PrintJob.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

Para criar uma sessão de carregamento usando **impressora**: 

<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/createUploadSession
```

Para criar uma sessão de carregamento usando o **printerShare**: 

<!-- { "blockType": "ignored" } -->
```http
POST /print/shares/{id}/jobs/{id}/documents/{id}/createUploadSession
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | {token} de portador. Obrigatório. |
| Content-type | application/json. Obrigatório.|


## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo        | Descrição |
|:-------------|:------------|:------------|
|propriedades|[printDocumentUploadProperties](../resources/printDocumentUploadProperties.md)|Representa as propriedades do arquivo binário a ser carregado.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um novo objeto [uploadSession](../resources/uploadsession.md) no corpo da resposta.

>**Observação**: a propriedade **uploadUrl** retornada como parte do objeto de resposta **uploadSession** é uma URL opaca para consultas subsequentes `PUT` para carregar intervalos de bytes do arquivo. Ele contém o token de autenticação apropriado para `PUT` consultas subsequentes que expiram pelo **expirationDateTime**. Não altere essa URL.

## <a name="examples"></a>Exemplos

O exemplo a seguir mostra como criar uma sessão de carregamento que você pode usar em operações de upload de arquivo subsequentes para o documento de documentos.

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
}-->
```http
POST https://graph.microsoft.com/beta/print/shares/1c879027-5120-4aaf-954a-ebfd509a3bcc/jobs/46207/documents/9001bcd9-e36a-4f51-bfc6-140c3ad7f9f7/createUploadSession
Content-type: application/json

{
  "properties": {
    "documentName": "TestFile.pdf",
    "contentType": "application/pdf", 
    "size": 4533322
  }
}
```

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}",
    "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
    "nextExpectedRanges": [
        "0-4533321"
    ]
}
```
