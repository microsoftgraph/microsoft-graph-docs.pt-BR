---
title: Tipo de recurso extension
description: Um tipo abstrato para oferecer suporte ao tipo openTypeExtension livre do OData v4.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 547570b70948590e72060432618005f02b8a167ba772cb39cd5290ea4134cdf8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141711"
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

