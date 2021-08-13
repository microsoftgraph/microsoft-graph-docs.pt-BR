---
title: Tipo de recurso modifiedProperty
description: Indica todas as propriedades em um recurso do Azure AD que foram modificadas, incluindo os valores antigos e novos.
localization_priority: Normal
author: dhanyahk
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9b1c520ac4be4e0c0957fe2b9f4f833f4065a19a2ed76ecd3166a46f7e50de6c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54192205"
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

