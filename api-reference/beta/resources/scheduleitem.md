---
title: tipo de recurso de scheduleItem
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: ed6b7441996cdf00b33be03f70afb888cc9bb251
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511349"
---
# <a name="scheduleitem-resource-type"></a>tipo de recurso de scheduleItem

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Um item que descreve a disponibilidade de um usuário correspondente a um evento real no calendário de padrão do usuário. Esse item se aplica a um recurso também.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|end |[dateTimeTimeZone](datetimetimezone.md) |A data, hora e fuso horário que termina o evento correspondente. |
|IsPrivate |Booliano |A sensibilidade do evento correspondente. True se o evento é marcado como `private`, false caso contrário. |
|location |String | O local onde o evento correspondente é mantido ou participou da. Opcional.|
|start |[dateTimeTimeZone](datetimetimezone.md) |A data, hora e fuso horário que inicia o evento correspondente. |
|status |String | O status de disponibilidade do usuário ou recurso durante o evento correspondente. Os valores possíveis são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`. |
|subject |Cadeia de caracteres | Linha de assunto do evento correspondente. Opcional.|


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
<!--
{
  "type": "#page.annotation",
  "description": "scheduleItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/scheduleitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
