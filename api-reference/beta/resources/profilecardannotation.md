---
title: tipo de recurso profileCardAnnotation
description: Permite que um administrador Personalize a aparência dos campos selecionados no cartão de perfil do Microsoft 365.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 973732dc92527dcf3795b8796e1c817ba880836c
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050990"
---
# <a name="profilecardannotation-resource-type"></a>tipo de recurso profileCardAnnotation

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado para definir um nome de exibição personalizado para os campos que são exibidos em um Microsoft 365 People experieence compartilhado. Um administrador pode definir uma cadeia de caracteres de nome para exibição padrão e um conjunto de traduções alternativas para os idiomas que eles dão suporte em sua organização.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo                                                            | Descrição                                                                                                                       |
|:-------------|:----------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------|
|displayName   |String                                                           | Se presente, o valor desse campo é usado pelo cartão de perfil como rótulo de propriedade padrão na experiência (por exemplo, "centro de custo"). |
|localizações |coleção [displayNameLocalization](displaynamelocalization.md) | Cada recurso dessa coleção representa o valor localizado do nome do atributo para um determinado idioma, usado como rótulo padrão para essa localidade. Por exemplo, um usuário com um `no-NB` cliente recebe "Kostnads Senter" como o rótulo do atributo, em vez de "centro de custo".|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profileCardAnnotation",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "localizations": [
    {
      "displayName": "String",
      "languageTag": "String"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profileCardAnnotation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
