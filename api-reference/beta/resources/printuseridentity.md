---
title: tipo de recurso printUserIdentity
description: Representa uma identidade do usuário no serviço de impressão universal. Mapeia para um usuário do Azure AD.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: de2899b3ca75660280b797dda62993789f634096
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917601"
---
# <a name="printuseridentity-resource-type"></a>tipo de recurso printUserIdentity

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma identidade do usuário no serviço de impressão universal. Mapeia para um [usuário do Azure Active Directory (Azure AD)](user.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String|O identificador do printUserIdentity. Somente leitura.|
|displayName|Cadeia de caracteres|O nome de exibição do printUserIdentity.|
|ipAddress|Cadeia de caracteres|O endereço IP do printUserIdentity. Não preenchido.|
|userPrincipalName|String|O nome principal do usuário (UPN) do printUserIdentity.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUserIdentity",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "ipAddress": "String",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printUserIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
