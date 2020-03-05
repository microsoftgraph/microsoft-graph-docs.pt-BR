---
title: tipo de recurso referenciouobject
description: Descreve uma referência a outro objeto definido na mesma definição de diretório.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6c27830b1ee9762b52a7f24a0785e1b19010181d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520118"
---
# <a name="referencedobject-resource-type"></a>tipo de recurso referenciouobject

Namespace: Microsoft. Graph

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
            
