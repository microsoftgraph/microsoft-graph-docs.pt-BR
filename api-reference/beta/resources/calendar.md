---
title: tipo de recurso calendar
description: Um calendário que é um contêiner para eventos. Pode ser um calendário para um usuário ou o calendário padrão de um grupo do Office 365.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 169e400609e6e6405369b65693e9a17625111e12
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778639"
---
# <a name="calendar-resource-type"></a>tipo de recurso calendar

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um calendário que é um contêiner para eventos. Pode ser um calendário para um [usuário](user.md) ou o calendário padrão de um [grupo](group.md) do Office 365.

> **Observação:** existem algumas pequenas diferenças na maneira como você pode interagir com calendários de usuários e calendários de grupos:

- Você pode organizar apenas os calendários de usuários em [calendarGroup](calendargroup.md).
- O Outlook aceita automaticamente todas as solicitações de reunião em nome de grupos. Você pode [aceitar](../api/event-accept.md), [aceitar provisoriamente](../api/event-tentativelyaccept.md) ou [recusar](../api/event-decline.md) solicitações de reuniões apenas para calendários do usuário.
- O Outlook não oferece suporte a lembretes de eventos do grupo. Você pode [adiar](../api/event-snoozereminder.md) ou [descartar](../api/event-dismissreminder.md) um [lembrete](reminder.md) apenas para calendários do usuário.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar calendários](../api/user-list-calendars.md)|Coleção [calendar](calendar.md)|Obtenha todos os calendários do usuário ou os calendários no grupo de calendários padrão ou em outro grupo de calendários específico.|
|[Criar calendário](../api/user-post-calendars.md) |[calendar](calendar.md)| Crie um novo calendário no grupo de calendário padrão ou no grupo de calendários especificado para um usuário.|
|[Obter calendário](../api/calendar-get.md) | [calendar](calendar.md) |Obtenha as propriedades e as relações de um objeto **calendar**. O calendário pode ser um para um usuário ou o calendário padrão de um grupo do Office 365. |
|[Atualizar](../api/calendar-update.md) | [calendar](calendar.md)  |Atualize as propriedades de um objeto **calendar**. O calendário pode ser um para um usuário ou o calendário padrão de um grupo do Office 365. |
|[Excluir](../api/calendar-delete.md) | Nenhum |Exclua um objeto calendar. |
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
|canEdit |Boolean |Verdadeira se o usuário pode gravar o calendário, falsa caso contrário. Essa propriedade é verdadeira para o usuário que criou o calendário. Esta propriedade também é verdadeira para um usuário com o qual tenha sido compartilhado um calendário e tenha sido concedido acesso de gravação. |
|canShare |Boolean |Verdadeira se o usuário tem permissão para compartilhar o calendário, falsa caso contrário. Somente o usuário que criou o calendário pode compartilhá-lo. |
|canViewPrivateItems |Boolean |Verdadeira se o usuário pode ler itens do calendário que foram marcados como particulares, falsa caso contrário. |
|changeKey|String|Identifica a versão do objeto calendar. Toda vez que o calendário é alterado, a changeKey também muda. Isso permite que o Exchange aplique as alterações na versão correta do objeto. Somente leitura.|
|color|String|Especifica o tema de cores para distinguir o calendário de outros calendários em uma interface do usuário. Os valores de propriedade são: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1|
|hexColor|String|Uma cor que representa o calendário. A cor é representada por um número hexadecimal de 6 dígitos e 3 bytes. Cada byte representa um dos componentes vermelho, verde e azul da cor, no intervalo de 00 a FF na notação hexadecimal. |
|id|String|O identificador exclusivo do grupo. Somente leitura.|
|isDefaultCalendar|Booliano|True se esse calendário for o calendário padrão do usuário, caso contrário, será false.|
|isShared |Booliano |True se o usuário tiver compartilhado o calendário com outros usuários. Caso contrário, será false. Como apenas o usuário que criou o calendário pode compartilhá-lo, ** isShared ** e ** isSharedWithMe ** não podem ser verdadeiros para o mesmo usuário. |
|isSharedWithMe |Booliano |True se o usuário tiver compartilhado este calendário, caso contrário, será false. Essa propriedade sempre será false para o proprietário de um calendário.  |
|name|String|O nome do calendário.|
|owner |[emailAddress](emailaddress.md) | Se definida, representa o usuário que criou ou adicionou o calendário. Para um calendário que o usuário criou ou adicionou, a propriedade **owner** é definida para o usuário. Para um calendário compartilhado com o usuário, a propriedade **owner** é definida para a pessoa que compartilhou o calendário com o usuário. |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|calendarView|Coleção [event](event.md)|O modo de exibição do calendário. Propriedade de navegação. Somente leitura.|
|events|Coleção [event](event.md)|Os eventos do calendário. Propriedade de navegação. Somente leitura.|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para o calendário. Somente leitura. Anulável.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para a mensagem. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "calendarView",
    "events",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendar"
}-->

```json
{
  "canEdit": "boolean",
  "canShare": "boolean",
  "canViewPrivateItems": "boolean",
  "changeKey": "string",
  "color": "String",
  "hexColor": "String",
  "id": "string (identifier)",
  "isDefaultCalendar": "boolean",
  "isShared": "boolean",
  "isSharedWithMe": "boolean",
  "name": "string",
  "owner": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "calendar resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
