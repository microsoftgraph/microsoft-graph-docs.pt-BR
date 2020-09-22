---
title: tipo de recurso Credential
description: Indica uma única credencial usada para entrar em um aplicativo.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a281e39850ea18ee3bcbe0d83c5df3b41d0ccd31
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016685"
---
# <a name="credential-resource-type"></a>tipo de recurso Credential

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Indica uma única credencial usada para entrar em um aplicativo. Por exemplo, username é uma credencial, password é outra credencial.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|fieldId|String|O nome do campo para esta credencial. por exemplo, nome de usuário ou senha ou phoneNumber. Isso é definido pelo aplicativo. Deve corresponder ao que está no campo HTML no objeto singleSignOnSettings/password.|
|tipo|String|O tipo desta credencial. Valores válidos: username, password ou Other.|
|value|Cadeia de caracteres|O valor dessa credencial. por exemplo, mysuperhiddenpassword. Observação o valor de senhas é somente gravação, o valor nunca pode ser lido novamente.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credential",
  "baseType": null
}-->

```json
{
  "fieldId": "param_username",
  "value": "myusername",
  "type": "username"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


