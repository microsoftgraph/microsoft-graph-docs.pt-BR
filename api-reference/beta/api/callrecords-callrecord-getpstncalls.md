---
title: 'callRecord: getPstnCalls'
description: Obter log de chamadas PSTN.
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: c70491399b564ef2d3daa8df33932f4728f87681
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58786905"
---
# <a name="callrecord-getpstncalls"></a>callRecord: getPstnCalls

Namespace: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter log de chamadas PSTN como uma coleção de [entradas pstnCallLogRow.](../resources/callrecords-pstncalllogrow.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Sem suporte. |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Application                            | CallRecord-PstnCalls.Read.All, CallRecords.Read.All |

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
|fromDateTime|DateTimeOffset|Início do intervalo de tempo para consulta. UTC, inclusive.<br/>O intervalo de tempo se baseia na hora de início da chamada.|
|toDateTime|DateTimeOffset|Fim do intervalo de tempo para consulta. UTC, inclusive.|

> [!IMPORTANT]
> Os **valores fromDateTime** **e toDateTime** não podem ser mais de um intervalo de datas de 90 dias.

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="response"></a>Resposta

Se tiver êxito, essa função retornará um código de resposta e uma coleção de entradas `200 OK` [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) no corpo da resposta.
  
Se houver mais de 1000 entradas no intervalo de datas, o corpo também incluirá um com uma URL para consultar a próxima página de entradas `@odata.NextLink` de chamada. A última página no intervalo de datas não tem `@odata.NextLink` . Para obter mais informações, [consulte paging Microsoft Graph data in your app](/graph/paging).

## <a name="example"></a>Exemplo

O exemplo a seguir mostra como obter uma coleção de registros para chamadas PSTN que ocorreram no intervalo de datas especificado. A resposta inclui enumerar o número de registros nesta primeira resposta e obter registros além `"@odata.count": 1000` `@odata.NextLink` dos primeiros 1000. Para a capacidade de leitura, a resposta mostra apenas uma coleção de 1 registro. Suponha que haja mais de 1000 chamadas nesse intervalo de datas.

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "callrecord_getpstncalls"
}
-->

``` http
GET https://graph.microsoft.com/beta/communications/callRecords/getPstnCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)
```

### <a name="response"></a>Resposta

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
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
            "inventoryType": "Subscriber",
            "operator": "Microsoft",
            "callDurationSource": "microsoft"
        }],
    "@odata.nextLink": "https://graph.microsoft.com/beta/communications/callRecords/getPstnCalls(from=2019-11-01,to=2019-12-01)?$skip=1000"
}
```

## <a name="see-also"></a>Confira também

* [Microsoft Teams relatório de uso PSTN](/microsoftteams/teams-analytics-and-reports/pstn-usage-report).
* [Relatório de roteamento direto no Microsoft Graph](callrecords-callrecord-getdirectroutingcalls.md).
