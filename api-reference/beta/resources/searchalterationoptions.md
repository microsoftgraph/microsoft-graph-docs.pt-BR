---
title: tipo de recurso searchAlterationOptions
description: Fornece as opções de alteração de pesquisa para correção ortográfica.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: dc17698715b4ea6e894ae13f1999e78ab361cc5e
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067886"
---
# <a name="searchalterationoptions-resource-type"></a>tipo de recurso searchAlterationOptions

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece as opções de alteração de pesquisa para correção ortográfica.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|enableSuggestion|Boolean|Indica se as sugestões ortográficas estão habilitadas. Se habilitado, o usuário receberá os resultados da pesquisa para consulta de pesquisa original e [](/graph/api/resources/searchresponse?view=graph-rest-beta&preserve-view=true) sugerirá correção ortográfica na **propriedade queryAlterationResponse** da resposta para erros de digitação na consulta. Opcional.|
|enableModification|Boolean|Indica se as modificações ortográficas estão habilitadas. Se habilitado, o usuário receberá os resultados  da pesquisa para consulta corrigida quando não houver resultados para a consulta original com erros de digitação e obterá as informações de modificação ortográfica na propriedade **queryAlterationResponse** da resposta [.](/graph/api/resources/searchresponse?view=graph-rest-beta&preserve-view=true) Opcional.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchAlterationOptions",
  "baseType": null
}-->

```json
{
  "enableSuggestion": true,
  "enableModification": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchAlterationOptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
