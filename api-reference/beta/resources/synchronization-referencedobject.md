---
title: Tipo de recurso referencedObject
description: Descreve uma referência a outro objeto definido na mesma definição de diretório.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: c6e273474c70919bab3c30335a26477509eca8cc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132515"
---
# <a name="referencedobject-resource-type"></a>Tipo de recurso referencedObject

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve uma referência a outro objeto definido na mesma definição [de diretório.](synchronization-directorydefinition.md)

## <a name="properties"></a>Propriedades

| Propriedade                   | Tipo                      | Descrição    |
|:---------------------------|:--------------------------|:---------------|
|referencedObjectName        |String                     |Nome do objeto referenciado. Deve corresponder a um dos objetos na definição [de diretório.](synchronization-directorydefinition.md)|
|referencedProperty          |String                     |**Não há suporte no momento.** Nome da propriedade no objeto referenciado, o valor para o qual é usado como referência.|

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
            


