---
title: tipo de recurso calendar
description: Um calendário que é um contêiner para eventos. Pode ser um calendário para um usuário ou o calendário padrão de um grupo do Microsoft 365.
localization_priority: Priority
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 47a63319efea2bdcdf11728bbac7d17903c6590a
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895703"
---
# <a name="calendar-resource-type"></a>tipo de recurso calendar

Namespace: microsoft.graph

Um calendário que é um contêiner para eventos. Pode ser um calendário para um [usuário](user.md)ou o calendário padrão de um [grupo](group.md)do Microsoft 365.

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
|[Atualizar](../api/calendar-update.md) | [calendar](calendar.md)  |Atualize as propriedades de um objeto **calendar**. O calendário pode ser um para um usuário ou o calendário padrão de um grupo do Microsoft 365. |
|[Excluir](../api/calendar-delete.md) | Nenhum |Exclua um objeto calendar. |
|[Listar calendarView](../api/calendar-list-calendarview.md) |Coleção [event](event.md)| Obtenha as ocorrências, as exceções e as instâncias de eventos únicas em uma visão de calendário definida por um intervalo de tempo, do calendário principal do usuário `(../me/calendarview)` ou de um calendário especificado.|
|[Listar eventos](../api/calendar-list-events.md) |Coleção [event](event.md)| Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.|
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
|allowedOnlineMeetingProviders|coleção de cadeias de caracteres| Represente os provedores de serviços de reunião online que podem ser usados para criar reuniões online neste calendário. Os valores possíveis são: `unknown`, `skypeForBusiness`, `skypeForConsumer`, `teamsForBusiness`.|
|canEdit |Boolean |True if the user can write to the calendar, false otherwise. This property is true for the user who created the calendar. This property is also true for a user who has been shared a calendar and granted write access. |
|canShare |Boolean |True if the user has the permission to share the calendar, false otherwise. Only the user who created the calendar can share it. |
|canViewPrivateItems |Boolean |Verdadeira se o usuário pode ler itens do calendário que foram marcados como particulares, falsa caso contrário. |
|changeKey|String|Identifies the version of the calendar object. Every time the calendar is changed, changeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.|
|color|calendarColor|Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1|
|defaultOnlineMeetingProvider|onlineMeetingProviderType|O provedor de reunião online padrão para reuniões enviadas deste calendário. Os valores possíveis são: `unknown`, `skypeForBusiness`, `skypeForConsumer`, `teamsForBusiness`.|
|id|String|The calendar's unique identifier. Read-only.|
|isRemovable|Booliano| Indica se o calendário deste usuário pode ser excluído da caixa de correio do usuário.|
|isTallyingResponses|Booliano|Indica se o calendário deste usuário dá suporte ao acompanhamento de respostas de reunião. Somente os convites para reuniões enviados do calendário principal do usuário oferecem suporte para respostas de reunião.|
|nome|String|O nome do calendário.|
|owner |[emailAddress](emailaddress.md) | If set, this represents the user who created or added the calendar. For a calendar that the user created or added, the **owner** property is set to the user. For a calendar shared with the user, the **owner** property is set to the person who shared that calendar with the user. |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|calendarPermissions|Coleção de [calendarPermission](calendarpermission.md)| As permissões dos usuários com os quais o calendário é compartilhado.|
|calendarView|Coleção [Event](event.md)|The calendar view for the calendar. Navigation property. Read-only.|
|events|Coleção [Event](event.md)|The events in the calendar. Navigation property. Read-only.|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| The collection of multi-value extended properties defined for the calendar. Read-only. Nullable.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| The collection of single-value extended properties defined for the calendar. Read-only. Nullable.|

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
  "id": "string (identifier)",
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
