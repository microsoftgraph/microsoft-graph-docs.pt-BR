---
title: tipo de recurso referenciouobject
description: Descreve uma referência a outro objeto definido na mesma definição de diretório.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c1c7e1554764031efbfa3a5d1c1280f4b72bc160
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007855"
---
# <a name="referencedobject-resource-type"></a>tipo de recurso referenciouobject

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve uma referência a outro objeto definido na mesma [definição de diretório](synchronization-directorydefinition.md).

## <a name="properties"></a>Propriedades

| Propriedade                   | Tipo                      | Descrição    |
|:---------------------------|:--------------------------|:---------------|
|referencedObjectName        |String                     |Nome do objeto referenciado. Deve corresponder a um dos objetos na [definição de diretório](synchronization-directorydefinition.md).|
|referenciouproperty          |String                     |**Não suportado no momento**. Nome da propriedade no objeto referenciado, o valor para o qual é usado como a referência.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referencedObject"
}-->

```json
{
  "referencedObjectName": "String",
  "referencedProperty": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "referencedObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
            
