---
title: Tipo de recurso samlSingleSignOnSettings
description: Representa as configurações de login único SAML.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: c0bbe655f1e9ac79b31b3eaa90ad57d72d08f642
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117701"
---
# <a name="samlsinglesignonsettings-resource-type"></a>Tipo de recurso samlSingleSignOnSettings

Representa um contêiner para configurações relacionadas ao login único SAML.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|relayState|Cadeia de caracteres| O URI relativo para o que o provedor de serviços redirecionaria após a conclusão do fluxo de logom único. |


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
