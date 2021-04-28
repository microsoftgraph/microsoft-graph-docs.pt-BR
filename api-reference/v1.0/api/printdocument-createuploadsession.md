---
title: 'printDocument: createUploadSession'
description: Crie uma sessão de carregamento para carregar de forma iterativa intervalos de arquivo binário de printDocument.
localization_priority: Normal
author: nilakhan
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: c72144dc8b4aa39a87b1c8785ba61e69dab16c37
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067212"
---
# <a name="printdocument-createuploadsession"></a>printDocument: createUploadSession
Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Crie uma sessão de carregamento que permita que um aplicativo carregue de forma iterativa intervalos de um arquivo binário vinculado ao documento de impressão.

Como parte da resposta, essa ação retorna uma URL de carregamento que pode ser usada em consultas `PUT` sequenciais subsequentes. Os headers de solicitação para cada operação podem ser usados para especificar o intervalo exato de `PUT` bytes a serem carregados. Isso permite que a transferência seja retomada, caso a conexão de rede seja largada durante o carregamento. 

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma [](printer-get.md) assinatura de Impressão Universal ativa e ter uma permissão que conceda Obter impressora ou Obter acesso a [PrinterShare,](printershare-get.md) dependendo se a impressora ou impressoraShare está sendo usada.

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | PrintJob.Create, PrintJob.ReadWrite, PrintJob.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | PrintJob.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

Para criar uma sessão de carregamento usando **impressora**: 

<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/createUploadSession
```

Para criar uma sessão de carregamento usando **printerShare**: 

<!-- { "blockType": "ignored" } -->
```http
POST /print/shares/{id}/jobs/{id}/documents/{id}/createUploadSession
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo        | Descrição |
|:-------------|:------------|:------------|
|propriedades|[printDocumentUploadProperties](../resources/printDocumentUploadProperties.md)|Representa propriedades do arquivo binário a ser carregado.|

O valor da **propriedade contentType** no corpo da solicitação deve ser suportado pela impressora/printerShare. Você pode obter os tipos de conteúdo com suporte ao obter [printerCapabilities](../resources/printercapabilities.md) da impressora/printerShare. 

Para **conversão de OXPS para PDF,** você precisa passar `application/oxps` como contentType para printer/printerShare que oferece suporte `application/pdf` a . Impressão Universal converte **OXPS em PDF**, quando **todas** as seguintes condições são atendidas: 
1.  O compartilhamento de impressora/impressora é `application/pdf` compatível **com printerCapabilities**. 
2.  O compartilhamento de impressora/impressora NÃO é `application/oxps` suportado em **printerCapabilities**. 
3.  O valor da **propriedade contentType** no corpo da solicitação é `application/oxps` .

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` novo [objeto uploadSession](../resources/uploadsession.md) no corpo da resposta.

>**Observação**: a **propriedade uploadUrl** retornada como parte do objeto de resposta **uploadSession** é uma URL opaca para consultas subsequentes para carregar intervalos de `PUT` byte do arquivo. Ele contém o token de auth apropriado para consultas `PUT` subsequentes que expiram por **expirationDateTime**. Não altere essa URL.

## <a name="examples"></a>Exemplos

O exemplo a seguir mostra como criar uma sessão de carregamento que você pode usar nas operações subsequentes de carregamento de arquivo para o printDocument especificado.

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "printdocument_createuploadsession"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}/documents/{printDocumentId}/createUploadSession
Content-Type: application/json
Content-length: 96

{
  "properties": {
    "documentName": "TestFile.pdf",
    "contentType": "application/pdf", 
    "size": 4533322
  }
}
```


### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}",
    "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
    "nextExpectedRanges": [
        "0-4533321"
    ]
}
```

