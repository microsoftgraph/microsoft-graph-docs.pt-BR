---
title: 'callRecord: getDirectRoutingCalls'
description: Obter um log de chamadas de roteamento direto.
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 5dd389ddba5e3f081b850e2303833b47b832e7d7
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872916"
---
# <a name="callrecord-getdirectroutingcalls"></a>callRecord: getDirectRoutingCalls

Namespace: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter um log de chamadas de roteamento direto como uma coleção de entradas [directRoutingLogRow.](../resources/callrecords-directroutinglogrow.md)

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
GET /communications/callRecords/getDirectRoutingCalls
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="function-parameters"></a>Parâmetros de função

Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.
A tabela a seguir mostra os parâmetros que podem ser usados com esta função.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|fromDateTime|DateTimeOffset|Início do intervalo de tempo para consulta. UTC, inclusive.<br/>O intervalo de tempo é baseado na hora de início da chamada.|
|toDateTime|DateTimeOffset|Fim do intervalo de tempo a ser consultado. UTC, inclusive.|

## <a name="response"></a>Resposta

Se bem-sucedida, esta função retorna um código de resposta e uma coleção de entradas `200 OK` [directRoutingLogRow](../resources/callrecords-directroutinglogrow.md) no corpo da resposta.
  
Se houver mais de 1.000 entradas no intervalo de datas, o corpo também incluirá um com uma URL para consultar a próxima página de entradas `@odata.NextLink` de chamada. A última página no intervalo de datas não tem `@odata.NextLink` . Para obter mais informações, consulte [paging dados do Microsoft Graph em seu aplicativo.](/graph/paging)

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "ignored",
  "name": "callrecord_getdirectroutingcalls"
}
-->

``` http
GET https://graph.microsoft.com/beta/communications/callRecords/getDirectRoutingCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)
```

### <a name="response"></a>Resposta

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.callRecords.directRoutingLogRow",
  "isCollection": true
} 
-->

``` http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.callRecords.directRoutingLogRow)",
    "@odata.count": 1000,
    "value": [{
            "id": "9e8bba57-dc14-533a-a7dd-f0da6575eed1",
            "correlationId": "c98e1515-a937-4b81-b8a8-3992afde64e0",
            "userId": "db03c14b-06eb-4189-939b-7cbf3a20ba27",
            "userPrincipalName": "richard.malk@contoso.com",
            "userDisplayName": "Richard Malk",
            "startDateTime": "2019-11-01T00:00:25.105Z",
            "inviteDateTime": "2019-11-01T00:00:21.949Z",
            "failureDateTime": "0001-01-01T00:00:00Z",
            "endDateTime": "2019-11-01T00:00:30.105Z",
            "duration": 5,
            "callType": "ByotIn",
            "successfulCall": true,
            "callerNumber": "+12345678**_",
            "calleeNumber": "+01234567_*_",
            "mediaPathLocation": "USWE",
            "signalingLocation": "EUNO",
            "finalSipCode": 0,
            "callEndSubReason": 540000,
            "finalSipCodePhrase": "BYE",
            "trunkFullyQualifiedDomainName": "tll-audiocodes01.adatum.biz",
            "mediaBypassEnabled": false
        }],
    "@odata.nextLink": "https://graph.microsoft.com/beta/communications/callRecords/getDirectRoutingCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)?$skip=1000"
}
```

## <a name="see-also"></a>Confira também

_ [Relatório de uso de roteamento direto do Microsoft Teams](/microsoftteams/teams-analytics-and-reports/pstn-usage-report#direct-routing) no centro de administração do Microsoft Teams
* [Painel de Saúde para roteamento direto](/MicrosoftTeams/direct-routing-health-dashboard) no centro de administração do Microsoft Teams
* [Relatório de chamada PSTN no Microsoft Graph](callrecords-callrecord-getpstncalls.md)