---
title: Tipo de recurso assignedLabel
description: Representa um rótulo de sensibilidade atribuído a um grupo do Microsoft 365. Os rótulos de confidencialidade permitem que os administradores imigam configurações de grupo específicas em um grupo atribuindo uma classificação ao grupo (como Confidencial, Altamente Confidencial ou Geral).
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: f22bfdd6cce307a83a90ada1da6a312994a3538e
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761244"
---
# <a name="assignedlabel-resource-type"></a>Tipo de recurso assignedLabel

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um rótulo de sensibilidade atribuído a um grupo do Microsoft 365. Os rótulos de confidencialidade permitem que os administradores imigam configurações de grupo específicas em um grupo atribuindo uma classificação ao grupo (como Confidencial, Altamente Confidencial ou Geral). Os rótulos de sensibilidade são publicados pelos administradores no Centro de Conformidade e Segurança do Microsoft 365 & como parte dos recursos de Proteção de Informações da Microsoft. Para obter mais informações sobre rótulos de sensibilidade, consulte [Visão geral dos rótulos de sensibilidade.](/Office365/SecurityCompliance/sensitivity-labels)

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|labelId|Cadeia de Caracteres|O identificador exclusivo do rótulo.|
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


