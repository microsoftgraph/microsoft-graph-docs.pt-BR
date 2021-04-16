---
title: Tipo de recurso onPremisesExtensionAttributes
description: A **propriedade onPremisesExtensionAttributes** da entidade do usuário contém quinze propriedades de atributo de extensão personalizadas. Para um usuário **onPremisesSyncEnabled,** esse conjunto de propriedades é mestre no Active Directory local e sincronizado com o Azure AD, e é somente leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas sobre o Exchange Online. Os atributos são lidos somente no Microsoft Graph.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: f21369156e1a1337d16d64be40bd6de210bd56d2
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766102"
---
# <a name="onpremisesextensionattributes-resource-type"></a>Tipo de recurso onPremisesExtensionAttributes

Namespace: microsoft.graph

A **propriedade onPremisesExtensionAttributes** da entidade do usuário contém quinze propriedades de atributo de extensão personalizadas. [](user.md) Para um usuário **onPremisesSyncEnabled,** a fonte de autoridade para esse conjunto de propriedades é o Active Directory local que é sincronizado com o Azure AD e é somente leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas sobre o Exchange Online. Os atributos são lidos somente no Microsoft Graph.

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
|extensionAttribute14|String| Décimo quarto atributo de extensão personalizável. |
|extensionAttribute15|String| Décimo quinto atributo de extensão personalizável. |

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

