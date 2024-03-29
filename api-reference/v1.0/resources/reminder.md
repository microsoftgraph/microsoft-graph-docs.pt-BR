---
title: Tipo de recurso reminder
description: Um lembrete para um evento em um calendário do usuário.
ms.localizationpriority: medium
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ae24d37e05d104faf83da1c5056237686b88dcf6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067028"
---
# <a name="reminder-resource-type"></a>Tipo de recurso reminder

Namespace: microsoft.graph

Um lembrete para um [evento](event.md) em um calendário do [usuário.](calendar.md)

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|changeKey|Cadeia de caracteres|Identifica a versão do lembrete. Toda vez que o lembrete é alterado, **changeKey** também muda. Isso permite que o Exchange aplique as alterações na versão correta do objeto.|
|eventEndTime|[DateTimeTimeZone](datetimetimezone.md)|A data, a hora e o fuso horário em que o evento termina.|
|eventId|String|A ID exclusiva do evento. Somente leitura.|
|eventLocation|[Location](location.md)|O local do evento.|
|eventStartTime|[DateTimeTimeZone](datetimetimezone.md)|A data, a hora e o fuso horário em que o evento começa.|
|eventSubject|String|O texto da linha de assunto do evento.|
|eventWebLink|String|A URL para abrir o evento no Outlook na Web.<br/><br/>O evento será aberto no navegador se você estiver conectado à sua caixa de correio através do Outlook na Web. Você será solicitado a fazer login se já não estiver conectado no navegador.<br/><br/>Este URL não pode ser acessado a partir de um iFrame.|
|reminderFireTime|[DateTimeTimeZone](datetimetimezone.md)|A data, a hora e o fuso horário do lembrete.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reminder"
}-->

```json
{
  "changeKey": "string",
  "eventEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventId": "string",
  "eventLocation": {"@odata.type": "microsoft.graph.location"},
  "eventStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventSubject": "string",
  "eventWebLink": "string",
  "reminderFireTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

