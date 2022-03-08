---
title: Tipo de recurso onPremisesExtensionAttributes
description: 'A **propriedade onPremisesExtensionAttributes** da entidade do usuário contém quinze propriedades de atributo de extensão personalizadas. '
ms.localizationpriority: medium
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: d43bcc3e838a9d7955954127dbc5960f45b60b15
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335931"
---
# <a name="onpremisesextensionattributes-resource-type"></a>Tipo de recurso onPremisesExtensionAttributes

Namespace: microsoft.graph

O tipo de retorno da **propriedade onPremisesExtensionAttributes** do objeto [de](user.md) usuário e da propriedade **extensionAttributes** do [objeto device](device.md) . Retorna quinze propriedades de atributo de extensão personalizadas.

Na entidade [](user.md) do usuário e para um usuário **onPremisesSyncEnabled**, a fonte de autoridade para esse conjunto de propriedades é o Active Directory local que é sincronizado com o Azure AD e é somente leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** `false` está ou `null`), essas propriedades podem ser definidas durante a [criação](../api/user-post-users.md) ou [atualização](../api/user-update.md). Se um usuário somente na nuvem tiver sido sincronizado anteriormente do Active Directory local, essas propriedades não poderão ser gerenciadas por meio da API do Microsoft Graph. Em vez disso, eles podem ser gerenciados por meio do Centro de administração Exchange ou o módulo Exchange Online V2 no PowerShell.

A **propriedade extensionAttributes** da entidade [de](device.md) dispositivo é gerenciada somente no Azure AD durante a [criação ou atualização](../api/device-post-devices.md) do [dispositivo](../api/device-update.md).

> **Observação:** Esses atributos de extensão também são conhecidos como Exchange atributos personalizados 1-15.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|extensionAttribute1|Cadeia de caracteres| Primeiro atributo de extensão personalizável. |
|extensionAttribute2|String| Segundo atributo de extensão personalizável. |
|extensionAttribute3|String| Terceiro atributo de extensão personalizável. |
|extensionAttribute4|Cadeia de caracteres| Quarto atributo de extensão personalizável. |
|extensionAttribute5|String| Quinto atributo de extensão personalizável. |
|extensionAttribute6|String| Sexto atributo de extensão personalizável. |
|extensionAttribute7|Cadeia de caracteres| Sétimo atributo de extensão personalizável. |
|extensionAttribute8|Cadeia de caracteres| Oitavo atributo de extensão personalizável. |
|extensionAttribute9|Cadeia de caracteres| Nono atributo de extensão personalizável. |
|extensionAttribute10|Cadeia de caracteres| Décimo atributo de extensão personalizável. |
|extensionAttribute11|String| Décimo primeiro atributo de extensão personalizável. |
|extensionAttribute12|Cadeia de caracteres| Décimo segundo atributo de extensão personalizável. |
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