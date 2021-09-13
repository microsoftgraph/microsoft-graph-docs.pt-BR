---
title: Tipo de recurso extension
description: Um tipo abstrato para oferecer suporte ao tipo openTypeExtension livre do OData v4.
ms.localizationpriority: medium
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 711684fe3717e742c04d13b3f85d3f4b8581fb51
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123513"
---
# <a name="extension-resource-type"></a>Tipo de recurso extension

Namespace: microsoft.graph

Um tipo abstrato para oferecer suporte ao tipo [openTypeExtension](opentypeextension.md) livre do OData v4.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "abstract": "true",
  "baseType": "microsoft.graph.entity",
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extension"
}-->

```json
{
  "id": "string (identifier)"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura.|

## <a name="relationships"></a>Relações
Nenhuma


## <a name="methods"></a>Métodos

Consulte os métodos do tipo derivado [openTypeExtension](opentypeextension.md) para métodos que são realmente compatíveis.


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

