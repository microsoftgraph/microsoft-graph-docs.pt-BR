---
title: tipo de recurso de educationOrganization
description: Entidade abstrata usada para modelar o comum entre os tipos de organização diferentes dentro do setor de educação.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 99f3294f76a246e4e78f0f61b0fc1f62532c3a03
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977420"
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
