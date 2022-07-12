---
title: Tipo de recurso typedEmailAddress
description: Representa o nome, os endereços de email e o tipo de endereço de email correspondente de um contato.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: mail
author: kevinbellinger
ms.openlocfilehash: 849e566919b22ddaa9c12a275f19139701bf467d
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66723486"
---
# <a name="typedemailaddress-resource-type"></a>Tipo de recurso typedEmailAddress

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o nome, os endereços de email e o tipo de endereço de email correspondente de um [contato](contact.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|address|Cadeia de caracteres|O endereço de email de um contato.|
|nome|String|O nome de exibição de um contato.|
|type |String |O tipo de endereço de email. Os valores possíveis são: `unknown`, `work`, `personal`, `main`, `other`. O valor padrão é `unknown`, o que significa **que o** endereço não foi definido como um tipo específico. |
|otherLabel |String  |Para especificar um tipo personalizado de endereço de email, defina **o tipo** e `other`atribua **otherLabel** a uma cadeia de caracteres personalizada. Por exemplo, você pode usar um endereço de email específico para suas atividades voluntárias. **Defina o** tipo `other`como , e defina **otherLabel** como uma cadeia de caracteres personalizada, como `Volunteer work`. |

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


