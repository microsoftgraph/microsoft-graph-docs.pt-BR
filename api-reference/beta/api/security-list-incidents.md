---
title: Listar incidentes
description: Obter uma lista dos objetos de incidente e suas propriedades.
ms.date: 09/09/2021
author: BenAlfasi
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 1e0dd929000299770d3e5240905e17890ba2ae7e
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220815"
---
# <a name="list-incidents"></a>Listar incidentes
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter uma lista dos objetos [de incidente](../resources/incident.md) e suas propriedades.

A operação de incidentes de lista permite classificar incidentes para criar uma resposta de segurança cibernética informada. Ele expõe uma coleção de incidentes que foram sinalizados em sua rede, dentro do intervalo de tempo especificado na política de retenção do ambiente. Os incidentes mais recentes são exibidos na parte superior da lista.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|Incidents.Read.All, Incidents.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Incidents.Read.All, Incidents.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/incidents
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta: `$count` `$filter` , , , `$skip` `$top` .

As propriedades a seguir `$filter` suportam : **assignedTo**, **classification**, **createdDateTime**, **determination**, **lastUpdateDateTime**, **severity**, and **status**.

Use `@odata.nextLink` para paginação.

Veja a seguir exemplos de seu uso:

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/incidents?$count=true
GET /security/incidents?$filter={property}+eq+'{property-value}'
GET /security/incidents?$top=10
```

Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).


## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [de](../resources/incident.md) incidentes no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "list_incident"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/incidents
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.incident",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
        "@odata.type": "#microsoft.graph.incident",
        "id": "2972395",
        "incidentWebUrl": "https://security.microsoft.com/incidents/2972395?tid=12f988bf-16f1-11af-11ab-1d7cd011db47",
        "redirectIncidentId": null,
        "displayName": "Multi-stage incident involving Initial access & Command and control on multiple endpoints reported by multiple sources",
        "createdDateTime": "2021-08-13T08:43:35.5533333Z",
        "lastUpdateDateTime": "2021-09-30T09:35:45.1133333Z",
        "assignedTo": "KaiC@contoso.onmicrosoft.com",
        "classification": "TruePositive",
        "determination": "MultiStagedAttack",
        "status": "Active",
        "severity": "Medium",
        "tags": [
          "Demo"
        ],
        "comments": [
          {
                "comment": "Demo incident",
                "createdBy": "DavidS@contoso.onmicrosoft.com",
                "createdTime": "2021-09-30T12:07:37.2756993Z"
          }
        ]
    }
  ]
}
```

