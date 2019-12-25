---
title: tipo de recurso assignedLabel
description: Representa um rótulo de confidencialidade atribuído a um grupo do Office 365. Os rótulos de confidencialidade permitem que os administradores imponham configurações de grupo específicas em um grupo atribuindo uma classificação ao grupo (como confidencial, altamente confidencial ou geral).
localization_priority: Normal
author: krbain
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 7e8390ec1773061d447e7526f55e67b87e51531b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870936"
---
# <a name="assignedlabel-resource-type"></a>tipo de recurso assignedLabel

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um rótulo de confidencialidade atribuído a um grupo do Office 365. Os rótulos de confidencialidade permitem que os administradores imponham configurações de grupo específicas em um grupo atribuindo uma classificação ao grupo (como confidencial, altamente confidencial ou geral). Os rótulos de confidencialidade são publicados por administradores no centro de conformidade & segurança da Microsoft 365 como parte dos recursos de proteção de informações da Microsoft. Para obter mais informações sobre rótulos de sensibilidade, consulte [visão geral dos rótulos de sensibilidade](/Office365/SecurityCompliance/sensitivity-labels).

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
