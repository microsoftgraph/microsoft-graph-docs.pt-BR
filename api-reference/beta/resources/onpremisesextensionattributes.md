---
title: tipo de recurso Onpremisesextensionattributes à
description: A propriedade **onpremisesextensionattributes à** da entidade de usuário contém quinze Propriedades de atributos de extensões personalizadas.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: krbain
ms.openlocfilehash: 1035674a6ce5d9f2c0a1a8b2cd35896c92ec7147
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863751"
---
# <a name="onpremisesextensionattributes-resource-type"></a>tipo de recurso Onpremisesextensionattributes à

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
