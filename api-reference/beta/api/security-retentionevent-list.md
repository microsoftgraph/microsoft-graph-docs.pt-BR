---
title: Listar retentionEvents
description: Obtenha uma lista dos objetos retentionEvent e suas propriedades.
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 9357bc4668f0b275a4c69025063e2542b4156f40
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447525"
---
# <a name="list-retentionevents"></a>Listar retentionEvents
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha uma lista dos objetos [retentionEvent](../resources/security-retentionevent.md) e suas propriedades.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|RecordsManagement.Read.All, RecordsManagement.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|RecordsManagement.Read.All, RecordsManagement.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/triggers/retentionEvents
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esse método dá suporte à expansão dos parâmetros de consulta OData para ajudar a personalizar a resposta. Por exemplo, para obter o tipo de evento, use `$expand=retentionEventType`. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de [objetos microsoft.graph.security.retentionEvent](../resources/security-retentionevent.md)  no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "list_retentionevent"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/triggers/retentionEvents
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.retentionEvent)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.security.retentionEvent",
      "id": "fcdbfb58-d0c6-85dd-d011-4e0ff9a6805d",
      "displayName": "String",
      "description": "String",
      "eventQueries": [
        {
          "@odata.type": "microsoft.graph.security.eventQueries"
        }
      ],
      "eventTriggerDateTime": "String (timestamp)",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "createdDateTime": "String (timestamp)",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "lastModifiedDateTime": "String (timestamp)",
      "eventPropagationResults": [
        {
          "@odata.type": "microsoft.graph.security.eventPropagationResult"
        }
      ],
      "eventStatus": {
        "@odata.type": "microsoft.graph.security.retentionEventStatus"
      },
      "lastStatusUpdateDateTime": "String (timestamp)"
    }
  ]
}
```
