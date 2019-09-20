---
title: tipo de recurso de evento
description: Um evento em um calendário.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 83bacdd688705596302d7ec5c0708924a3583d20
ms.sourcegitcommit: 471f07c30867658688bd932e06822be1bbcea360
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2019
ms.locfileid: "37036190"
---
# <a name="event-resource-type"></a>tipo de recurso de evento

Um evento em um calendário de [usuário](user.md) ou o calendário padrão de um [grupo](group.md) do Office 365.

O número máximo de participantes incluídos em um**evento**e o número máximo de destinatários em uma[eventMessage](eventmessage.md) enviada de uma caixa de correio no Exchange Online é 500. Para obter mais informações, veja [limites de envio](https://docs.microsoft.com/pt-BR/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#sending-limits).

Esse recurso permite:

- Adicionar seus próprios dados às propriedades personalizadas como [extensions](/graph/extensibility-overview).
- Assinar as [notificações de alteração](/graph/webhooks).
- Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/event-delta.md).

> **Observação:** existem algumas pequenas diferenças na maneira como você pode interagir com calendários de usuários, calendários de grupos e seus eventos:

- Você pode organizar apenas os calendários de usuários em [calendarGroup](calendargroup.md).
- O Outlook aceita automaticamente todas as solicitações de reunião em nome de grupos. Você pode [aceitar](../api/event-accept.md), [aceitar provisoriamente](../api/event-tentativelyaccept.md) ou [recusar](../api/event-decline.md) solicitações de reuniões apenas para calendários do _usuário_.
- O Outlook não oferece suporte a lembretes de eventos do grupo. Você pode [adiar](../api/event-snoozereminder.md) ou [descartar](../api/event-dismissreminder.md) um [lembrete](reminder.md) apenas para calendários de _usuário_.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar eventos](../api/user-list-events.md)|Coleção [event](event.md) |Recuperar uma lista de objetos [event](../resources/event.md) na caixa de correio do usuário. A lista contém reuniões de instância única e reuniões mestres em série.|
|[Criar evento](../api/user-post-events.md) |[event](event.md)| Criar um novo evento postando na coleção de instâncias.|
|[Obter evento](../api/event-get.md) | [event](event.md) |Ler as propriedades e as relações do objeto event.|
|[Atualizar](../api/event-update.md) | [event](event.md) |Atualizar o objeto event. |
|[Excluir](../api/event-delete.md) | Nenhum |Excluir o objeto event. |
|[accept](../api/event-accept.md)|Nenhum|Aceite o evento específico em um calendário do usuário.|
|[tentativelyAccept](../api/event-tentativelyaccept.md)|Nenhum|Aceitar provisoriamente o evento específico em um calendário de usuário.|
|[decline](../api/event-decline.md)|Nenhum|Recusar o convite para o evento específico em um calendário de usuário.|
|[delta](../api/event-delta.md)|Coleção [event](event.md)|Obtenha um conjunto de eventos que foram adicionados, excluídos ou atualizados em um **calendarView** (um intervalo de eventos) do calendário principal do usuário.|
|[dismissReminder](../api/event-dismissreminder.md)|Nenhum|Descarte o lembrete do evento específico em um calendário de usuário.|
|[snoozeReminder](../api/event-snoozereminder.md)|Nenhum|Adie um lembrete de evento específico em um calendário do usuário até um novo horário.|
|[List instances](../api/event-list-instances.md) |Coleção [event](event.md)| Obter as instâncias (ocorrências) de um evento para um intervalo de tempo especificado. Se o evento for do tipo `SeriesMaster`, isso retornará as exceções e ocorrências desse evento no intervalo de tempo especificado.|
|**Anexos**| | |
|[List attachments](../api/event-list-attachments.md) |Coleção [attachment](attachment.md)| Obtenha todos os anexos em um evento.|
|[Add attachment](../api/event-post-attachments.md) |[attachment](attachment.md)| Adicione um novo anexo a um evento postando na coleção attachments.|
|**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Criar uma extensão aberta e adicionar propriedades personalizadas em uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension-get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obter um ou mais objetos de extensão ou identificados por nome ou nome totalmente qualificado.|
|**Propriedades estendidas**| | |
|[Criar uma propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[event](event.md)  |Criar uma ou mais propriedades estendidas de valor único em um evento novo ou existente.   |
|[Obter evento com propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-get.md)  | [event](event.md) | Obter eventos que contenham uma propriedade estendida de valor único usando `$expand` ou `$filter`. |
|[Criar propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [event](event.md) | Criar uma ou mais propriedades estendidas de vários valores em um evento novo ou existente.  |
|[Obter evento com propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-get.md)  | [event](event.md) | Obter um evento que contenha uma propriedade estendida de vários valores usando `$expand`. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|attendees|Coleção [attendee](attendee.md)|A coleção de participantes do evento.|
|body|[itemBody](itembody.md)|O corpo da mensagem associada ao evento. Pode estar no formato HTML ou no formato de texto.|
|bodyPreview|String|A visualização da mensagem associada ao evento. Está no formato de texto.|
|categories|Coleção de cadeias de caracteres|As categorias associadas ao evento.|
|changeKey|String|Identifica a versão do objeto event. Toda vez que o evento muda, ChangeKey também muda. Isso permite que o Exchange aplique alterações à versão correta do objeto.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|end|[dateTimeTimeZone](datetimetimezone.md)|A data, a hora e o fuso horário em que o evento termina. Por padrão, a hora de término é em UTC.|
|hasAttachments|Booliano|Defina como true se o evento tiver anexos.|
|iCalUId|String|Um identificador exclusivo que é compartilhado por todas as instâncias de um evento em calendários diferentes. Somente leitura.|
|id|String| Somente leitura.|
|importância|importância|A importância do evento. Os valores possíveis são: `low`, `normal`, `high`.|
|isAllDay|Booliano|Defina como true se o evento durar o dia inteiro.|
|isCancelled|Booliano|Defina como true se o evento tiver sido cancelado.|
|isOrganizer|Booliano|Defina como true se o remetente da mensagem também for o organizador.|
|isReminderOn|Booliano|Defina como true se um alerta estiver definido para lembrar o usuário sobre o evento.|
|lastModifiedDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|location|[location](location.md)|O local do evento.|
|locations|Coleção [location](location.md)|Locais onde o evento é realizado ou onde participar. As propriedades **location** e **locations** sempre correspondem entre si. Se você atualizar a propriedade **location**, os locais anteriores na coleção **locations** deverão ser removidos e substituídos pelo novo valor **location**. |
|onlineMeetingUrl|String|Uma URL para uma reunião online. A propriedade só é definida quando um organizador especifica um evento como uma reunião online como o Skype. Somente leitura.|
|organizer|[recipient](recipient.md)|O organizador do evento.|
|originalEndTimeZone|String|O fuso horário de término que foi definido quando o evento foi criado. Um valor de `tzone://Microsoft/Custom` indica que um fuso horário personalizado herdado foi definido no Outlook para área de trabalho.|
|originalStart|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|originalStartTimeZone|String|O fuso horário de início que foi definido quando o evento foi criado. Um valor de `tzone://Microsoft/Custom` indica que um fuso horário personalizado herdado foi definido no Outlook para área de trabalho. |
|recurrence|[patternedRecurrence](patternedrecurrence.md)|O padrão de recorrência do evento.|
|reminderMinutesBeforeStart|Int32|O número de minutos antes da hora de início do evento em que o alerta de lembrete ocorre.|
|responseRequested|Booliano|Defina como true se o remetente quiser receber uma resposta quando o evento for aceito ou recusado.|
|responseStatus|[responseStatus](responsestatus.md)|Indica o tipo de resposta enviada em resposta a uma mensagem de evento.|
|sensitivity|sensibilidade| Os valores possíveis são: `normal`, `personal`, `private`, `confidential`.|
|seriesMasterId|String|A ID do item mestre da série recorrente se este evento for parte de uma série recorrente.|
|showAs|freeBusyStatus|O status a ser exibido. Os valores possíveis são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.|
|iniciar|[dateTimeTimeZone](datetimetimezone.md)|A data, a hora e o fuso horário em que o evento começa. Por padrão, a hora de início é em UTC.|
|assunto|String|O texto da linha de assunto do evento.|
|type|eventType|O tipo de evento. Os valores possíveis são: `singleInstance`, `occurrence`, `exception`, `seriesMaster`. Somente leitura.|
|webLink|String|A URL para abrir o evento no Outlook na Web.<br/><br/>O Outlook na Web abre o evento no navegador se você estiver conectado à sua caixa de correio. Caso contrário, o Outlook na Web solicitará que você entre.<br/><br/>Essa URL pode ser acessada de um iFrame.|

> [!NOTE]
> A propriedade**webLink** especifica uma URL que abre o evento apenas em versões anteriores do Outlook na Web. Estes são os formatos da URL, com _{event-id}_ sendo o valor _**codificado na URL**_ da propriedade**id**:
>
> * Para contas corporativas ou de estudante: `https://outlook.office365.com/owa/?itemid={event-id}&exvsurl=1&path=/calendar/item`
>
> * Para contas da Microsoft: `https://outlook.live.com/owa/?itemid={event-id}&exvsurl=1&path=/calendar/item`
>
> Para abrir o evento em uma versão atual do Outlook na Web, converta a URL em um dos seguintes formatos e use essa URL para abrir o evento: 
>
> * Para contas corporativas ou de estudante: `https://outlook.office365.com/calendar/item/{event-id}`
>
> * Para contas da Microsoft: `https://outlook.live.com/calendar/item/{event-id}`


## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|attachments|Coleção [attachment](attachment.md)|A coleção de anexos [fileAttachment](fileattachment.md) e [itemAttachment](itemattachment.md) do evento. Propriedade de navegação. Somente leitura. Anulável.|
|calendário|[calendar](calendar.md)|O calendário que contém o evento. Propriedade de navegação. Somente leitura.|
|extensions|Coleção [Extension](extension.md)|A coleção de extensões abertas definidas para o evento. Somente leitura. Anulável.|
|instances|Coleção [event](event.md)|As instâncias do evento. Propriedade de navegação. Somente leitura. Anulável.|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para o evento. Somente leitura. Anulável.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de valor único definidas para o evento. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "attachments",
    "calendar",
    "extensions",
    "instances",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.outlookItem",
  "@odata.type": "microsoft.graph.event",
  "@odata.annotations": [
    {
      "property": "attachments",
      "capabilities": {
        "changeTracking": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "calendar",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "extensions",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "instances",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "attendees": [{"@odata.type": "microsoft.graph.attendee"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "string",
  "categories": ["string"],
  "changeKey": "string",
  "createdDateTime": "String (timestamp)",
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "hasAttachments": true,
  "iCalUId": "string",
  "id": "string (identifier)",
  "importance": "String",
  "isAllDay": true,
  "isCancelled": true,
  "isOrganizer": true,
  "isReminderOn": true,
  "lastModifiedDateTime": "String (timestamp)",
  "location": {"@odata.type": "microsoft.graph.location"},
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "onlineMeetingUrl": "string",
  "organizer": {"@odata.type": "microsoft.graph.recipient"},
  "originalEndTimeZone": "string",
  "originalStart": "String (timestamp)",
  "originalStartTimeZone": "string",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "reminderMinutesBeforeStart": 1024,
  "responseRequested": true,
  "responseStatus": {"@odata.type": "microsoft.graph.responseStatus"},
  "sensitivity": "String",
  "seriesMasterId": "string",
  "showAs": "String",
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "subject": "string",
  "type": "String",
  "webLink": "string",

  "attachments": [ { "@odata.type": "microsoft.graph.attachment" } ],
  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "extensions": [ { "@odata.type": "microsoft.graph.extension" } ],
  "instances": [ { "@odata.type": "microsoft.graph.event" }],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]

}

```


## <a name="see-also"></a>Confira também

- [Usar a consulta delta para controlar alterações nos dados do Microsoft Graph](/graph/delta-query-overview)
- [Obter as alterações incrementais para os eventos em uma pasta](/graph/delta-query-events)
- [Adicionar dados personalizados a recursos usando extensões](/graph/extensibility-overview)
- [Adicionar dados personalizados aos usuários usando extensões abertas](/graph/extensibility-open-users)
- [Adicionar dados personalizados a grupos usando as extensões do esquema](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
