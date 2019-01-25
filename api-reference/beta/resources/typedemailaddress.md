---
title: tipo de recurso de typedEmailAddress
description: Representa o nome, endereços de email e seu correspondente tipo de endereço de email de um contato.
localization_priority: Normal
ms.openlocfilehash: 3b1230dabc1e49c6cb9220eea95f0c3b93053d96
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510705"
---
# <a name="typedemailaddress-resource-type"></a>tipo de recurso de typedEmailAddress

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o nome, endereços de email e seu correspondente tipo de endereço de email de um [contato](contact.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|address|Cadeia de caracteres|O endereço de email de um contato.|
|name|Cadeia de caracteres|O nome de exibição de um contato.|
|type |String |O tipo de endereço de email. Os valores possíveis são: `unknown`, `work`, `personal`, `main`, `other`. O valor padrão é `unknown`, que significa que o **endereço** não tiver sido definida como um tipo específico. |
|otherLabel |String  |Para especificar um tipo personalizado de endereço de email, defina o **tipo** como `other`e atribuir **otherLabel** a uma cadeia de caracteres personalizada. Por exemplo, você pode usar um endereço de email específica para suas atividades voluntárias. Definir **tipo** `other`e configurado **otherLabel** como uma cadeia de caracteres personalizada como `Volunteer work`. |

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
