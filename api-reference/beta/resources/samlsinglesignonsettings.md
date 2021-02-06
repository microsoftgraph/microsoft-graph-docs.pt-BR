---
title: Tipo de recurso samlSingleSignOnSettings
description: Representa as configurações de login único do SAML.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 0b82f334196bcd9f7799a3a7a3ef7b5374571ac4
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136125"
---
# <a name="samlsinglesignonsettings-resource-type"></a>Tipo de recurso samlSingleSignOnSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um contêiner para configurações relacionadas ao single sign-on do SAML.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|relayState|String| O URI relativo ao que o provedor de serviços redirecionaria após a conclusão do fluxo de logom único. |


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


