---
title: tipo de recurso de credencial
description: Indica uma única credencial usada para entrar em um aplicativo.
localization_priority: Normal
author: bharathramh92
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0521f766a7a0da482cf67628c3816935ee9270b8
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761678"
---
# <a name="credential-resource-type"></a>tipo de recurso de credencial

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Indica uma única credencial usada para entrar em um aplicativo. Por exemplo, nome de usuário é uma credencial, senha é outra credencial.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|fieldId|Cadeia de Caracteres|O nome do campo para essa credencial. por exemplo, nome de usuário ou senha ou telefoneNumber. Isso é definido pelo aplicativo. Deve corresponder ao que está no campo html no objeto singleSignOnSettings/password.|
|tipo|Cadeia de caracteres|O tipo dessa credencial. Valores válidos: nome de usuário, senha ou outros.|
|value|Cadeia de caracteres|O valor dessa credencial. por exemplo, mysuperhiddenpassword. Observe que o valor das senhas é somente gravação, o valor nunca poderá ser lido de volta.|

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


