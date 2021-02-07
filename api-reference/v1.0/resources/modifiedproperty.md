---
title: Tipo de recurso modifiedProperty
description: Indica todas as propriedades em um recurso do Azure AD que foram modificadas, incluindo os valores antigo e novo.
localization_priority: Normal
author: dhanyahk
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 4e34501f5011310eb7ade73d1c5d938cb58e65cc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136035"
---
# <a name="modifiedproperty-resource-type"></a>Tipo de recurso modifiedProperty

Namespace: microsoft.graph

Indica todas as propriedades em um recurso do Azure AD que foram modificadas, incluindo os valores antigo e novo.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|String|Indica o nome da propriedade do atributo de destino que foi alterado.|
|newValue|Cadeia de caracteres|Indica o valor atualizado para a adequada.|
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

