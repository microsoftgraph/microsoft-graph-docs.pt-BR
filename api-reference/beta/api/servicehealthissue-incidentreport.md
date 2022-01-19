---
title: 'serviceHealthIssue: incidentReport'
description: Forneça o documento PIR (Revisão pós-incidente) de um problema de serviço especificado para locatário.
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 122ec4726d3dc89483d76d80e3848526e67a099a
ms.sourcegitcommit: bfd1ab7e015ef04cb2ca3fb85d308ba2ce830a89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/19/2022
ms.locfileid: "62072401"
---
# <a name="servicehealthissue-incidentreport"></a>serviceHealthIssue: incidentReport
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Forneça o documento PIR (Revisão pós-incidente) de um problema de serviço especificado para locatário.

Um problema apenas com o status de `PostIncidentReviewPublished` indica que o documento PIR existe para o problema. A operação retornará um erro se o problema especificado não existir para o locatário ou se o documento PIR não existir para o problema.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|ServiceHealth.Read.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|ServiceHealth.Read.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/issues/{serviceHealthIssueId}/incidentReport
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, essa função retornará um código de resposta e um `200 OK` fluxo de arquivos no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MO248163"],
  "name": "servicehealthissue_incidentreport"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/issues/MO248163/incidentReport
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/servicehealthissue-incidentreport-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/servicehealthissue-incidentreport-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/servicehealthissue-incidentreport-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/servicehealthissue-incidentreport-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



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
Content-Type: application/json

{
  "value": "Stream"
}
```

