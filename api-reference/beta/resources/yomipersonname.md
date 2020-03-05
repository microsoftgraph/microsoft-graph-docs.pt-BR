---
title: tipo de recurso yomiPersonName
description: tipo de recurso yomiPersonName
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0a598c4b5e999b03aeb7201c6eae3a230d3160a7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518970"
---
# <a name="yomipersonname-resource-type"></a>tipo de recurso yomiPersonName

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece um mecanismo para que um usuário armazene informações sobre como pronunciar um nome para alto-falantes não nativos do idioma no qual o recurso [PersonName](personname.md) é representado.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição                                             |
|:-------------|:------------|:--------------------------------------------------------|
|displayName   |String       | Composto de guias de pronúncia de nome e de sobrenome.  |
|primeiro         |String       | Guia de pronúncia para o primeiro nome do usuário.     |
|durar          |String       | Guia de pronúncia para o sobrenome do usuário.      |
|Virgem        |String       | Guia de pronúncia para o nome de solteira do usuário.    |
|middleware        |String       | Guia de pronúncia para o nome do meio do usuário.    |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.yomiPersonName",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "first": "String",
  "last": "String",
  "maiden": "String",
  "middle": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "yomiPersonName resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
