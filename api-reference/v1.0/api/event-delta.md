---
title: 'evento: delta'
description: 'Obtém um conjunto de eventos que foram adicionados, excluídos ou atualizado em um **calendarView** (um intervalo de eventos) '
localization_priority: Priority
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f410ec6aee93e70596d811760833ac54366858ba
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514011"
---
# <a name="event-delta"></a>evento: delta

Namespace: microsoft.graph

Obtenha um conjunto de [eventos](../resources/event.md) recursos que foram adicionados, excluídos ou atualizados em um **calendárioView** (um intervalo de eventos definidos por datas de início e fim) do calendário principal do usuário.

Geralmente, sincronizar eventos em um **calendárioView** em uma repositório local implica em uma rodada de várias chamadas de função **delta**. A chamada inicial é uma sincronização completa, e cada chamada **delta** subsequente na mesma rodada recebe as alterações incrementais (acréscimos, exclusões ou atualizações). Isto permite manter e sincronizar uma repositório local de eventos no **calendárioView** especificado, sem ter que ir buscar todos os eventos desse calendário do servidor toda vez.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Calendars.Read    |
|Delegado (conta pessoal da Microsoft) | Calendars.Read    |
|Aplicativo | Calendars.Read |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}

```

## <a name="query-parameters"></a>Parâmetros de consulta

O controle de alterações em eventos corresponde a uma série de uma ou mais chamadas de função **delta**. Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**. O Microsoft Graph codifica automaticamente todos os parâmetros especificados na porção do token da URL `nextLink` ou `deltaLink` fornecida na resposta. Você só precisa especificar os parâmetros de consulta desejados uma vez antecipados. Em solicitações subsequentes, basta copiar e aplicar a URL `nextLink` ou `deltaLink` da resposta anterior já que essa URL inclui os parâmetros codificados desejados.


| Parâmetro de consulta      | Tipo   |Descrição|
|:---------------|:--------|:----------|
|startDateTime|String|A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T19:00:00.0000000".|
|endDateTime|String|A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T20:00:00.0000000".|
| $deltatoken | string | Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior do mesmo modo de exibição de calendário, indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle do modo de exibição de calendário.|
| $skiptoken | string | Um [token de estado](/graph/delta-query-overview) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas no mesmo modo de exibição de calendário. |

### <a name="odata-query-parameters"></a>Parâmetros de consulta OData
- Esperar uma **delta** chamada de função em um **calendárioView** para retornar as mesmas propriedades que você normalmente obteria de um `GET /calendarview` solicitação. Você não pode usar `$select` para obter apenas um subconjunto dessas propriedades.

- Existem outros parâmetros de consulta OData que a função **delta** para **calendarView** não suporta: `$expand`, `$filter`,`$orderby`, e `$search`. 


## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição |
|:---------------|:----------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |
| Content-Type  | string  | application/json. Obrigatório. |
| Preferir | cadeia de caracteres  | odata.maxpagesize={x}. Opcional. |
| Preferir | string | {Fuso horário}. Opcional, supõe-se o UTC se estiver ausente.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `200 OK` e uma coleção de objetos [event](../resources/event.md) no corpo da resposta.

Dentro de uma rodada de **delta** chamadas de função associadas ao intervalo de datas de um **calendárioView**, você pode encontrar uma **delta** chamada retornando dois tipos de eventos em `@removed` com o motivo `deleted`: 
- Eventos que estejam dentro do intervalo de datas e que tenham sido excluídos desde a chamada anterior **delta**.
- Eventos que estejam _fora_ do intervalo de datas e que tenham sido adicionados, excluídos ou atualizados desde a chamada anterior **delta**.

Filtre os eventos sob `@removed` para o intervalo de datas que seu cenário requer.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação

O exemplo a seguir mostra como fazer uma única chamada de função **delta** e limitar o número máximo de eventos no corpo da resposta a 2.

Para controlar as alterações em um modo de exibição de calendário, você faz uma ou mais chamadas de função **delta**, com os [tokens de estado](/graph/delta-query-overview) apropriados, para obter o conjunto de alterações incrementais desde a última consulta delta. 


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?startdatetime={start_datetime}&enddatetime={end_datetime}

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a>Resposta
Se a solicitação for bem-sucedida, a resposta incluiria um token de estado, que é um _skipToken_ (em um cabeçalho de resposta _@odata.nextLink_) ou um _deltaToken_ (em um cabeçalho de resposta _@odata.deltaLink_). Respectivamente, elas indicam se você deverá continuar com a série ou se já concluiu a obtenção de todas as alterações dessa série.

A resposta abaixo mostra um _skipToken_ em um cabeçalho de resposta _@odata.nextLink_.

Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 359

{
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "response-value",
        "time": "datetime-value"
      },
      "transactionId": null,
      "iCalUId": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isDraft": false,
      "isReminderOn": true
    }
  ]
}
```

## <a name="see-also"></a>Confira também

- [Usar a consulta delta para controlar alterações nos dados do Microsoft Graph](/graph/delta-query-overview)
- [Obter as alterações incrementais para os eventos em um calendário](/graph/delta-query-events)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

