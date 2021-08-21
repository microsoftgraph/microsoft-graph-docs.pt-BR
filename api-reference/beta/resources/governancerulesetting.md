---
title: Tipo de recurso governanceRuleSetting
description: Representa as regras de que as configurações de função são compostas.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu1
ms.openlocfilehash: 956d3b3c17182285d1ba74552a3b0bfdd5c717fa
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2021
ms.locfileid: "58454042"
---
# <a name="governancerulesetting-resource-type"></a>Tipo de recurso governanceRuleSetting

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as regras de que as configurações de função são compostas.


## <a name="properties"></a>Propriedades
|Propriedade      | Tipo         |Descrição|
|:-------------|:-------------|:----------|
|ruleIdentifier|Cadeia de caracteres        |A id da regra. Por exemplo, ``ExpirationRule`` e ``MfaRule`` .|
|configuração       |Cadeia de caracteres        |As configurações da regra. O valor é uma cadeia de caracteres JSON com uma lista de pares no formato Parameter_Name:Parameter_Value. Por exemplo, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`|

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


