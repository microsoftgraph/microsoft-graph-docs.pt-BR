---
title: 'printDocument: createUploadSession'
description: Crie uma sessão de upload para carregar iterativamente intervalos de arquivo binário do printDocument.
localization_priority: Normal
author: nilakhan
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 0dbb2a9101fbf5033d1c91f1254c6ea0ba00f6e4
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2021
ms.locfileid: "49784834"
---
# <a name="printdocument-createuploadsession"></a>printDocument: createUploadSession

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie uma sessão de upload que permita que um aplicativo carregue iterativamente intervalos de um arquivo binário vinculado ao documento de impressão.

Como parte da resposta, essa ação retorna uma URL de carregamento que pode ser usada em consultas `PUT` sequenciais subsequentes. Os headers de solicitação para cada operação podem ser usados para especificar o intervalo exato de `PUT` bytes a serem carregados. Isso permite que a transferência seja retomada, caso a conexão de rede seja retirada durante o upload. 

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é necessária para chamar essa API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).
Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa e ter uma permissão que conceda acesso a [Obter](printer-get.md) impressora ou Obter [printerShare,](printershare-get.md) dependendo se impressora ou printerShare está sendo usada.

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | PrintJob.Create, PrintJob.ReadWrite, PrintJob.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | PrintJob.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

Para criar uma sessão de upload usando **impressora:** 

<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/createUploadSession
```

Para criar uma sessão de upload usando **printerShare**: 

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
|propriedades|[printDocumentUploadProperties](../resources/printDocumentUploadProperties.md)|Representa propriedades do arquivo binário a ser carregado.|

O valor da propriedade **contentType** no corpo da solicitação deve ser suportado pela impressora/printerShare. Você pode obter os tipos de conteúdo com suporte ao [obter printerCapabilities](../resources/printercapabilities.md) da impressora/printerShare. 

Para **conversão de OXPS para PDF,** você precisa passar `application/oxps` como contentType para printer/printerShare que oferece `application/pdf` suporte. A Impressão Universal converte **OXPS em PDF,** **quando todas as** seguintes condições são atendidas: 
1.  O compartilhamento de impressora/impressora `application/pdf` é compatível **com printerCapabilities**. 
2.  O compartilhamento de impressora/impressora NÃO é suportado `application/oxps` em **printerCapabilities**. 
3.  O valor da propriedade **contentType** no corpo da solicitação é `application/oxps` .

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta e um novo objeto `200 OK` [uploadSession](../resources/uploadsession.md) no corpo da resposta.

>**Observação:** a **propriedade uploadUrl** retornada como parte do objeto de resposta **uploadSession** é uma URL opaca para consultas subsequentes para carregar intervalos de `PUT` byte do arquivo. Ele contém o token de autorização apropriado para consultas `PUT` subsequentes que expiram **por expirationDateTime**. Não altere essa URL.

## <a name="examples"></a>Exemplos

O exemplo a seguir mostra como criar uma sessão de upload que você pode usar nas operações subsequentes de carregamento de arquivo para o printDocument especificado.

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
