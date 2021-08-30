---
title: Tipo de recurso displayNameLocalization
description: Fornece a capacidade de um administrador personalizar a cadeia de caracteres usada em uma experiência Microsoft 365 compartilhada.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a45c64d8cb80d94a702cfd4be57012949a7c86e3
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696464"
---
# <a name="displaynamelocalization-resource-type"></a>Tipo de recurso displayNameLocalization

Fornece a capacidade de um administrador personalizar a cadeia de caracteres usada em uma experiência Microsoft 365 compartilhada.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|displayName   |Cadeia de caracteres       | Se presente, o valor deste campo contém a cadeia de **caracteres displayName** que foi definida para o idioma presente no **campo languageTag.**|
|languageTag   |Cadeia de caracteres       | Fornece o código de cultura de idioma e o nome amigável do idioma em que o **campo displayName** foi fornecido.                  |

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


