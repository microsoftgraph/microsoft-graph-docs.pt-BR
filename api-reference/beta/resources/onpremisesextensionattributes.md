---
title: Tipo de recurso onPremisesExtensionAttributes
description: A **propriedade onPremisesExtensionAttributes** da entidade do usuário contém quinze propriedades de atributo de extensão personalizadas.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: jpettere
ms.openlocfilehash: 95d777140210070471c9578399e26e0eda3620d7
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720582"
---
# <a name="onpremisesextensionattributes-resource-type"></a>Tipo de recurso onPremisesExtensionAttributes

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A **propriedade onPremisesExtensionAttributes** da entidade do usuário contém quinze propriedades de atributo de extensão personalizadas. [](user.md) Para um usuário **onPremisesSyncEnabled,** a fonte de autoridade para esse conjunto de propriedades é o Active Directory local que é sincronizado com o Azure AD e é somente leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas durante a criação ou atualização.

> **Observação:** Esses atributos de extensão também são conhecidos como atributos personalizados do Exchange 1-15.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|extensionAttribute1|Cadeia de caracteres| Primeiro atributo de extensão personalizável. |
|extensionAttribute2|Cadeia de caracteres| Segundo atributo de extensão personalizável. |
|extensionAttribute3|Cadeia de caracteres| Terceiro atributo de extensão personalizável. |
|extensionAttribute4|Cadeia de caracteres| Quarto atributo de extensão personalizável. |
|extensionAttribute5|Cadeia de caracteres| Quinto atributo de extensão personalizável. |
|extensionAttribute6|Cadeia de caracteres| Sexto atributo de extensão personalizável. |
|extensionAttribute7|Cadeia de caracteres| Sétimo atributo de extensão personalizável. |
|extensionAttribute8|Cadeia de caracteres| Oitavo atributo de extensão personalizável. |
|extensionAttribute9|Cadeia de caracteres| Nono atributo de extensão personalizável. |
|extensionAttribute10|Cadeia de caracteres| Décimo atributo de extensão personalizável. |
|extensionAttribute11|Cadeia de caracteres| Décimo primeiro atributo de extensão personalizável. |
|extensionAttribute12|Cadeia de caracteres| Décimo segundo atributo de extensão personalizável. |
|extensionAttribute13|Cadeia de caracteres| Décimo terceiro atributo de extensão personalizável. |
|extensionAttribute14|Cadeia de caracteres| Décimo quarto atributo de extensão personalizável. |
|extensionAttribute15|Cadeia de caracteres| Décimo quinto atributo de extensão personalizável. |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
}-->


```json
{
      "extensionAttribute1": "string",
      "extensionAttribute2": "string",
      "extensionAttribute3": "string",
      "extensionAttribute4": "string",
      "extensionAttribute5": "string",
      "extensionAttribute6": "string",
      "extensionAttribute7": "string",
      "extensionAttribute8": "string",
      "extensionAttribute9": "string",
      "extensionAttribute10": "string",
      "extensionAttribute11": "string",
      "extensionAttribute12": "string",
      "extensionAttribute13": "string",
      "extensionAttribute14": "string",
      "extensionAttribute15": "string"
  }

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


