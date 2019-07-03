---
title: Atualizar evento
description: Atualizar as propriedades do objeto evento.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 911f15257ce10e628cb63db2ca4ee9517b5cbe81
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440936"
---
# <a name="update-event"></a>Atualizar evento

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualizar as propriedades do objeto [evento](../resources/event.md).
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Calendars.ReadWrite    |
|Delegado (conta pessoal da Microsoft) | Calendars.ReadWrite    |
|Aplicativo | Calendars.ReadWrite |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/events/{id}
PATCH /users/{id | userPrincipalName}/events/{id}
PATCH /groups/{id}/events/{id}

PATCH /me/calendar/events/{id}
PATCH /users/{id | userPrincipalName}/calendar/events/{id}
PATCH /groups/{id}/calendar/events/{id}

PATCH /me/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}/events/{id}

PATCH /me/calendargroup/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

PATCH /me/calendargroups/{id}/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade       | Tipo    | Descrição |
|:---------------|:--------|:------------|
| attendees|Attendee|A coleção de participantes do evento.|
| corpo|ItemBody|O corpo da mensagem associada ao evento.|
| categories|String|As categorias associadas ao evento.|
| end|DateTimeTimeZone|A data e a hora em que o evento termina.<br/><br/>Por padrão, a hora de término é em UTC. Você pode especificar um fuso horário opcional em EndTimeZone, expressar a hora de término nesse fuso horário e incluir uma diferença de tempo em relação a UTC. Se usar EndTimeZone, você deverá especificar um valor para StartTimeZone também.<br/><br/>Este exemplo especifica 25 de fevereiro de 2015, 21: 34 na Hora Padrão do Pacífico: "2015-02-25T21:34:00-08:00". |
| importance|Cadeia de caracteres|A importância do evento. Os valores possíveis são: `low`, `normal`, `high`.|
| isAllDay|Booliano|Defina como true se o evento durar o dia inteiro.|
| isReminderOn|Booliano|Defina como true se um alerta estiver definido para lembrar o usuário sobre o evento.|
| location|Locais|O local do evento.|
|locations|[location](../resources/location.md) collection|Locais onde o evento é realizado ou onde participar. As propriedades **location** e **locations** sempre correspondem entre si. Se você atualizar a propriedade **location**, os locais anteriores na coleção **locations** deverão ser removidos e substituídos pelo novo valor **location**. |
| recurrence|PatternedRecurrence|O padrão de recorrência do evento.|
| reminderMinutesBeforeStart|Int32|O número de minutos antes da hora de início do evento em que o alerta de lembrete ocorre.|
| responseRequested|Booliano|Defina como true se o remetente quiser receber uma resposta quando o evento for aceito ou recusado.|
| sensitivity|String| Os valores possíveis são: `normal`, `personal`, `private`, `confidential`.|
| showAs|String|O status a ser exibido. Os valores possíveis são `free` : `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`,.|
| iniciar|DateTimeTimeZone|A hora de início do evento. <br/><br/>Por padrão, a hora de início é em UTC. Você pode especificar um fuso horário opcional em StartTimeZone, expressar a hora de início no fuso horário correspondente e incluir uma diferença de tempo em relação a UTC. Se usar StartTimeZone, você deverá especificar um valor para EndTimeZone também.<br/><br/>Este exemplo especifica 25 de fevereiro de 2015, 19:34 na Hora Padrão do Pacífico: "2015-02-25T19:34:00-08:00".  |
| subject|String|O texto da linha de assunto do evento.|

Como o recurso **evento** dá suporte as [extensões](/graph/extensibility-overview), você pode usar a operação `PATCH` para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância do **evento** existente.

Se o **evento** que você está atualizando é o evento mestre de uma série recorrente, com vários participantes e com instâncias atualizadas separadamente, vários emails de notificação serão enviados: uma para a série mestre e um por instância que foi atualizada.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [event](../resources/event.md) atualizado no corpo da resposta.

>**Observação:** Esse método poderá retornar uma Resposta de Solicitação Incorreta HTTP 400 com um código de erro `ErrorOccurrenceCrossingBoundary` e a seguinte mensagem de erro: A ocorrência modificada está cruzando ou se sobrepondo à ocorrência adjacente. Isso indica que a atualização viola a seguinte restrição do Outlook nas exceções de recorrência: uma ocorrência não pode ser movida para ou antes do dia da ocorrência anterior e não pode ser movida para ou após o dia da ocorrência seguinte.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_event"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/events/{id}
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "recurrence": null,
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "recurrence": null,
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```


## <a name="see-also"></a>Confira também

- [Adicionar dados personalizados a recursos usando extensões](/graph/extensibility-overview)
- [Adicionar dados personalizados aos usuários usando extensões abertas (visualização)](/graph/extensibility-open-users)
- [Adicionar dados personalizados a grupos usando extensões do esquema (visualização)](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
