---
title: Tipo de recurso optionalClaim
description: FORNECER A DESCRIÇÃO AQUI
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 0a7b6072b53fe26384f82f706b694c4b04c33113
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128348"
---
# <a name="optionalclaim-resource-type"></a>Tipo de recurso optionalClaim

Namespace: microsoft.graph

Contém uma declaração opcional associada a um [aplicativo](application.md) <!-- or a service principal -->. The `idToken` , and properties of the `accessToken` `saml2Token` [optionalClaims](optionalclaims.md) resource is a collection of **optionalClaim**. Se tiver suporte em uma declaração específica, você também poderá modificar o comportamento do optionalClaim usando a `additionalProperties` propriedade.

Confira [fornecer declarações opcionais ao aplicativo Azure AD](/azure/active-directory/develop/active-directory-optional-claims) para obter mais informações.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|additionalProperties|String collection| Propriedades adicionais da declaração. Se houver uma propriedade nessa coleção, ela modificará o comportamento da declaração opcional especificada na propriedade name. |
|essential|Booliano| Se o valor for verdadeiro, a declaração especificada pelo cliente será necessária para garantir uma experiência de autorização suave para a tarefa específica solicitada pelo usuário final. O valor padrão é falso.|
|nome|String| O nome da declaração opcional. |
|source|String| A origem (objeto de diretório) da declaração. Há declarações predefinidos e declarações definidas pelo usuário a partir de propriedades de extensão. Se o valor de origem for nulo, a declaração será uma declaração opcional predefinida. Se o valor de origem for usuário, o valor na propriedade name será a propriedade de extensão do objeto user. |

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
