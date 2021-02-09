---
title: Tipo de recurso profileCardProperty
description: Usado para designar uma nova propriedade a ser exibida em uma experiência compartilhada, pessoal ou uma que terá um nome de exibição personalizado ou anotação aplicado a ela. Um administrador pode definir uma cadeia de caracteres de nome de exibição padrão e um conjunto de traduções alternativas para os idiomas com suporte na organização.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 33d2b1111580ba2302848ab1dbce3f773055a0b4
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153561"
---
# <a name="profilecardproperty-resource-type"></a>Tipo de recurso profileCardProperty

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um atributo de um usuário no cartão de perfil do Microsoft 365 para uma organização surgir em uma experiência de pessoas compartilhada.

O atributo pode ser um atributo integrado do Azure Active Directory (Azure AD), como ou , ou pode ser `Alias` `UserPrincipalName` um atributo personalizado. Para um atributo personalizado, um administrador pode definir uma cadeia de caracteres de nome de exibição padrão e um conjunto de traduções alternativas para os idiomas aos quais ele dá suporte `en-us` em sua organização.

Para obter mais informações sobre como adicionar propriedades ao cartão de perfil de uma organização, consulte [personalizar o cartão de perfil.](/graph/add-properties-profilecard)

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [List](../api/organizationsettings-list-profilecardproperties.md) | [profileCardProperty](profilecardproperty.md) | Obter uma coleção **de recursos profileCardProperty** de uma organização. |
| [Criar](../api/organizationsettings-post-profilecardproperties.md) | [profileCardProperty](profilecardproperty.md) | Crie um novo **recurso profileCardProperty** para uma organização. |
| [Get](../api/profilecardproperty-get.md) | [profileCardProperty](profilecardproperty.md) | Leia as propriedades e as relações de um recurso **profileCardProperty,** que contém as personalizações de cartão de perfil existentes em uma organização do Microsoft 365 para um determinado campo. |
| [Update](../api/profilecardproperty-update.md)               | [profileCardProperty](profilecardproperty.md) | Atualize **um objeto profileCardProperty.**                               |
| [Delete](../api/profilecardproperty-delete.md)               | Nenhum(a)                                          | **Exclua um objeto profileCardProperty.**                               |

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                                                        | Descrição |
|:---------------------|:------------------------------------------------------------|:------------|
|anotações           |[Coleção profileCardAnnotation](profilecardannotation.md) | Permite que um administrador de definir um rótulo de exibição personalizado para a propriedade de diretório e localizá-lo para os usuários em seu locatário.|
|directoryPropertyName |String                                                       | Identifica um **recurso profileCardProperty** nas [operações Obter,](../api/profilecardproperty-get.md)Atualizar [ou](../api/profilecardproperty-delete.md) Excluir. [](../api/profilecardproperty-update.md) Permite que um administrador surface as propriedades ocultas do Azure Active Directory (Azure AD) no cartão de perfil do Microsoft 365 em seu locatário. Quando presente, o campo do Azure AD referenciado nesse campo ficará visível para todos os usuários em seu locatário no painel de contatos do cartão de perfil. Os valores permitidos para este campo são: `UserPrincipalName` , , , , , , , `Fax` , , , , `StreetAddress` , , , `PostalCode` , , `StateOrProvince` , `Alias` `CustomAttribute1`  `CustomAttribute2` `CustomAttribute3` `CustomAttribute4` `CustomAttribute5` , `CustomAttribute6` `CustomAttribute7` `CustomAttribute8` `CustomAttribute9` `CustomAttribute10` `CustomAttribute11` `CustomAttribute12` `CustomAttribute13` `CustomAttribute14` `CustomAttribute15` . |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profileCardProperty"
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

