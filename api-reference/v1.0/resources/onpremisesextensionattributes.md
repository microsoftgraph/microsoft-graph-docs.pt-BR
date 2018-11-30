---
title: tipo de recurso de onPremisesExtensionAttributes
description: A propriedade **onPremisesExtensionAttributes** da entidade do usuário contém quinze propriedades de atributo de extensão personalizada. Um usuário **onPremisesSyncEnabled** , esse conjunto de propriedades é administrado no Active Directory no local e sincronizado com o Azure AD e é somente leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definida durante a criação ou atualização.
ms.openlocfilehash: e5a56b5a846cf48cfc819b6d884689be10d6992e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005670"
---
# <a name="onpremisesextensionattributes-resource-type"></a>tipo de recurso de onPremisesExtensionAttributes

A propriedade **onPremisesExtensionAttributes** da entidade do [usuário](user.md) contém quinze propriedades de atributo de extensão personalizada. Um usuário **onPremisesSyncEnabled** , esse conjunto de propriedades é administrado no Active Directory no local e sincronizado com o Azure AD e é somente leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definida durante a criação ou atualização.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|extensionAttribute1|String| Primeiro atributo de extensão personalizável. |
|extensionAttribute2|String| Segundo atributo de extensão personalizável. |
|extensionAttribute3|String| Atributo do terceiro extensão personalizável. |
|extensionAttribute4|String| Quarto atributo de extensão personalizável. |
|extensionAttribute5|String| Atributo do quinto extensão personalizável. |
|extensionAttribute6|String| Sexto atributo de extensão personalizável. |
|extensionAttribute7|String| Sétimo atributo de extensão personalizável. |
|extensionAttribute8|String| Oitavo atributo de extensão personalizável. |
|extensionAttribute9|String| Nono atributo de extensão personalizável. |
|extensionAttribute10|String| Décimo atributo de extensão personalizável. |
|extensionAttribute11|String| Atributo de extensão Décima primeira personalizável. |
|extensionAttribute12|String| Atributo de extensão Décima segunda personalizável. |
|extensionAttribute13|String| Atributo de extensão Décima terceira personalizável. |
|extensionAttribute14|String| Atributo de extensão décima quarta personalizável. |
|extensionAttribute15|String| Atributo de extensão Décima quinta personalizável. |

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