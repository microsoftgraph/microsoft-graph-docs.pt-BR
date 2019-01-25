---
title: tipo de recurso de onPremisesExtensionAttributes
description: A propriedade **onPremisesExtensionAttributes** da entidade do usuário contém quinze propriedades de atributo de extensão personalizada. Para um usuário onPremisesSyncEnabled, esse conjunto de propriedades é masterizado no Active Directory local e sincronizado com o Azure Active Directory e é somente leitura. Para um usuário somente na nuvem (onde onPremisesSyncEnabled é falso), essas propriedades podem ser definidas durante a criação ou atualização.
localization_priority: Normal
ms.openlocfilehash: f44f71fdcd86d2165289282568a2d7153ccc99b1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518237"
---
# <a name="onpremisesextensionattributes-resource-type"></a>tipo de recurso de onPremisesExtensionAttributes

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A propriedade **onPremisesExtensionAttributes** da entidade do [usuário](user.md) contém quinze propriedades de atributo de extensão personalizada. Para um usuário onPremisesSyncEnabled, esse conjunto de propriedades é masterizado no Active Directory local e sincronizado com o Azure Active Directory e é somente leitura. Para um usuário somente na nuvem (onde onPremisesSyncEnabled é falso), essas propriedades podem ser definidas durante a criação ou atualização.


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
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisesextensionattributes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
