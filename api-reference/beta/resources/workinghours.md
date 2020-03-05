---
title: Tipo de recurso workingHours
description: Representa os dias da semana e as horas de um fuso horário específico que o usuário trabalha.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: 67a61c5ca767f00c32bf568cea4e495d5b0909ac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519068"
---
# <a name="workinghours-resource-type"></a>Tipo de recurso workingHours

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os dias da semana e as horas de um fuso horário específico que o usuário trabalha.

Ter acesso ao horário de trabalho de um usuário é útil em cenários que lidam com o planejamento de atividades ou recursos. Você pode [obter](../api/user-get-mailboxsettings.md#example-3) e [definir](../api/user-update-mailboxsettings.md#example-2) o horário de trabalho de um usuário como parte das [configurações da caixa de correio](mailboxsettings.md) do usuário. 

Você pode optar por definir um fuso horário para seu horário de trabalho de maneira diferente do fuso horário definido no seu cliente do Outlook. Isso pode ser útil em casos como quando você viaja para um fuso horário diferente daquele no qual você normalmente trabalha. É possível configurar o cliente do Outlook  
no fuso horário de destino para que os valores de tempo do Outlook sejam exibidos no horário local enquanto você estiver lá.
Quando outras pessoas solicitarem reuniões de trabalho com você no seu local habitual de trabalho, elas ainda poderão respeitar seu horário de trabalho no fuso horário apropriado.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| daysOfWeek | coleção dayOfWeek | Os dias da semana em que o usuário trabalha. |
| startTime | Edm.TimeOfDay | A hora do dia em que o usuário começa a trabalhar. |
| endTime | Edm.TimeOfDay | A hora do dia em que o usuário para de trabalhar. |
| timeZone | [timeZoneBase](timezonebase.md) | O fuso horário ao qual o horário de trabalho se aplica. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workingHours"
}-->

```json
{
  "daysOfWeek": ["string"],
  "startTime": "string (TimeOfDay)",
  "endTime": "string (TimeOfDay)",
  "timeZone": {"@odata.type": "microsoft.graph.timeZoneBase"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workingHours resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
