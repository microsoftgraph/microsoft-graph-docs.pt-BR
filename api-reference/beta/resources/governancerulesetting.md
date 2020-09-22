---
title: tipo de recurso governanceRuleSetting
description: Representa as regras nas quais as configurações de função são compostas.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: b2a4b70eb7d8af5dde6e3741c3473683ca7e0586
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081633"
---
# <a name="governancerulesetting-resource-type"></a>tipo de recurso governanceRuleSetting

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as regras nas quais as configurações de função são compostas.


## <a name="properties"></a>Propriedades
|Propriedade      | Tipo         |Descrição|
|:-------------|:-------------|:----------|
|ruleIdentifier|Cadeia de caracteres        |A ID da regra. Por exemplo, ``ExpirationRule`` e ``MfaRule`` .|
|configuração       |Cadeia de caracteres        |As configurações da regra. O valor é uma cadeia de caracteres JSON com uma lista de pares no formato de Parameter_Name: Parameter_Value. Por exemplo, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceRuleSetting"
}-->


```json
{
  "ruleIdentifier": "String",
  "setting": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRuleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


