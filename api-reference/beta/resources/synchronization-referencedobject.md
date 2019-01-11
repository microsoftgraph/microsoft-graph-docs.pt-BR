---
title: tipo de recurso de referencedObject
description: Descreve uma referência a outro objeto definido na mesma definição de diretório.
localization_priority: Normal
ms.openlocfilehash: 5a2aa2dcc358c856c18ea2ce9871ec634194ce54
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821032"
---
# <a name="referencedobject-resource-type"></a>tipo de recurso de referencedObject

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Descreve uma referência a outro objeto definido na mesma [definição de diretório](synchronization-directorydefinition.md).

## <a name="properties"></a>Propriedades

| Propriedade                   | Tipo                      | Descrição    |
|:---------------------------|:--------------------------|:---------------|
|referencedObjectName        |Cadeia de caracteres                     |Nome do objeto referenciado. Deve corresponder a um dos objetos na [definição de diretório](synchronization-directorydefinition.md).|
|referencedProperty          |Cadeia de caracteres                     |**No momento não tem suporte**. Nome da propriedade no objeto referenciado, o valor para o qual é usado como referência.|

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
<!-- {
  "type": "#page.annotation",
  "description": "referencedObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
            
