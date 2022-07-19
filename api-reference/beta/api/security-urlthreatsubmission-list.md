---
title: Listar urlThreatSubmissions
description: Obtenha uma lista dos objetos urlThreatSubmission e suas propriedades.
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 700184a6b08cec7b7eae95d3e83a977addfaf473
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856485"
---
# <a name="list-urlthreatsubmissions"></a>Listar urlThreatSubmissions
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha uma lista dos [objetos urlThreatSubmission](../resources/security-urlthreatsubmission.md) e suas propriedades.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|ThreatSubmission.Read,ThreatSubmission.ReadWrite,ThreatSubmission.Read.All,ThreatSubmission.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|ThreatSubmission.Read.All,ThreatSubmission.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/threatSubmission/urlThreats
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esse método dá `$filter`suporte a `$top`, e `$skipToken` `$count` para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de [objetos urlThreatSubmission](../resources/security-urlthreatsubmission.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "list_urlthreatsubmission"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/threatSubmission/urlThreats
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.urlThreatSubmission)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/threatSubmission/urlThreatSubmission/$entity",
      "@odata.type": "#microsoft.graph.urlThreatSubmission",
      "category": "phishing",  
      "id": "49c5ef5b-1f65-444a-e6b9-08d772ea2059",
      "createdDateTime": "2021-10-10T03:30:18.6890937Z",
      "contentType": "url",
      "webUrl": "http://phishing.contoso.com",
      "status": "running",
      "source": "administrator",
      "createdBy": {
        "user": {
          "identity": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
          "displayName": "Ronald Admin",
          "email": "tifc@a830edad9050849eqtpwbjzxodq.onmicrosoft.com"
        }
      },
      "result": {
        "detail": "underInvestigation"
      },
      "adminReview": null,
      "tenantId" : "39238e87-b5ab-4ef6-a559-af54c6b07b42"
    }
  ]
}
```

