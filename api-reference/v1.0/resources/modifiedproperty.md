---
title: Tipo de recurso modifiedProperty
description: Indica todas as propriedades em um recurso do Azure AD que foram modificadas, incluindo os valores antigos e novos.
ms.localizationpriority: medium
author: dhanyahk
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 4c74e492b50435b7911952ffe32107008db11330
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067070"
---
# <a name="modifiedproperty-resource-type"></a>Tipo de recurso modifiedProperty

Namespace: microsoft.graph

Indica todas as propriedades em um recurso do Azure AD que foram modificadas, incluindo os valores antigos e novos.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|Cadeia de caracteres|Indica o nome da propriedade do atributo de destino que foi alterado.|
|newValue|Cadeia de caracteres|Indica o valor atualizado para a adequada.|
|oldValue|Cadeia de caracteres|Indica o valor anterior (antes da atualização) da propriedade.|

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

