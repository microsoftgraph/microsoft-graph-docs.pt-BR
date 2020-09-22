---
title: tipo de recurso printUserIdentity
description: Representa uma identidade do usuário no serviço de impressão universal. Mapeia para um usuário do Azure AD.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 8a695bed829d6c7e8825898da366737427195e1d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070650"
---
# <a name="printuseridentity-resource-type"></a>tipo de recurso printUserIdentity

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma identidade do usuário no serviço de impressão universal. Mapeia para um [usuário do Azure Active Directory (Azure AD)](user.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres|O identificador do printUserIdentity. Somente leitura.|
|displayName|Cadeia de caracteres|O nome de exibição do printUserIdentity.|
|ipAddress|Cadeia de caracteres|O endereço IP do printUserIdentity. Não preenchido.|
|userPrincipalName|Cadeia de caracteres|O nome principal do usuário (UPN) do printUserIdentity.|

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


