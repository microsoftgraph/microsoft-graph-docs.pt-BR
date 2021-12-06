---
title: 'callRecord: getDirectRoutingCalls'
description: Obter um log de chamadas de roteamento direto.
author: williamlooney
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 4c8bcf937c929b5d6568d7e6f2961d7c63f511ad
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029662"
---
# <a name="callrecord-getdirectroutingcalls"></a>callRecord: getDirectRoutingCalls

Namespace: microsoft.graph.callRecords

Obter um log de chamadas de roteamento direto como uma coleção [de entradas directRoutingLogRow.](../resources/callrecords-directroutinglogrow.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Sem suporte. |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | CallRecord-PstnCalls.Read.All, CallRecords.Read.All |

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
|fromDateTime|DateTimeOffset|Início do intervalo de tempo para consulta. UTC, inclusive.<br/>O intervalo de tempo se baseia na hora de início da chamada.|
|toDateTime|DateTimeOffset|Fim do intervalo de tempo para consulta. UTC, inclusive.|

## <a name="response"></a>Resposta

Se tiver êxito, essa função retornará um código de resposta e uma coleção de entradas `200 OK` [directRoutingLogRow](../resources/callrecords-directroutinglogrow.md) no corpo da resposta.
  
Se houver mais de 1000 entradas no intervalo de datas, o corpo também incluirá um com uma URL para consultar a próxima página de entradas `@odata.NextLink` de chamada. A última página no intervalo de datas não tem `@odata.NextLink` . Para obter mais informações, [consulte paging Microsoft Graph data in your app](/graph/paging).

## <a name="example"></a>Exemplo

O exemplo a seguir mostra como obter uma coleção de registros para chamadas de roteamento direto que ocorreram no intervalo de datas especificado. A resposta inclui enumerar o número de registros nesta primeira resposta e obter registros além `"@odata.count": 1000` `@odata.NextLink` dos primeiros 1000. Para a capacidade de leitura, a resposta mostra apenas uma coleção de 1 registro. Suponha que haja mais de 1000 chamadas nesse intervalo de datas.

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "callrecord_getdirectroutingcalls"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/communications/callRecords/getDirectRoutingCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/callrecord-getdirectroutingcalls-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/callrecord-getdirectroutingcalls-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/callrecord-getdirectroutingcalls-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/callrecord-getdirectroutingcalls-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/callrecord-getdirectroutingcalls-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.callRecords.directRoutingLogRow",
  "isCollection": true
} 
-->

``` http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.callRecords.directRoutingLogRow)",
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
            "callerNumber": "+12345678***",
            "calleeNumber": "+01234567***",
            "mediaPathLocation": "USWE",
            "signalingLocation": "EUNO",
            "finalSipCode": 0,
            "callEndSubReason": 540000,
            "finalSipCodePhrase": "BYE",
            "trunkFullyQualifiedDomainName": "tll-audiocodes01.adatum.biz",
            "mediaBypassEnabled": false
        }],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/communications/callRecords/getDirectRoutingCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)?$skip=1000"
}
```

## <a name="see-also"></a>Confira também

* [Microsoft Teams relatório de uso de roteamento](/microsoftteams/teams-analytics-and-reports/pstn-usage-report#direct-routing) direto no Microsoft Teams de administração.
* [Painel de Saúde para roteamento](/MicrosoftTeams/direct-routing-health-dashboard) direto no Microsoft Teams de administração.
* [Relatório de chamada PSTN no Microsoft Graph](callrecords-callrecord-getpstncalls.md).
