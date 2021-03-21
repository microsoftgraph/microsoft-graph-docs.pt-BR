---
title: tipo de recurso calendar
description: Um calendário que é um contêiner para eventos. Pode ser um calendário para um usuário ou o calendário padrão de um grupo do Microsoft 365.
localization_priority: Priority
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d6d549435cd9350f9baf1136fd10f174eb1d0938
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952547"
---
# <a name="calendar-resource-type"></a>tipo de recurso calendar

Namespace: microsoft.graph

Um calendário que é um contêiner para eventos. Pode ser um calendário para um [usuário](user.md)ou o calendário padrão de um [grupo](group.md) do Microsoft 365.

> **Observação:** existem algumas pequenas diferenças na maneira como você pode interagir com calendários de usuários e calendários de grupos:

- Você pode organizar apenas os calendários de usuários em [calendarGroup](calendargroup.md).
- O Outlook aceita automaticamente todas as solicitações de reunião em nome de grupos. Você pode [aceitar](../api/event-accept.md), [aceitar provisoriamente](../api/event-tentativelyaccept.md) ou [recusar](../api/event-decline.md) solicitações de reuniões apenas para calendários do usuário.
- O Outlook não oferece suporte a lembretes de eventos do grupo. Você pode [adiar](../api/event-snoozereminder.md) ou [descartar](../api/event-dismissreminder.md) um [lembrete](reminder.md) apenas para calendários do usuário.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar calendários](../api/user-list-calendars.md)|Coleção [calendar](calendar.md)|Obtenha todos os calendários do usuário ou os calendários no grupo de calendários padrão ou em outro grupo de calendários específico.|
|[Criar calendário](../api/user-post-calendars.md) |[calendar](calendar.md)| Crie um novo calendário no grupo de calendário padrão ou no grupo de calendários especificado para um usuário.|
|[Obter calendário](../api/calendar-get.md) | [calendar](calendar.md) |Obtenha as propriedades e as relações de um objeto **calendar**. O calendário pode ser um para um usuário ou o calendário padrão de um grupo do Microsoft 365. |
|[Update](../api/calendar-update.md) | [calendar](calendar.md)  |Atualize as propriedades de um objeto **calendar**. O calendário pode ser um para um usuário ou o calendário padrão de um grupo do Microsoft 365. |
|[Delete](../api/calendar-delete.md) | Nenhum |Exclua um objeto calendar. |
|[Listar calendarView](../api/calendar-list-calendarview.md) |Coleção [event](event.md)| Obtenha as ocorrências, as exceções e as instâncias de eventos únicas em uma visão de calendário definida por um intervalo de tempo, do calendário principal do usuário `(../me/calendarview)` ou de um calendário especificado.|
|[Listar eventos](../api/calendar-list-events.md) |Coleção [event](event.md)| Recupera uma lista de eventos em um calendário.  A lista contém reuniões de instância única e reuniões mestres da série.|
|[Criar evento](../api/calendar-post-events.md) |[event](event.md)| Crie um novo evento no calendário especificado ou padrão.|
|[getSchedule](../api/calendar-getschedule.md) |Coleção [scheduleInformation](scheduleinformation.md)|Obtenha as informações de disponibilidade para um conjunto de usuários, listas de distribuição ou recursos para um período especificado. |
|[findMeetingTimes](../api/user-findmeetingtimes.md) |[meetingTimeSuggestionsResult](meetingtimesuggestionsresult.md) |Sugira horários e locais para a reunião com base no organizador e na disponibilidade dos participantes, além de restrições de horário ou local. |
|[Criar uma propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[calendar](calendar.md)  |Criar uma ou mais propriedades estendidas de valor único em um calendário novo ou existente.   |
|[Obter calendário com propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-get.md)  | [calendar](calendar.md) | Obter calendários que contenham uma propriedade estendida de valor único usando `$expand` ou `$filter`. |
|[Criar propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [calendar](calendar.md) | Criar uma ou mais propriedades estendidas de vários valores em um calendário novo ou existente.  |
|[Obter calendário com propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-get.md)  | [calendar](calendar.md) | Obter um calendário que contenha uma propriedade estendida de vários valores usando `$expand`. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|allowedOnlineMeetingProviders|onlineMeetingProviderType collection| Represente os provedores de serviços de reunião online que podem ser usados para criar reuniões online neste calendário. Os valores possíveis são: `unknown`, `skypeForBusiness`, `skypeForConsumer`, `teamsForBusiness`.|
|canEdit |Booliano |`true` se o usuário pode escrever no calendário, `false` caso contrário. Esta propriedade é `true` para o usuário que criou o calendário. Esta propriedade também é `true` para um usuário que compartilhou uma agenda e recebeu acesso de gravação. |
|canShare |Boolean |`true` se o usuário tiver permissão para compartilhar a agenda, `false` caso contrário. Apenas o usuário que criou o calendário pode compartilhá-lo. |
|canViewPrivateItems |Boolean |`true` se o usuário pode ler itens de calendário que foram marcados como privados, `false` caso contrário. |
|changeKey|String|Identifica a versão do objeto calendar. Toda vez que o calendário é alterado, a changeKey também muda. Isso permite que o Exchange aplique as alterações na versão correta do objeto. Somente leitura.|
|color|calendarColor|Especifica o tema de cores para distinguir o calendário de outros calendários em uma interface do usuário. Os valores das propriedades são: `auto`, `lightBlue`, `lightGreen`, `lightOrange`, `lightGray`, `lightYellow`, `lightTeal`, `lightPink`, `lightBrown`, `lightRed`, `maxColor`|
|defaultOnlineMeetingProvider|onlineMeetingProviderType|O provedor de reunião online padrão para reuniões enviadas deste calendário. Os valores possíveis são: `unknown`, `skypeForBusiness`, `skypeForConsumer`, `teamsForBusiness`.|
|hexColor |String |A cor do calendário, expressa em um código de cor hexadecimal de três valores hexadecimais, cada um variando de 00 a FF e representando os componentes vermelho, verde ou azul da cor no espaço de cores RGB. Se o usuário nunca tiver definido explicitamente uma cor para o calendário, esta propriedade estará vazia. Somente leitura.|
|id|String|O identificador exclusivo do calendário. Somente leitura.|
|isDefaultCalendar|Booliano|`true` se este for o calendário padrão onde novos eventos são criados por padrão, `false` caso contrário.|
|isRemovable|Booliano| Indica se o calendário deste usuário pode ser excluído da caixa de correio do usuário.|
|isTallyingResponses|Booliano|Indica se o calendário deste usuário dá suporte ao acompanhamento de respostas de reunião. Somente os convites para reuniões enviados do calendário principal do usuário oferecem suporte para respostas de reunião.|
|nome|String|O nome do calendário.|
|owner |[emailAddress](emailaddress.md) | Se definida, representa o usuário que criou ou adicionou o calendário. Para um calendário que o usuário criou ou adicionou, a propriedade **owner** é definida para o usuário. Para um calendário compartilhado com o usuário, a propriedade **owner** é definida para a pessoa que compartilhou o calendário com o usuário. |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|calendarPermissions|Coleção de [calendarPermission](calendarpermission.md)| As permissões dos usuários com os quais o calendário é compartilhado.|
|calendarView|Coleção [Event](event.md)|O modo de exibição do calendário. Propriedade de navegação. Somente leitura.|
|events|Coleção [Event](event.md)|Os eventos do calendário. Propriedade de navegação. Somente leitura.|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para o calendário. Somente leitura. Anulável.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para a mensagem. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "calendarView",
    "events",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.calendar",
  "@odata.annotations": [
    {
      "property": "calendarView",
      "capabilities": {
        "changeTracking": true,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "events",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "allowedOnlineMeetingProviders": ["string"],
  "canEdit": "boolean",
  "canShare": "boolean",
  "canViewPrivateItems": "boolean",
  "changeKey": "string",
  "color": "String",
  "defaultOnlineMeetingProvider": "string",
  "hexColor": "String",
  "id": "string (identifier)",
  "isDefaultCalendar": "boolean",
  "isRemovable": "boolean",
  "isTallyingResponses": "boolean",
  "name": "string",
  "owner": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendar resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

