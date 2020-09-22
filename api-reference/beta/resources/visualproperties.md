---
title: tipo de recurso visualproperties
description: 'Representa o conteúdo visual, como título e corpo, de uma notificação Visual direcionada para um usuário.  '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: 62580847844a4b397ed117ea4b256cc4f035577a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057686"
---
# <a name="visualproperties-resource-type"></a>tipo de recurso visualproperties

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o conteúdo visual, como título e corpo, de uma notificação Visual direcionada para um usuário. 

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|title|String|O título de uma notificação de usuário visual. Este campo é obrigatório para cargas de notificação visuais. |
|body|Cadeia de caracteres|O corpo de uma notificação de usuário visual. O corpo é opcional.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.visualProperties",
  "baseType": null
}-->

```json
{
  "title": "String",
  "body": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "visualProperties resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

