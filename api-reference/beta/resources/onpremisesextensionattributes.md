---
title: Tipo de recurso onPremisesExtensionAttributes
description: A propriedade **onpremisesextensionattributes à** da entidade de usuário contém quinze Propriedades de atributos de extensões personalizadas.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: krbain
ms.openlocfilehash: 2729d6d624f1bde304425229ccf4ae7df8ddf781
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052584"
---
# <a name="onpremisesextensionattributes-resource-type"></a>Tipo de recurso onPremisesExtensionAttributes

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A propriedade **onpremisesextensionattributes à** da entidade de [usuário](user.md) contém quinze Propriedades de atributos de extensões personalizadas. Para um usuário do **onPremisesSyncEnabled** , a fonte de autoridade desse conjunto de propriedades é o Active Directory local que é sincronizado com o Azure AD e é somente leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas durante a criação ou atualização.

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
|extensionAttribute14|Cadeia de caracteres| Atributo de extensão personalizável décimo quarto. |
|extensionAttribute15|Cadeia de caracteres| Atributo de extensão personalizável décimo quinto. |

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


