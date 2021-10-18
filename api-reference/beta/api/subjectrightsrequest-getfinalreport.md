---
title: 'subjectRightsRequest: getFinalReport'
description: Obter o relatório final de uma solicitação de direitos de assunto.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 6ca3e10d75a5cf4bc670b516e647d36fac490504
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60447023"
---
# <a name="subjectrightsrequest-getfinalreport"></a>subjectRightsRequest: getFinalReport
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter o relatório final de uma solicitação de direitos de assunto. O relatório é um arquivo de texto que contém informações sobre os arquivos incluídos pelo administrador de privacidade.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|SubjectRightsRequest.Read.All *, SubjectRightsRequest.ReadWrite.All*|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte|

>[!IMPORTANT]
>No momento, as permissões marcadas com um asterisco (*) não estão disponíveis.  Para mais detalhes, confira [Problemas conhecidos](/graph/known-issues#compliance).

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /privacy/subjectRightsRequests{subjectRightsRequestId}/getFinalReport
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, essa função retornará `200 OK` um código de resposta e um Stream no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "subjectRightsRequest_getfinalreport"
}
-->
``` http
GET https://graph.microsoft.com/beta/privacy/subjectRightsRequests/{subjectRightsRequestId}/getFinalReport
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Edm.Stream"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Id, Workload, Size, ImmutableId, FileName, FilePath, ItemUrl
```

