---
title: tipo de recurso de mediaInfo
description: As informações de mídia usadas em ações para solicita.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 6fe2c49e86bac9d5961310694b21e9439a4896ab
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885600"
---
# <a name="mediainfo-resource-type"></a>tipo de recurso de mediaInfo

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

As informações de mídia usadas em ações para solicita.

## <a name="properties"></a>Propriedades
| Propriedade       | Tipo    | Descrição                      |
|:---------------|:--------|:---------------------------------|
| resourceId     | Cadeia de caracteres  | Identidade exclusiva do recurso. |
| URI            | Cadeia de caracteres  | Caminho para o recurso.            |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaInfo"
}-->
```json
{
  "resourceId": "String",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
