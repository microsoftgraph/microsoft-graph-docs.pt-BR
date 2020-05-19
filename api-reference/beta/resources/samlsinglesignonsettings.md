---
title: tipo de recurso samlSingleSignOnSettings
description: Representa as configurações de logon único do SAML.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 38fd3a9827f710d032502c71161446201447192f
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290360"
---
# <a name="samlsinglesignonsettings-resource-type"></a>tipo de recurso samlSingleSignOnSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um contêiner para configurações relacionadas ao logon único do SAML.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|relaystate|String| O URI relativo para o qual o provedor de serviços redirecionaria após a conclusão do fluxo de logon único. |


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.samlSingleSignOnSettings"
}-->

```json
{
    "relayState": "string",
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "samlSingleSignOnSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
