---
title: tipo de recurso modifiedproperty
description: Indica todas as propriedades em um recurso do Azure AD que foram modificadas, incluindo os valores antigo e novo.
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
doc_type: resourcePageType
ms.openlocfilehash: d98d0aaa4850e8ef2b82f9f5deb17424c3ab98d3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967377"
---
# <a name="modifiedproperty-resource-type"></a>tipo de recurso modifiedproperty

Namespace: microsoft.graph

Indica todas as propriedades em um recurso do Azure AD que foram modificadas, incluindo os valores antigo e novo.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|String|Indica o nome da Propriedade do atributo de destino que foi alterado.|
|newValue|Cadeia de caracteres|Indica o valor atualizado para o correto.|
|oldValue|Cadeia de caracteres|Indica o valor anterior (antes da atualização) para a propriedade.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.modifiedProperty"
}-->

```json
{
  "displayName": "String",
  "newValue": "String",
  "oldValue": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "modifiedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

