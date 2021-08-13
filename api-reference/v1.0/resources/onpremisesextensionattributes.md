---
title: Tipo de recurso onPremisesExtensionAttributes
description: A **propriedade onPremisesExtensionAttributes** da entidade do usuário contém quinze propriedades de atributo de extensão personalizadas. Para um usuário **onPremisesSyncEnabled,** esse conjunto de propriedades é mestre no Active Directory local e sincronizado com o Azure AD, e é somente leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas sobre Exchange Online. Os atributos são lidos somente no Microsoft Graph.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 8bc170e1878c1382cdf999211aae8ee0fbf05231c92c297ec87ca11ce64f505e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189405"
---
# <a name="onpremisesextensionattributes-resource-type"></a>Tipo de recurso onPremisesExtensionAttributes

Namespace: microsoft.graph

A **propriedade onPremisesExtensionAttributes** da entidade do usuário contém quinze propriedades de atributo de extensão personalizadas. [](user.md) Para um usuário **onPremisesSyncEnabled,** a fonte de autoridade para esse conjunto de propriedades é o Active Directory local que é sincronizado com o Azure AD e é somente leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** está ), essas propriedades podem ser definidas durante a `false` [criação](../api/user-post-users.md) ou [atualização.](../api/user-update.md)

> **Observação:** Esses atributos de extensão também são conhecidos como Exchange atributos personalizados 1-15.

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
|extensionAttribute8|String| Oitavo atributo de extensão personalizável. |
|extensionAttribute9|String| Nono atributo de extensão personalizável. |
|extensionAttribute10|Cadeia de caracteres| Décimo atributo de extensão personalizável. |
|extensionAttribute11|Cadeia de caracteres| Décimo primeiro atributo de extensão personalizável. |
|extensionAttribute12|String| Décimo segundo atributo de extensão personalizável. |
|extensionAttribute13|Cadeia de caracteres| Décimo terceiro atributo de extensão personalizável. |
|extensionAttribute14|Cadeia de caracteres| Décimo quarto atributo de extensão personalizável. |
|extensionAttribute15|Cadeia de caracteres| Décimo quinto atributo de extensão personalizável. |

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

