---
title: tipo de recurso employeeOrgData
description: Representa os dados da organização associados a um usuário.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: cmmdesai
ms.openlocfilehash: 841d3c7965309721d662475f2cba553c378c49ee
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635604"
---
# <a name="employeeorgdata-resource-type"></a>tipo de recurso employeeOrgData

Namespace: microsoft.graph

Representa os dados da organização associados a um usuário. A propriedade **employeeOrgData** da entidade [User](user.md) é uma coleção de atributos de organização.

## <a name="properties"></a>Propriedades
| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
| Division | String | O nome da divisão na qual o usuário trabalha. <br><br>Retornado apenas em `$select`. Oferece suporte para `$filter`. |
| costCenter | String | O centro de custos associado ao usuário. <br><br>Retornado apenas em `$select`. Oferece suporte para `$filter`. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.employeeOrgData"
}-->

```json
{
  "costCenter": "string",
  "division": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2020-10-24 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "employeeOrgData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
