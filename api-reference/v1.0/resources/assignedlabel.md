---
title: tipo de recurso assignedLabel
description: Representa um rótulo de confidencialidade atribuído a um grupo do Microsoft 365.
localization_priority: Normal
author: krbain
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 2e527dbf8cc1dd42474bee467f5e1f9a0beca261
ms.sourcegitcommit: 566d09c17f9d641b6fac9b9159405a3cc41e037b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/20/2020
ms.locfileid: "45184006"
---
# <a name="assignedlabel-resource-type"></a>tipo de recurso assignedLabel

Namespace: microsoft.graph

Representa um rótulo de confidencialidade atribuído a um grupo do Microsoft 365. Os rótulos de confidencialidade permitem que os administradores imponham configurações de grupo específicas em um grupo atribuindo uma classificação ao grupo (como confidencial, altamente confidencial ou geral). Os rótulos de confidencialidade são publicados por administradores no centro de conformidade & segurança da Microsoft 365 como parte dos recursos de proteção de informações da Microsoft. Para obter mais informações sobre rótulos de sensibilidade, consulte [visão geral dos rótulos de sensibilidade](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|labelID|String|O identificador exclusivo do rótulo.|
|displayName|String|O nome de exibição do rótulo. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.assignedLabel"
}-->

```json
{
  "labelId": "String",
  "displayName": "String"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "assignedLabel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->