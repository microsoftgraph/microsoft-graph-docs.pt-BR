---
title: Listar eventos
description: Recupera uma lista de eventos em um calendário.  A lista contém reuniões de instância única e reuniões mestres da série.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: ba16ca364dddd0b13e889d36eabb2b3f467f3057
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264782"
---
# <a name="list-events"></a>Listar eventos

Recupera uma lista de eventos em um calendário.  A lista contém reuniões de instância única e reuniões mestres da série.

Para obter instâncias de evento expandidas, [obtenha a visualização de calendário](calendar-list-calendarview.md) ou [obtenha as instâncias de um evento](event-list-instances.md).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Calendars.Read    |
|Delegado (conta pessoal da Microsoft) | Calendars.Read    |
|Aplicativo | Calendars.Read |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição |
|:---------------|:--------|:--------|
| Autorização  | string | {token} de portador. Obrigatório.  |
| Prefira: outlook.timezone  | string | Use isto para especificar o fuso horário para horas de início e término na resposta. Se não especificado, esses valores de tempo serão retornados em UTC. Opcional. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/events
```
##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 354

{
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "",
        "time": "datetime-value"
      },
      "iCalUId": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
    }
  ]
}
```
#### <a name="sdk-sample-code"></a>Código de exemplo do SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/get_events-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_events-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Objective-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_events-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/calendar-list-events.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/calendar-list-events.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/calendar-list-events.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
