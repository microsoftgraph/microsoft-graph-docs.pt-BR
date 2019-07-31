---
title: tipo de recurso typedEmailAddress
description: Representa o nome, os endereços de email e o tipo de endereço de email correspondente de um contato.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: c5ece5d1ad1c5c38253d73353b05b94727855fd5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007568"
---
# <a name="typedemailaddress-resource-type"></a>tipo de recurso typedEmailAddress

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o nome, os endereços de email e o tipo de endereço de email correspondente de um [contato](contact.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|address|Cadeia de caracteres|O endereço de email de um contato.|
|name|String|O nome de exibição de um contato.|
|type |String |O tipo de endereço de email. Os valores possíveis são: `unknown`, `work`, `personal`, `main`, `other`. O valor padrão é `unknown`, o que significa que o **endereço** não foi definido como um tipo específico. |
|otherLabel |String  |Para especificar um tipo personalizado de endereço de email, **** defina Type `other`como e atribua **otherLabel** a uma cadeia de caracteres personalizada. Por exemplo, você pode usar um endereço de email específico para suas atividades de voluntários. Defina **** o tipo `other`como e defina **otherLabel** como uma cadeia de caracteres personalizada `Volunteer work`, como. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.typedEmailAddress"
}-->

```json
{
  "address": "string",
  "name": "string",
  "type": "string",
  "otherLabel": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
