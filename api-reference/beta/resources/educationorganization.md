---
title: tipo de recurso educationOrganization
description: 'Entidade abstrata usada para modelar a semelhança entre diferentes tipos de organização dentro do setor educacional.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8652e6841c39442d8b9875ea48c785a0275073ef
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501483"
---
# <a name="educationorganization-resource-type"></a>tipo de recurso educationOrganization

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Entidade abstrata usada para modelar a semelhança entre diferentes tipos de organização dentro do setor educacional.  

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|description|String| Descrição da organização.|
|displayName|Cadeia de caracteres| Nome de exibição da organização.|
|externalSource|cadeia de caracteres| Origem de onde esta organização foi criada. Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
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
<!--
{
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
