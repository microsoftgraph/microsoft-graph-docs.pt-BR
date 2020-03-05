---
title: tipo de recurso visualproperties
description: 'Representa o conteúdo visual, como título e corpo, de uma notificação Visual direcionada para um usuário.  '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: 1678f560fa003c1884a9fa673ee85b7473e36c88
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519460"
---
# <a name="visualproperties-resource-type"></a>tipo de recurso visualproperties

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o conteúdo visual, como título e corpo, de uma notificação Visual direcionada para um usuário. 

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|title|String|O título de uma notificação de usuário visual. Este campo é obrigatório para cargas de notificação visuais. |
|corpo|String|O corpo de uma notificação de usuário visual. O corpo é opcional.|


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