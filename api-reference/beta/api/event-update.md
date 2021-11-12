---
title: Atualizar evento
description: Atualizar as propriedades do objeto evento.
author: harini84
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: dab816db63ef132ddb4e71f65c7f7cff9395e098
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60945550"
---
# <a name="update-event"></a>Atualizar evento

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualizar as propriedades do objeto [evento](../resources/event.md).

### <a name="notes-for-updating-specific-properties"></a>Observações para atualizar as propriedades específicas
Observe os seguintes comportamentos ou recomendações ao atualizar as propriedades correspondentes:

- atualizações de propriedade e reuniões dos **participantes**
  - Uma atualização de evento que inclui apenas a propriedade **participantes** no corpo da solicitação envia uma atualização de reunião apenas aos participantes que foram alterados.
  - Uma atualização de evento que remove um participante especificado como membro de uma lista de distribuição envia uma atualização de reunião a todos os participantes.

- propriedade do **corpo** e reuniões online

  Antes de atualizar o corpo de um evento que foi configurado como uma reunião online, primeiro deve-se obter a propriedade **corpo**, aplicar as alterações apropriadas ao conteúdo e preservar o blob de reunião para reunião online. Remover o blob de reunião do corpo de forma inadvertida desabilitará a reunião online. 

- propriedades **término** e **início** e seus fusos horários
  
  Ao atualizar o fuso horário da hora de início ou de término de um evento, primeiro [encontre os fusos horários com suporte](outlookuser-supportedtimezones.md) para garantir que você tenha definido apenas fusos horários que tenham sido configurados para o servidor de caixas de correio do usuário. 

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
| attendees|Participante|A coleção de participantes do evento. Consulte [observações adicionais para atualizar propriedades específicas](#notes-for-updating-specific-properties).|
| corpo|ItemBody|O corpo da mensagem associada ao evento. Consulte [observações adicionais para atualizar propriedades específicas](#notes-for-updating-specific-properties).|
| categories|Coleção de cadeias de caracteres|As categorias associadas ao evento.|
| end|DateTimeTimeZone|A data, a hora e o fuso horário em que o evento termina. Consulte [observações adicionais para atualizar propriedades específicas](#notes-for-updating-specific-properties). |
|hideAttendees|Booliano|Quando definido como `true`, cada participante só se vê na solicitação de reunião e na lista de **Rastreamento** da reunião. O padrão é falso.|
| importância|Cadeia de caracteres|A importância do evento. Os valores possíveis são: `low`, `normal` e `high`.|
| isAllDay|Booliano|Defina como True se o evento durar o dia inteiro. Se estiver definido como True, independentemente de ser um evento de um ou de vários dias, a hora de início e término deve ser definida como meia-noite e estar no mesmo fuso horário.|
|isOnlineMeeting|Booliano| `True` se o evento tem informações sobre a reunião online, caso contrário, `false`. O padrão é false. Opcional.|
| isReminderOn|Booliano|Defina como true se um alerta estiver definido para lembrar o usuário sobre o evento.|
| location|Local|O local do evento.|
|locations|[location](../resources/location.md) collection|Locais onde o evento é realizado ou onde participar. As propriedades **location** e **locations** sempre correspondem entre si. Se você atualizar a propriedade **location**, os locais anteriores na coleção **locations** deverão ser removidos e substituídos pelo novo valor **location**. |
|onlineMeetingProvider|onlineMeetingProviderType| Representa o provedor de serviços de reunião online. Os valores possíveis são `teamsForBusiness`, `skypeForBusiness` e `skypeForConsumer`. Opcional. |
| recurrence|PatternedRecurrence|O padrão de recorrência do evento.|
| reminderMinutesBeforeStart|Int32|O número de minutos antes da hora de início do evento em que o alerta de lembrete ocorre.|
| responseRequested|Booliano|Defina como true se o remetente quiser receber uma resposta quando o evento for aceito ou recusado.|
| sensitivity|String| Os valores possíveis são: `normal`, `personal`, `private`, `confidential`.|
| showAs|String|O status a ser exibido. Os valores possíveis `free` são: `tentative` , , , , , `busy` `oof` `workingElsewhere` `unknown` .|
| iniciar|DateTimeTimeZone|A data, a hora e o fuso horário do evento. Consulte [observações adicionais para atualizar propriedades específicas](#notes-for-updating-specific-properties). |
| assunto|String|O texto da linha de assunto do evento.|

Como o recurso **evento** dá suporte as [extensões](/graph/extensibility-overview), você pode usar a operação `PATCH` para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância do **evento** existente.

Se o **evento** que você está atualizando é o evento mestre de uma série recorrente, com vários participantes e com instâncias atualizadas separadamente, vários emails de notificação serão enviados: uma para a série mestre e um por instância que foi atualizada.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [event](../resources/event.md) atualizado no corpo da resposta.

>**Observação:** Esse método poderá retornar uma Resposta de Solicitação Incorreta HTTP 400 com um código de erro `ErrorOccurrenceCrossingBoundary` e a seguinte mensagem de erro: A ocorrência modificada está cruzando ou se sobrepondo à ocorrência adjacente. Isso indica que a atualização viola a seguinte restrição do Outlook nas exceções de recorrência: uma ocorrência não pode ser movida para ou antes do dia da ocorrência anterior e não pode ser movida para ou após o dia da ocorrência seguinte.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_event"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/events/{id}
Content-type: application/json

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
  "isOnlineMeeting": true,
  "onlineMeetingProvider": "teamsForBusiness",
  "isReminderOn": true,
  "hideAttendees": false,
  "categories": ["Red category"]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta

Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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
  "isOnlineMeeting": true,
  "onlineMeetingProvider": "teamsForBusiness",
  "isReminderOn": true,
  "hideAttendees": false,
  "onlineMeeting": {
        "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_NzIyNzhlMGEtM2YyZC00ZmY0LTlhNzUtZmZjNWFmZGNlNzE2%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22bc55b173-cff6-457d-b7a1-64bda7d7581a%22%7d",
        "conferenceId": "177513992",
        "tollNumber": "+91 22 6241 6885"
    }
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
