---
title: tipo de recurso optionalClaim
description: FORNEÇA UMA DESCRIÇÃO AQUI
localization_priority: Normal
author: sureshja
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: de97333a2a7580e9b6a9b58e042c0c5a8ff9bbe7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534125"
---
# <a name="optionalclaim-resource-type"></a>tipo de recurso optionalClaim

Namespace: microsoft.graph

Contém uma declaração opcional associada a um [aplicativo](application.md) <!-- or a service principal -->. As `idToken`propriedades `accessToken`,, `saml2Token` e do recurso [optionalClaims](optionalclaims.md) é uma coleção de **optionalClaim**. Se houver suporte para uma declaração específica, você também poderá modificar o comportamento do optionalClaim usando a `additionalProperties` propriedade.

Confira [fornecer declarações opcionais ao aplicativo Azure AD](/azure/active-directory/develop/active-directory-optional-claims) para obter mais informações.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|AdditionalProperties|String collection| Propriedades adicionais da declaração. Se uma propriedade existir nessa coleção, ela modificará o comportamento da declaração opcional especificada na propriedade Name. |
|essencial|Booliano| Se o valor for true, a declaração especificada pelo cliente será necessária para garantir uma experiência de autorização suave para a tarefa específica solicitada pelo usuário final. O valor padrão é falso.|
|nome|String| O nome da declaração opcional. |
|source|String| A origem (objeto de diretório) da declaração. Há declarações predefinidas e declarações definidas pelo usuário das propriedades de extensão. Se o valor de origem for nulo, a declaração será uma declaração opcional predefinida. Se o valor de origem for User, o valor na propriedade Name será a Propriedade Extension do objeto user. |

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