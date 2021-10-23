---
title: 'subjectRightsRequest: getFinalAttachment'
description: Obter o anexo final de uma solicitação de direitos de assunto.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 0e537a31cad80a35d79e3cd4d2cf95aac4b67349
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60559635"
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
|Application|Sem suporte|

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

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "subjectRightsRequest_getfinalattachment"
}
-->
``` http
GET https://graph.microsoft.com/beta/privacy/subjectRightsRequests/{subjectRightsRequestId}/getFinalAttachment
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/subjectrightsrequest-getfinalattachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/subjectrightsrequest-getfinalattachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/subjectrightsrequest-getfinalattachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/subjectrightsrequest-getfinalattachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 302 
```

