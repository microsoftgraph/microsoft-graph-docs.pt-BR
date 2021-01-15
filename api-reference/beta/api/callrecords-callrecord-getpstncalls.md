---
title: 'callRecord: getPstnCalls'
description: Obter log de chamadas PSTN.
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 6aa3c85c25373ecee98894ce0704b35a6de25cdb
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872909"
---
# <a name="callrecord-getpstncalls"></a>callRecord: getPstnCalls

Namespace: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter log de chamadas PSTN como uma coleção de entradas [pstnCallLogRow.](../resources/callrecords-pstncalllogrow.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Sem suporte. |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | CallRecords.Read.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /communications/callRecords/getPstnCalls
```

## <a name="function-parameters"></a>Parâmetros de função

Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.
A tabela a seguir mostra os parâmetros que podem ser usados com esta função.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|fromDateTime|DateTimeOffset|Início do intervalo de tempo para consulta. UTC, inclusive.<br/>O intervalo de tempo é baseado na hora de início da chamada.|
|toDateTime|DateTimeOffset|Fim do intervalo de tempo a ser consultado. UTC, inclusive.|

> [!IMPORTANT]
> Os **valores fromDateTime** **e toDateTime** não podem ser maiores do que um intervalo de datas de 90 dias.

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="response"></a>Resposta

Se tiver êxito, esta função retornará um código de resposta e uma coleção de entradas `200 OK` [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) no corpo da resposta.
  
Se houver mais de 1.000 entradas no intervalo de datas, o corpo também incluirá um com uma URL para consultar a próxima página de entradas `@odata.NextLink` de chamada. A última página no intervalo de datas não tem `@odata.NextLink` . Para obter mais informações, consulte [paging dados do Microsoft Graph em seu aplicativo.](/graph/paging)

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "ignored",
  "name": "callrecord_getpstncalls"
}
-->

``` http
GET https://graph.microsoft.com/beta/communications/callRecords/getPstnCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)
```

### <a name="response"></a>Resposta

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.callRecords.pstnCallLogRow)"
}
-->

``` http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.callRecords.pstnCallLogRow)",
    "@odata.count": 1000,
    "value": [{
            "id": "9c4984c7-6c3c-427d-a30c-bd0b2eacee90",
            "callId": "1835317186_112562680@61.221.3.176",
            "userId": "db03c14b-06eb-4189-939b-7cbf3a20ba27",
            "userPrincipalName": "richard.malk@contoso.com",
            "userDisplayName": "Richard Malk",
            "startDateTime": "2019-11-01T00:00:08.2589935Z",
            "endDateTime": "2019-11-01T00:03:47.2589935Z",
            "duration": 219,
            "charge": 0.00,
            "callType": "user_in",
            "currency": "USD",
            "calleeNumber": "+1234567890",
            "usageCountryCode": "US",
            "tenantCountryCode": "US",
            "connectionCharge": 0.00,
            "callerNumber": "+0123456789",
            "destinationContext": null,
            "destinationName": "United States",
            "conferenceId": null,
            "licenseCapability": "MCOPSTNU",
            "inventoryType": "Subscriber"
        }],
    "@odata.nextLink": "https://graph.microsoft.com/beta/communications/callRecords/getPstnCalls(from=2019-11-01,to=2019-12-01)?$skip=1000"
}
```

## <a name="see-also"></a>Confira também

* [Relatório de uso de PSTN do Microsoft Teams](/microsoftteams/teams-analytics-and-reports/pstn-usage-report)
* [Relatório de roteamento direto no Microsoft Graph](callrecords-callrecord-getdirectroutingcalls.md)
