---
title: Tipo de recurso resultTemplateOption
description: Fornece as opções de modelo de resultado de pesquisa para renderizar resultados de pesquisa de conectores.
ms.localizationpriority: medium
author: cristianv-ms
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5f1e6b30a1730bfb0e4a667b51c93a47cc3dcb12
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878673"
---
# <a name="resulttemplateoption-resource-type"></a>Tipo de recurso resultTemplateOption

Namespace: microsoft.graph

Fornece as opções de modelo de resultado de pesquisa para renderizar resultados de pesquisa de conectores.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|enableResultTemplate|Booliano|Indica se os layouts de exibição de pesquisa estão habilitados. Se habilitado, o usuário receberá o modelo de resultado para renderizar o conteúdo dos resultados da pesquisa na **propriedade resultTemplates** da [resposta](/graph/api/resources/searchresponse). O modelo de resultado é baseado em [Cartões Adaptáveis](https://adaptivecards.io/). Opcional. |


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
    "enableResultTemplate": "Boolean"
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
