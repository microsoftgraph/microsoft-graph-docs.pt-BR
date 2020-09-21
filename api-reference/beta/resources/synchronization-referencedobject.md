---
title: tipo de recurso referenciouobject
description: Descreve uma referência a outro objeto definido na mesma definição de diretório.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9ea400e40074b30943412cf7b5fbae75f9037ca1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023881"
---
# <a name="referencedobject-resource-type"></a>tipo de recurso referenciouobject

Namespace: microsoft.graph

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
            


