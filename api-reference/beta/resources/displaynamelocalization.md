---
title: tipo de recurso displayNameLocalization
description: Fornece a capacidade de um administrador personalizar a cadeia de caracteres usada em uma experiência compartilhada do Microsoft 365.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 8ae6c62acfacfccd22cc9985386762a2f61a2bc7
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050852"
---
# <a name="displaynamelocalization-resource-type"></a>tipo de recurso displayNameLocalization

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece a capacidade de um administrador personalizar a cadeia de caracteres usada em uma experiência compartilhada do Microsoft 365.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|displayName   |String       | Se presente, o valor desse campo contém a cadeia de caracteres **DisplayName** que foi definida para o idioma presente no campo **languageTag** .|
|languageTag   |String       | Fornece o código de cultura de idioma e o nome amigável do idioma no qual o campo **DisplayName** foi fornecido.                  |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.displayNameLocalization",
  "baseType": null
}-->

```json
{
  "displayName": "string",
  "languageTag": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "displayNameLocalization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
