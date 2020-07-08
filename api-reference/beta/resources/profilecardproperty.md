---
title: tipo de recurso profileCardProperty
description: Usado para designar uma nova propriedade à superfície em uma experiência compartilhada, de pessoas ou uma que terá um nome de exibição ou uma anotação personalizada aplicada a ela. Um administrador pode definir uma cadeia de caracteres de nome para exibição padrão e um conjunto de traduções alternativas para os idiomas que eles dão suporte em sua organização.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a577d050ae55ec7b99cbceb23f27a6dd4ec2121f
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081358"
---
# <a name="profilecardproperty-resource-type"></a>tipo de recurso profileCardProperty

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um atributo de um usuário no cartão de perfil do Microsoft 365 para uma organização apresentar uma experiência de pessoas compartilhada.

O atributo pode ser um atributo interno do Azure Active Directory (Azure AD), como `Alias` ou `UserPrincipalName` , ou pode ser um atributo personalizado. Para um atributo personalizado, um administrador pode definir uma `en-us` cadeia de caracteres de nome de exibição padrão e um conjunto de traduções alternativas para os idiomas que eles dão suporte em sua organização.

Para obter mais informações sobre como adicionar propriedades ao cartão de perfil de uma organização, consulte [Customize The Profile Card](/graph/add-properties-profilecard).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [Listar](../api/organizationsettings-list-profilecardproperties.md) | [profileCardProperty](profilecardproperty.md) | Leia as propriedades e os relacionamentos de um objeto **profileCardProperty** . |
| [Criar](../api/organizationsettings-post-profilecardproperties.md) | [profileCardProperty](profilecardproperty.md) | Leia as propriedades e os relacionamentos de um objeto **profileCardProperty** . |
| [Get](../api/profilecardproperty-get.md) | [profileCardProperty](profilecardproperty.md) | Leia as propriedades e os relacionamentos de um objeto **profileCardProperty** . |
| [Update](../api/profilecardproperty-update.md)               | [profileCardProperty](profilecardproperty.md) | Atualizar um objeto **profileCardProperty** .                               |
| [Delete](../api/profilecardproperty-delete.md)               | Nenhuma                                          | Excluir um objeto **profileCardProperty** .                               |

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                                                        | Descrição |
|:---------------------|:------------------------------------------------------------|:------------|
|anotações           |coleção [profileCardAnnotation](profilecardannotation.md) | Permite que um administrador defina um rótulo de exibição personalizado para a propriedade Directory e o localize para os usuários em seu locatário.|
|directoryPropertyName |String                                                       | Identifica um recurso do **profileCardProperty** em operações [Get](../api/profilecardproperty-get.md), [Update](../api/profilecardproperty-update.md)ou [delete](../api/profilecardproperty-delete.md) . Permite que um administrador Surface as propriedades do Azure Active Directory (Azure AD) ocultas no cartão de perfil do Microsoft 365 dentro de seu locatário. Quando presente, o campo do Azure AD mencionado neste campo ficará visível para todos os usuários em seu locatário no painel de contato do cartão de perfil. Os valores permitidos para este campo são:,,,,,,,,,, `UserPrincipalName` `Fax` `StreetAddress` `PostalCode` `StateOrProvince` `Alias` `CustomAttribute1` `CustomAttribute2` `CustomAttribute3` `CustomAttribute4` `CustomAttribute5` `CustomAttribute6` , `CustomAttribute7` , `CustomAttribute8` , `CustomAttribute9` , `CustomAttribute10` , `CustomAttribute11` , `CustomAttribute12` `CustomAttribute13` `CustomAttribute14` `CustomAttribute15` ,,,,,,,. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profileCardProperty",
  "baseType": ""
}-->

```json
{
  "annotations": [
    {
      "displayName": "String",
      "localizations": [
        {
          "languageTag": "String",
          "displayName": "String"
        }
      ]
    }
  ],
  "directoryPropertyName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profileCardProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->