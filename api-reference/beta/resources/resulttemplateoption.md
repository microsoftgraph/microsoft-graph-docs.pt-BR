---
title: Tipo de recurso resultTemplateOption
description: Fornece as opções de layouts de exibição de pesquisa para resultados de pesquisa de conectores de renderização.
localization_priority: Normal
author: cristianv-ms
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 404051f4eeee68ca3d5f5eb3ac6b84a23a331515
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211201"
---
# <a name="resulttemplateoption-resource-type"></a>Tipo de recurso resultTemplateOption

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece as opções de modelos de resultados de pesquisa para resultados de pesquisa de conectores de renderização.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|enableResultTemplate|Booliano|Indica se os layouts de exibição de pesquisa estão habilitados. Se habilitado, o usuário receberá o modelo de resultado para renderizar o conteúdo dos resultados da pesquisa na **propriedade resultTemplates** da [resposta](/graph/api/resources/searchresponse?view=graph-rest-beta&preserve-view=true). O modelo de resultado baseia-se em [Cartões Adaptáveis.](https://adaptivecards.io/) Essa propriedade é opcional.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultTemplateOption",
  "baseType": null
}-->

```json
 {
    "enableResultTemplate": true
 }
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resultTemplateOption resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
