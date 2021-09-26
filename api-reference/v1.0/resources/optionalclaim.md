---
title: Tipo de recurso optionalClaim
description: FORNECER DESCRIÇÃO AQUI
ms.localizationpriority: medium
author: sureshja
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: e7479cc139fbe5dcdb8051ab2dc9a486b4de3c17
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59508430"
---
# <a name="optionalclaim-resource-type"></a>Tipo de recurso optionalClaim

Namespace: microsoft.graph

Contém uma declaração opcional associada a um [aplicativo](application.md) <!-- or a service principal -->. As `idToken` propriedades , e do recurso `accessToken` `saml2Token` [optionalClaims](optionalclaims.md) são uma coleção **de optionalClaim**. Se tiver suporte para uma declaração específica, você também poderá modificar o comportamento do optionalClaim usando a `additionalProperties` propriedade.

Para obter mais informações, [consulte provide optional claims to your Azure AD app](/azure/active-directory/develop/active-directory-optional-claims).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|additionalProperties|Coleção de cadeias de caracteres| Propriedades adicionais da declaração. Se uma propriedade existir nessa coleção, ela modificará o comportamento da declaração opcional especificada na propriedade name. |
|essential|Boolean| Se o valor for verdadeiro, a declaração especificada pelo cliente será necessária para garantir uma experiência de autorização suave para a tarefa específica solicitada pelo usuário final. O valor padrão é falso.|
|name|Cadeia de caracteres| O nome da declaração opcional. |
|source|String| A origem (objeto directory) da declaração. Há declarações predefinidos e declarações definidas pelo usuário de propriedades de extensão. Se o valor de origem for nulo, a declaração será uma declaração opcional predefinida. Se o valor de origem for usuário, o valor na propriedade name será a propriedade extension do objeto user. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.optionalClaim",
  "baseType": null
}-->

```json
{
  "additionalProperties": ["String"],
  "essential": true,
  "name": "String",
  "source": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "optionalClaim resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
