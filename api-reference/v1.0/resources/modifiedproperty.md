---
title: tipo de recurso modifiedproperty
description: Indica todas as propriedades em um recurso do Azure AD que foram modificadas, incluindo os valores antigo e novo.
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
doc_type: resourcePageType
ms.openlocfilehash: 0c5375ea3e188d6023e3588531e07877f6de38ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036096"
---
# <a name="modifiedproperty-resource-type"></a>tipo de recurso modifiedproperty

Indica todas as propriedades em um recurso do Azure AD que foram modificadas, incluindo os valores antigo e novo.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|String|Indica o nome da Propriedade do atributo de destino que foi alterado.|
|newValue|Cadeia de caracteres|Indica o valor atualizado para o correto.|
|oldValue|String|Indica o valor anterior (antes da atualização) para a propriedade.|

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
