---
title: tipo de recurso de governanceRuleSetting
description: Representa as regras que as configurações de função são compostas de.
ms.openlocfilehash: 486b5163c59772c971cfc1d61a98817b7f0c16f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037342"
---
# <a name="governancerulesetting-resource-type"></a>tipo de recurso de governanceRuleSetting

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa as regras que as configurações de função são compostas de.


## <a name="properties"></a>Propriedades
|Propriedade      | Tipo         |Descrição|
|:-------------|:-------------|:----------|
|ruleIdentifier|String        |A id da regra. Por exemplo, ``ExpirationRule`` e ``MfaRule``.|
|configuração       |Cadeia de caracteres        |As configurações da regra. O valor é uma cadeia de caracteres JSON com uma lista de pares no formato de Parameter_Name:Parameter_Value. Por exemplo, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`|

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
<!-- {
  "type": "#page.annotation",
  "description": "governanceRuleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->