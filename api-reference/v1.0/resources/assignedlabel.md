---
title: Tipo de recurso assignedLabel
description: Representa um rótulo de sensibilidade atribuído a um Microsoft 365 grupo.
ms.localizationpriority: medium
author: psaffaie
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: a4992960d63c90efb06d3799944c9df66616759c
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588320"
---
# <a name="assignedlabel-resource-type"></a>Tipo de recurso assignedLabel

Namespace: microsoft.graph

Representa um rótulo de sensibilidade atribuído a um Microsoft 365 grupo. Os rótulos de confidencialidade permitem que os administradores imigam configurações de grupo específicas em um grupo atribuindo uma classificação ao grupo (como Confidencial, Altamente Confidencial ou Geral). Os rótulos de sensibilidade são publicados pelos administradores Microsoft 365 Centro de Conformidade & Segurança como parte dos recursos Proteção de Informações da Microsoft segurança. Para obter mais informações sobre rótulos de sensibilidade, consulte [Visão geral dos rótulos de sensibilidade](/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide).

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
