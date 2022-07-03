---
title: tipo de recurso assignedLabel
description: Representa um rótulo de confidencialidade atribuído a um grupo do Microsoft 365.
ms.localizationpriority: medium
author: psaffaie
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 1088ad83b8f2a46d687c234a9b7c87d7e2943ef5
ms.sourcegitcommit: 6a4e81d2b8e7447771c9060998c7e1cc18a57902
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/03/2022
ms.locfileid: "66609735"
---
# <a name="assignedlabel-resource-type"></a>tipo de recurso assignedLabel

Namespace: microsoft.graph

Representa um rótulo de confidencialidade atribuído a um grupo do Microsoft 365. Os rótulos de confidencialidade permitem que os administradores imponham configurações de grupo específicas em um grupo atribuindo uma classificação ao grupo (como Confidencial, Altamente Confidencial ou Geral). Os rótulos de confidencialidade são publicados pelos administradores no Centro de Conformidade & Segurança do Microsoft 365 como parte dos Proteção de Informações do Microsoft Purview recursos. Para obter mais informações sobre rótulos de confidencialidade, consulte [Visão geral dos rótulos de confidencialidade](/microsoft-365/compliance/sensitivity-labels).

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo   | Descrição                               |
| :---------- | :----- | :---------------------------------------- |
| labelId     | Cadeia de caracteres | O identificador exclusivo do rótulo.       |
| displayName | Cadeia de caracteres | O nome de exibição do rótulo. Somente leitura. |

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
