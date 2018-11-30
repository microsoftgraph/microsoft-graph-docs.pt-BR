---
title: tipo de recurso de scheduleItem
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: a7a31f47cde92549a72299b22a40b10c6f7845c6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038536"
---
# <a name="scheduleitem-resource-type"></a>tipo de recurso de scheduleItem

 > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.
 
Um item que descreve a disponibilidade de um usuário correspondente a um evento real no calendário de padrão do usuário. Esse item se aplica a um recurso também.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|end |[dateTimeTimeZone](datetimetimezone.md) |A data, hora e fuso horário que termina o evento correspondente. |
|isPrivate |Booliano |A sensibilidade do evento correspondente. True se o evento é marcado como `private`, false caso contrário. |
|location |String | O local onde o evento correspondente é mantido ou participou da. Opcional.|
|start |[dateTimeTimeZone](datetimetimezone.md) |A data, hora e fuso horário que inicia o evento correspondente. |
|status |String | O status de disponibilidade do usuário ou recurso durante o evento correspondente. Os valores possíveis são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`. |
|subject |String | Linha de assunto do evento correspondente. Opcional.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scheduleItem"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "isPrivate": true,
  "location": "String",
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String",
  "subject": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "scheduleItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->