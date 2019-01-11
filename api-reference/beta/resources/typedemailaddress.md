---
title: tipo de recurso de typedEmailAddress
description: Representa o nome, endereços de email e seu correspondente tipo de endereço de email de um contato.
localization_priority: Normal
ms.openlocfilehash: c77d3dddc3e2bfcac47e6ed245dad9223fe7f08c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871264"
---
# <a name="typedemailaddress-resource-type"></a>tipo de recurso de typedEmailAddress

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa o nome, endereços de email e seu correspondente tipo de endereço de email de um [contato](contact.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|address|Cadeia de caracteres|O endereço de email de um contato.|
|name|Cadeia de caracteres|O nome de exibição de um contato.|
|type |Cadeia de caracteres |O tipo de endereço de email. Os valores possíveis são: `unknown`, `work`, `personal`, `main`, `other`. O valor padrão é `unknown`, que significa que o **endereço** não tiver sido definida como um tipo específico. |
|otherLabel |Cadeia de caracteres  |Para especificar um tipo personalizado de endereço de email, defina o **tipo** como `other`e atribuir **otherLabel** a uma cadeia de caracteres personalizada. Por exemplo, você pode usar um endereço de email específica para suas atividades voluntárias. Definir **tipo** `other`e configurado **otherLabel** como uma cadeia de caracteres personalizada como `Volunteer work`. |

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
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
