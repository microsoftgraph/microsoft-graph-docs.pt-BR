---
title: tipo de recurso ACL
description: Uma entrada de controle de acesso para um item indexado por um externalConnection de pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 6d390ac0fee3063bd8f0d292d14e04b2616c1d00
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193530"
---
# <a name="acl-resource-type"></a>tipo de recurso ACL

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma entrada de controle de acesso para um item indexado por um [externalConnection](externalconnection.md)de pesquisa da Microsoft.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo   | Descrição                                        |
|:---------------|:-------|:---------------------------------------------------|
| accessType     | String | O acesso concedido à identidade. Os valores possíveis são: `grant` e `deny`. |
| identificação da identidade | String | A fonte de identidade. Os valores possíveis são `azureActiveDirectory` ou `external` .           |
| tipo           | String | O tipo de identidade. Os valores possíveis são: `user` , `group` , `everyone` , `everyoneExceptGuests` se a identificação do próprio é `azureActiveDirectory` e apenas `group` se a identificação do próprio é `external` . |
| value          | Cadeia de caracteres | O identificador exclusivo da identidade. No caso de identidades do Active Directory do Azure, `value` é definido como o identificador de objeto do usuário, grupo ou locatário para tipos usuário, grupo e todos (e everyoneExceptGuests), respectivamente. No caso de grupos externos, `value` está definido como a ID do grupo [externo](externalgroup.md).|

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
