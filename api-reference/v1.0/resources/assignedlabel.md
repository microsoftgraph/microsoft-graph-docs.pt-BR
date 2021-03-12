---
title: Tipo de recurso assignedLabel
description: Representa um rótulo de sensibilidade atribuído a um grupo do Microsoft 365.
localization_priority: Normal
author: jpettere
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 9602e10dda5d558110c55f1fb4ee166e53187989
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720890"
---
# <a name="assignedlabel-resource-type"></a>Tipo de recurso assignedLabel

Namespace: microsoft.graph

Representa um rótulo de sensibilidade atribuído a um grupo do Microsoft 365. Os rótulos de confidencialidade permitem que os administradores imigam configurações de grupo específicas em um grupo atribuindo uma classificação ao grupo (como Confidencial, Altamente Confidencial ou Geral). Os rótulos de sensibilidade são publicados pelos administradores no Centro de Conformidade e Segurança do Microsoft 365 & como parte dos recursos de Proteção de Informações da Microsoft. Para obter mais informações sobre rótulos de sensibilidade, consulte [Visão geral dos rótulos de sensibilidade.](/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide)

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|labelId|Cadeia de caracteres|O identificador exclusivo do rótulo.|
|displayName|Cadeia de caracteres|O nome de exibição do rótulo. Somente leitura.|

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