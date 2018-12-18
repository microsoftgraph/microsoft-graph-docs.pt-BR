---
title: tipo de recurso de educationOrganization
description: Entidade abstrata usada para modelar o comum entre os tipos de organização diferentes dentro do setor de educação.
author: mmast-msft
ms.openlocfilehash: e4c0f69d63108cc88b88f530e99cbd55b23f49ed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326142"
---
# <a name="educationorganization-resource-type"></a>tipo de recurso de educationOrganization

Entidade abstrata usada para modelar o comum entre os tipos de organização diferentes dentro do setor de educação.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|description|String| Descrição da organização.|
|displayName|String| Nome de exibição da organização.|
|externalSource|educationExternalSource| Fonte local a partir do qual esta organização foi criada. Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->