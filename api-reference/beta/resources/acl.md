---
title: tipo de recurso ACL
description: Uma entrada de controle de acesso para um item indexado por um externalConnection de pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5a26004cf20a5f8c5c032eeade8f657fdf8bd93c
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703937"
---
# <a name="acl-resource-type"></a>tipo de recurso ACL

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma entrada de controle de acesso para um item indexado por um [externalConnection](externalconnection.md)de pesquisa da Microsoft.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo   | Descrição                                        |
|:---------------|:-------|:---------------------------------------------------|
| accessType     | String | O acesso concedido à identidade. Os valores possíveis são: `grant` e `deny`. |
| identificação da identidade | String | Deve ser definida como `Azure Active Directory`.           |
| type           | String | O tipo de identidade. Os valores possíveis são: `user`, `group`, `everyone`, `everyoneExceptGuests`. |
| value          | Cadeia de caracteres | O identificador do Azure Active Directory. Se `type` for `user` ou `group`, `value` será definido como o identificador de objeto para o usuário ou grupo. Se `type` for `everyone` ou `everyoneExceptGuests`, `value` será definido como o identificador de locatário para o locatário do Azure Active Directory. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.acl",
  "baseType": null
}-->

```json
{
  "accessType": "String",
  "identitySource": "String",
  "type": "String",
  "value": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "acl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
