---
title: tipo de recurso de participantInfo
description: Contém propriedades adicionais sobre a identidade dos participantes
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 94bbc587f26f8b5122571899eb235d9c1fc27e90
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870661"
---
# <a name="participantinfo-resource-type"></a>tipo de recurso de participantInfo

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Contém propriedades adicionais sobre a identidade dos participantes

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo                          | Descrição  |
|:---------------|:------------------------------|:-------------|
| identidade       | [identitySet](identityset.md) | O [identitySet](identityset.md) associado a esse participante. |
| languageId     | Cadeia de caracteres                        | A cadeia de caracteres de cultura do idioma. |
| região         | Cadeia de caracteres                        | Região do participante. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "languageId", "region"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
  "languageId": "String",
  "region": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
