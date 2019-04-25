---
title: tipo de recurso typedEmailAddress
description: Representa o nome, os endereços de email e o tipo de endereço de email correspondente de um contato.
localization_priority: Normal
ms.openlocfilehash: 3b1230dabc1e49c6cb9220eea95f0c3b93053d96
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576455"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/typedemailaddress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
