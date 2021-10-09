---
title: tipo de recurso de evento
description: Um evento em um calendário.
author: Harini84
ms.localizationpriority: high
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 355ecee7c0292d29059695631eeb7ae21736a4f5
ms.sourcegitcommit: 6cea9bc17d3859e475a74c4a6f661f848e837e89
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/08/2021
ms.locfileid: "60240954"
---
# <a name="event-resource-type"></a>tipo de recurso de evento

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um evento em um calendário de [usuário](user.md) ou o calendário padrão de um [grupo](group.md) do Microsoft 365.

O número máximo de participantes incluídos em um **evento** e o número máximo de destinatários em um [eventMessage](eventmessage.md) enviado de uma caixa de correio do Exchange Online é 500. Para obter mais informações, consulte [limites de envio](/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#sending-limits).

Esse recurso permite:

- Adicionar seus próprios dados às propriedades personalizadas como [extensions](/graph/extensibility-overview).
- Assinar as [notificações de alteração](/graph/webhooks).
- Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/event-delta.md).

> **Observação:** existem algumas pequenas diferenças na maneira como você pode interagir com calendários de usuários, calendários de grupos e seus eventos:

- Você pode organizar apenas os calendários de usuários em [calendarGroup](calendargroup.md).
- Você pode adicionar objetos [anexos](attachment.md) a apenas eventos de calendários de usuário, mas não a eventos em calendários de grupo.
- O Outlook aceita automaticamente todas as solicitações de reunião em nome de grupos. Você pode [aceitar](../api/event-accept.md), [aceitar provisoriamente](../api/event-tentativelyaccept.md) ou [recusar](../api/event-decline.md) solicitações de reuniões apenas para calendários do _usuário_.
- O Outlook não oferece suporte a lembretes de eventos do grupo. Você pode [adiar](../api/event-snoozereminder.md) ou [descartar](../api/event-dismissreminder.md) um [lembrete](reminder.md) apenas para calendários de _usuário_.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar eventos](../api/user-list-events.md)|[Event](event.md) collection |Recuperar uma lista de objetos [event](../resources/event.md) na caixa de correio do usuário. A lista contém reuniões de instância única e reuniões mestres em série.|
|[Criar evento](../api/user-post-events.md) |[event](event.md)| Criar um novo evento postando na coleção de instâncias.|
|[Obter evento](../api/event-get.md) | [event](event.md) |Ler as propriedades e as relações do objeto event.|
|[Atualizar](../api/event-update.md) | [event](event.md) |Atualizar o objeto event. |
|[Excluir](../api/event-delete.md) | Nenhum |Excluir o objeto event. |
|[delta](../api/event-delta.md)|Coleção [event](event.md)|Obtenha um conjunto de eventos que foram adicionados, excluídos ou atualizados em um **calendarView** (um intervalo de eventos) do calendário principal do usuário.|
|[forward](../api/event-forward.md)|Nenhum|Permite que o organizador ou os participantes de um evento de reunião encaminhe a solicitação de reunião para um novo destinatário.|
|[cancel](../api/event-cancel.md) | Nenhum | Enviar a mensagem de cancelamento do organizador para todos os participantes e cancelar a reunião específica. |
|[accept](../api/event-accept.md)|Nenhum|Aceite o evento específico em um calendário do usuário.|
|[tentativelyAccept](../api/event-tentativelyaccept.md)|Nenhum|Aceitar provisoriamente o evento específico em um calendário de usuário.|
|[decline](../api/event-decline.md)|Nenhum|Recusar o convite para o evento específico em um calendário de usuário.|
|[dismissReminder](../api/event-dismissreminder.md)|Nenhum|Descarte o lembrete do evento específico em um calendário de usuário.|
|[snoozeReminder](../api/event-snoozereminder.md)|Nenhum|Adie um lembrete de evento específico em um calendário do usuário até um novo horário.|
|[List instances](../api/event-list-instances.md) |[Event](event.md) collection| Obtenha uma coleção do objeto Event.|
|**Anexos**| | |
|[Listar anexos](../api/event-list-attachments.md) |[Attachment](attachment.md) collection| Obtenha todos os anexos em um evento.|
|[Add attachment](../api/event-post-attachments.md) |[Attachment](attachment.md)| Adicione um novo anexo a um evento postando na coleção attachments.|
|**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Crie uma extensão aberta e adicione propriedades personalizadas a uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension-get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obtenha uma extensão aberta identificada pelo nome da extensão.|
|**Extensões de esquema**| | |
|[Adicionar valores de extensões de esquema](/graph/extensibility-schema-groups) || Cria uma definição para a extensão de esquema e usa-a para adicionar dados digitados personalizados a um recurso.|
|**Propriedades estendidas**| | |
|[Criar uma propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[event](event.md)  |Criar uma ou mais propriedades estendidas de valor único em um evento novo ou existente.   |
|[Obter evento com propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-get.md)  | [event](event.md) | Obter eventos que contenham uma propriedade estendida de valor único usando `$expand` ou `$filter`. |
|[Criar propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [event](event.md) | Criar uma ou mais propriedades estendidas de vários valores em um evento novo ou existente.  |
|[Obter evento com propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-get.md)  | [event](event.md) | Obter um evento que contenha uma propriedade estendida de vários valores usando `$expand`. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo |Descrição|
|:---------------|:--------|:----------|
|allowNewTimeProposals| Booliano | `true` se o organizador da reunião permitir que os convidados proponham um novo horário ao responder; caso contrário, `false`. Opcional. O padrão é `true`. |
|attendees|[Attendee](attendee.md) collection|A coleção de participantes do evento.|
|corpo|[ItemBody](itembody.md)|O corpo da mensagem associada ao evento. Pode estar no formato HTML ou no formato de texto.|
|bodyPreview|String|A visualização da mensagem associada ao evento. Está no formato de texto.|
|cancelledOccurrences|Coleção de cadeia de caracteres|Contém os valores da propriedade **occurrenceId** de instâncias canceladas em uma série recorrente, se o evento for o mestre da série. As instâncias de uma série recorrente que estão canceladas são chamadas de cancelledOccurences.<br><br>Devolvido somente no $select em uma operação[Get](../api/event-get.md) que especifica a identidade de uma sériede eventos mestre (ou seja, o valor da propriedade seriesMasterId).|
|categories|Coleção de cadeias de caracteres|As categorias associadas ao evento. Cada categoria corresponde à propriedade **displayName** de um [outlookCategory](outlookcategory.md) definido para o usuário.|
|changeKey|String|Identifica a versão do objeto event. Toda vez que o evento muda, ChangeKey também muda. Isso permite que o Exchange aplique alterações à versão correta do objeto.|
|createdDateTime|DateTimeOffset|O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|end|[DateTimeTimeZone](datetimetimezone.md)|A data, a hora e o fuso horário em que o evento termina. Por padrão, a hora de término é em UTC.|
|exceptionOccurrences|Coleção de cadeia de caracteres|Contém os valores da propriedade **id** das instâncias de evento que são exceções em uma série recorrente.<br>As exceções podem diferir das outras ocorrências em uma série recorrente, tais como o assunto, o início ou fim do horário, ou os participantes. As exceções não incluem as ocorrências canceladas.<br><br>Devolvido somente em $select e $expand em uma operação [GET](../api/event-get.md) que especifica a identidade de uma série de eventos mestre (ou seja, o valor da propriedade seriesMasterId).|
|hasAttachments|Booliano|Defina como true se o evento tiver anexos.|
|hideAttendees|Booliano|Quando definido como `true`, cada participante só se vê na solicitação de reunião e na lista de **Rastreamento** da reunião. O padrão é falso.|
|iCalUId|Cadeia de caracteres|Um único identificador para um evento em todos os calendários. Esta identificação é diferente para cada ocorrência em uma série recorrente. Somente leitura.|
|id|Cadeia de caracteres| Identificador exclusivo do evento. [!INCLUDE [outlook-beta-id](../../includes/outlook-immutable-id.md)] Sensível a maiúsculas e minúsculas e somente leitura.|
|importância|importância|A importância do evento. Os valores possíveis são: `low`, `normal`, `high`.|
|isAllDay|Booliano|Defina como True se o evento durar o dia inteiro. Se estiver definido como True, independentemente de ser um evento de um ou de vários dias, a hora de início e término deve ser definida como meia-noite e estar no mesmo fuso horário.|
|isCancelled|Booliano|Defina como true se o evento tiver sido cancelado.|
|isDraft|Boleano|Defina como verdadeiro se o usuário atualizou a reunião no Outlook mas não enviou as atualizações aos participantes. Defina como falso se todas as alterações forem enviadas, ou se o evento for um compromisso sem participantes.|
|isOnlineMeeting|Booliano| `True` se esse evento tiver informações de reunião online (ou seja, **onlineMeeting** aponta para um recurso [onlineMeetingInfo](onlinemeetinginfo.md)), `false` contrário. O padrão é `false` (**onlineMeeting** é `null`). Opcional. <br> Depois de definir **isOnlineMeeting** como `true`, o Microsoft Graph Inicializa **onlineMeeting**. Subsequentemente, o Outlook ignora todas as alterações feitas em **isOnlineMeeting** e a reunião permanece disponível online. |
|isOrganizer|Booliano|Defina como verdadeiro se o proprietário do calendário (especificado pela propriedade do **proprietário** do [calendário](calendar.md)) for o organizador do evento (especificado pela propriedade do **organizador** do **evento**). Isso também se aplica se um representante organizou o evento em nome do proprietário.|
|isReminderOn|Booliano|Defina como true se um alerta estiver definido para lembrar o usuário sobre o evento.|
|lastModifiedDateTime|DateTimeOffset|O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|location|[Location](location.md)|O local do evento.|
|locations|[location](location.md) collection|Locais onde o evento é realizado ou onde participar. As propriedades **location** e **locations** sempre correspondem entre si. Se você atualizar a propriedade **location**, os locais anteriores na coleção **locations** deverão ser removidos e substituídos pelo novo valor **location**. |
|occurrenceId|Cadeia de caracteres|Um identificador para uma ocorrência em uma série de eventos recorrentes. Nulo se o evento não faz parte de uma série recorrente.<br><br>O formato do valor da propriedade é OID.{seriesMasterId-value}.{occurrence-start-date}. O fuso horário para {occurrence-start-date} é a propriedade recurrenceTimeZone definida para o [recurrenceRange](recurrencerange.md) correspondente.<br><br>Esta propriedade pode identificar qualquer ocorrência em uma série recorrente, incluindo uma ocorrência que foi modificada ou cancelada. Você pode usar esta propriedade para executar todas as operações suportadas pelas ocorrências na série recorrente.|
|onlineMeeting|[OnlineMeetingInfo](onlinemeetinginfo.md)| Detalhes para um participante ingressar na reunião online. O padrão é nulo. Somente leitura. <br>Depois de definir as propriedades **isOnlineMeeting** e **onlineMeetingProvider** para habilitar uma reunião online, o Microsoft Graph Inicializa **onlineMeeting**. Depois de definida, a reunião ficará disponível on-line e você não poderá alterar as propriedades **isOnlineMeeting**, **onlineMeetingProvider** e **onlineMeeting** novamente.|
|onlineMeetingProvider|onlineMeetingProviderType| Representa o provedor de serviços de reunião online. Por padrão, **onlineMeetingProvider** é `unknown`. Os valores possíveis são `unknown`, `teamsForBusiness`, `skypeForBusiness` e `skypeForConsumer`. Opcional. <br> Depois de definir **onlineMeetingProvider**, o Microsoft Graph Inicializa **onlineMeeting**. Em seguida, não será possível alterar **onlineMeetingProvider** novamente, e a reunião permanecerá disponível online. |
|onlineMeetingUrl|String|Um URL de uma reunião online. A propriedade só é definida quando um organizador especifica no Outlook que um evento é uma reunião online como o Skype.<br>Para acessar a URL para ingressar em uma reunião online, use **joinUrl** que é exposta por meio da propriedade **onlineMeeting** do **event**. A propriedade **onlineMeetingUrl** será preterida no futuro. |
|organizer|[Recipient](recipient.md)|O organizador do evento.|
|originalEndTimeZone|String|O fuso horário de término que foi definido quando o evento foi criado. Um valor de `tzone://Microsoft/Custom` indica que um fuso horário personalizado herdado foi definido no Outlook da área de trabalho.|
|originalStart|DateTimeOffset|Representa a hora de início de um evento quando ele é inicialmente criado como uma ocorrência ou exceção em uma série recorrente. Essa propriedade não é retornada para eventos que são instâncias individuais. As informações de data e hora são expressas no formato ISO 8601 e estão sempre em UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|originalStartTimeZone|String|O fuso horário de início que foi definido quando o evento foi criado. Um valor de `tzone://Microsoft/Custom` indica que um fuso horário personalizado herdado foi definido no Outlook para área de trabalho.|
|recurrence|[PatternedRecurrence](patternedrecurrence.md)|O padrão de recorrência do evento.|
|reminderMinutesBeforeStart|Int32|O número de minutos antes da hora de início do evento em que o alerta de lembrete ocorre.|
|responseRequested|Booliano|O padrão é true, representando que o organizador gostaria de ter um convidado para enviar uma resposta para o evento.|
|responseStatus|[ResponseStatus](responsestatus.md)|Indica o tipo de resposta enviada em resposta a uma mensagem de evento.|
|sensitivity|String| Os valores possíveis são: `normal`, `personal`, `private`, `confidential`.|
|seriesMasterId|String|A ID do item mestre da série recorrente se este evento for parte de uma série recorrente.|
|showAs|String|O status a ser exibido. Os possíveis valores são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.|
|iniciar|[DateTimeTimeZone](datetimetimezone.md)|A data, a hora e o fuso horário do evento. Por padrão, a hora de início é em UTC.|
|assunto|String|O texto da linha de assunto do evento.|
|transactionId|Cadeia de caracteres|Um identificador personalizado especificado por um aplicativo cliente para o servidor para evitar operações [POST](../api/calendar-post-events.md) redundantes caso o cliente tente criar o mesmo evento. Isso é útil quando a conectividade de rede baixa faz com que o cliente expire antes de receber uma resposta do servidor para a solicitação anterior de criação de evento do cliente. Depois de definir **transactionId** ao criar um evento, não será possível alterar a **transactionId** em uma atualização subsequente. Essa propriedade só será retornada em um conteúdo de resposta se um aplicativo a tiver definido. Opcional.|
|type|String|O tipo de evento. Os valores possíveis são: `singleInstance`, `occurrence`, `exception`, `seriesMaster`. Somente leitura|
|uid|Cadeia de Caracteres|Um identificador exclusivo para eventos de calendário. Para eventos recorrentes, o valor é o mesmo do mestre da série e todas as suas ocorrências, incluindo as exceções. Essa propriedade substituirá a propriedade iCalUid atual definida nos [recursos de evento](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true), que é diferente para cada instância de uma série.|
|webLink|String|A URL para abrir o evento no Outlook na Web.<br/><br/>O Outlook na Web abre o evento no navegador se você estiver conectado à sua caixa de correio. Caso contrário, o Outlook na Web solicitará que você entre.<br/><br/>Este URL não pode ser acessado a partir de um iFrame.|

> [!NOTE]
> A propriedade **webLink** especifica uma URL que abre o evento apenas em versões anteriores do Outlook na Web. Este é o formato da URL, com _{event-id}_ sendo o valor _**codificado na URL**_ da propriedade **id**:
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
| Relação | Tipo |Descrição|
|:---------------|:--------|:----------|
|attachments|[Attachment](attachment.md) collection|A coleção de anexos [fileAttachment](fileattachment.md), [ItemAttachment](itemattachment.md)e [referenceAttachment](referenceattachment.md) para o evento. Propriedade de navegação. Somente leitura. Anulável.|
|calendar|[Calendar](calendar.md)|O calendário que contém o evento. Propriedade de navegação. Somente leitura.|
|extensions|Coleção [Extension](extension.md)|A coleção de extensões abertas definidas para o evento. Anulável.|
|instances|[Event](event.md) collection|São as ocorrências de uma série recorrente, se o evento for um mestre de série. Esta propriedade inclui ocorrências que fazem parte do padrão de recorrência e de exceções que foram modificadas, mas não inclui ocorrências da série que foram canceladas. Propriedade de navegação. Somente leitura. Anulável.|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para o evento. Somente leitura. Anulável.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de valor único definidas para o evento. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
   "keyProperty": "id",
  "optionalProperties": [
    "attachments",
    "calendar",
    "extensions",
    "instances",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties"
  ],
  "@odata.type": "microsoft.graph.event"
}-->

```json
{
  "allowNewTimeProposals": "Boolean",
  "attendees": [{"@odata.type": "microsoft.graph.attendee"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "string",
  "cancelledOccurrences":["string"],
  "categories": ["string"],
  "changeKey": "string",
  "createdDateTime": "String (timestamp)",
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "exceptionOccurrences":["string"],
  "hasAttachments": true,
  "hideAttendees": false,
  "uid": "string",
  "id": "string (identifier)",
  "importance": "String",
  "isAllDay": true,
  "isCancelled": true,
  "isDraft": false,
  "isOnlineMeeting": true,
  "isOrganizer": true,
  "isReminderOn": true,
  "lastModifiedDateTime": "String (timestamp)",
  "location": {"@odata.type": "microsoft.graph.location"},
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "occurrenceId":"string",
  "onlineMeeting": {"@odata.type": "microsoft.graph.onlineMeetingInfo"},
  "onlineMeetingProvider": "string",
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
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }]
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
<!--
{
  "type": "#page.annotation",
  "description": "event resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
