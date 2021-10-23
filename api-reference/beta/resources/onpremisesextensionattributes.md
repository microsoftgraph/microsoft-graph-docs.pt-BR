---
title: Tipo de recurso onPremisesExtensionAttributes
description: A **propriedade onPremisesExtensionAttributes** da entidade do usuário contém quinze propriedades de atributo de extensão personalizadas.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: users
author: jpettere
ms.openlocfilehash: aa22c50b940afce1e9da1fac0b094faea3e0ac56
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60559327"
---
# <a name="onpremisesextensionattributes-resource-type"></a>Tipo de recurso onPremisesExtensionAttributes

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O tipo de retorno da **propriedade onPremisesExtensionAttributes** do objeto [de](user.md) usuário e da propriedade **extensionAttributes** do [objeto device.](device.md) Retorna quinze propriedades de atributo de extensão personalizadas.

Na [](user.md) entidade do usuário e para um usuário **onPremisesSyncEnabled,** a fonte de autoridade para esse conjunto de propriedades é o Active Directory local que é sincronizado com o Azure AD e é somente leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é ), essas propriedades podem ser definidas durante a `false` [criação](../api/user-post-users.md) ou [atualização.](../api/user-update.md) Se um usuário somente na nuvem tiver sido sincronizado anteriormente do Active Directory local, essas propriedades não poderão ser gerenciadas por meio da API do Microsoft Graph. Em vez disso, eles podem ser gerenciados por meio do Exchange Admin Center ou do módulo Exchange Online V2 no PowerShell.

A **propriedade extensionAttributes** da entidade [de](device.md) dispositivo é gerenciada somente no Azure AD durante a criação [ou](../api/device-post-devices.md) atualização do [dispositivo.](../api/device-update.md)

> **Observação:** Esses atributos de extensão também são conhecidos como Exchange atributos personalizados 1-15.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|extensionAttribute1|Cadeia de Caracteres| Primeiro atributo de extensão personalizável. |
|extensionAttribute2|Cadeia de Caracteres| Segundo atributo de extensão personalizável. |
|extensionAttribute3|Cadeia de Caracteres| Terceiro atributo de extensão personalizável. |
|extensionAttribute4|Cadeia de Caracteres| Quarto atributo de extensão personalizável. |
|extensionAttribute5|Cadeia de Caracteres| Quinto atributo de extensão personalizável. |
|extensionAttribute6|Cadeia de Caracteres| Sexto atributo de extensão personalizável. |
|extensionAttribute7|Cadeia de Caracteres| Sétimo atributo de extensão personalizável. |
|extensionAttribute8|Cadeia de Caracteres| Oitavo atributo de extensão personalizável. |
|extensionAttribute9|Cadeia de Caracteres| Nono atributo de extensão personalizável. |
|extensionAttribute10|Cadeia de Caracteres| Décimo atributo de extensão personalizável. |
|extensionAttribute11|Cadeia de Caracteres| Décimo primeiro atributo de extensão personalizável. |
|extensionAttribute12|Cadeia de Caracteres| Décimo segundo atributo de extensão personalizável. |
|extensionAttribute13|Cadeia de Caracteres| Décimo terceiro atributo de extensão personalizável. |
|extensionAttribute14|Cadeia de Caracteres| Décimo quarto atributo de extensão personalizável. |
|extensionAttribute15|Cadeia de Caracteres| Décimo quinto atributo de extensão personalizável. |

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


