---
title: 'subjectRightsRequest: getFinalAttachment'
description: Obter o anexo final de uma solicitação de direitos de assunto.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 30c5c7df1e000fc284849e3f41f1dfec411d6fb7
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60447024"
---
# <a name="subjectrightsrequest-getfinalattachment"></a>subjectRightsRequest: getFinalAttachment
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter o anexo final de uma solicitação de direitos de assunto. O anexo é um arquivo zip que contém todos os arquivos incluídos pelo administrador de privacidade.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|SubjectRightsRequest.Read.All *, SubjectRightsRequest.ReadWrite.All*|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte|

>[!IMPORTANT]
>No momento, as permissões marcadas com um asterisco (*) não estão disponíveis. Para mais detalhes, confira [Problemas conhecidos](/graph/known-issues#compliance).

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /privacy/subjectRightsRequests/{subjectRightsRequestId}/getFinalAttachment
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, essa função será redirecionada para o link de armazenamento Microsoft Azure blob com o token SAS e retornará `302` um código de resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "subjectRightsRequest_getfinalattachment"
}
-->
``` http
GET https://graph.microsoft.com/beta/privacy/subjectRightsRequests/{subjectRightsRequestId}/getFinalAttachment
```


### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 302 
```

