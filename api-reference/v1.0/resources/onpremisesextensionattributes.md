---
title: Tipo de recurso onPremisesExtensionAttributes
description: A propriedade **onpremisesextensionattributes à** da entidade de usuário contém quinze Propriedades de atributos de extensões personalizadas. Para um usuário do **onPremisesSyncEnabled** , esse conjunto de propriedades é Mastered no Active Directory local e sincronizado com o Azure AD e é somente leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas durante a criação ou atualização.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 218bf0db4b615072ed3292311a26033279b1d803
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056433"
---
# <a name="onpremisesextensionattributes-resource-type"></a>Tipo de recurso onPremisesExtensionAttributes

Namespace: microsoft.graph

A propriedade **onpremisesextensionattributes à** da entidade de [usuário](user.md) contém quinze Propriedades de atributos de extensões personalizadas. Para um usuário do **onPremisesSyncEnabled** , a fonte de autoridade desse conjunto de propriedades é o Active Directory local que é sincronizado com o Azure AD e é somente leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas durante a criação ou atualização.

> **Observação:** Esses atributos de extensão também são conhecidos como atributos personalizados do Exchange 1-15.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|extensionAttribute1|String| Primeiro atributo de extensão personalizável. |
|extensionAttribute2|String| Segundo atributo de extensão personalizável. |
|extensionAttribute3|String| Terceiro atributo de extensão personalizável. |
|extensionAttribute4|String| Quarto atributo de extensão personalizável. |
|extensionAttribute5|String| Quinto atributo de extensão personalizável. |
|extensionAttribute6|String| Sexto atributo de extensão personalizável. |
|extensionAttribute7|String| Sétimo atributo de extensão personalizável. |
|extensionAttribute8|String| Oitavo atributo de extensão personalizável. |
|extensionAttribute9|String| Nono atributo de extensão personalizável. |
|extensionAttribute10|String| Décimo atributo de extensão personalizável. |
|extensionAttribute11|String| Décimo primeiro atributo de extensão personalizável. |
|extensionAttribute12|String| Décimo segundo atributo de extensão personalizável. |
|extensionAttribute13|String| Décimo terceiro atributo de extensão personalizável. |
|extensionAttribute14|String| Atributo de extensão personalizável décimo quarto. |
|extensionAttribute15|String| Atributo de extensão personalizável décimo quinto. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

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
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

