---
title: tipo de recurso searchAlterationOptions
description: Fornece as opções de alteração de pesquisa para correção ortográfica.
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1692cf40700c9af40b4ecab77b32210291e60f78
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878670"
---
# <a name="searchalterationoptions-resource-type"></a>tipo de recurso searchAlterationOptions

Namespace: microsoft.graph

Fornece as opções de alteração de pesquisa para correção ortográfica.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|enableModification|Booliano|Indica se as modificações ortográficas estão habilitadas. Se habilitado, o usuário receberá os resultados da pesquisa para a consulta corrigida caso não  haja resultados para a consulta original com erros de digitação. A [resposta](/graph/api/resources/searchresponse) também incluirá as informações de modificação ortográfica na **propriedade queryAlterationResponse** . Opcional.|
|enableSuggestion|Booliano|Indica se as sugestões ortográficas estão habilitadas. Se habilitado, o usuário receberá os resultados da pesquisa para a consulta de pesquisa original e sugestões para correção ortográfica na **propriedade queryAlterationResponse** da [](/graph/api/resources/searchresponse) resposta para os erros de digitação na consulta. Opcional.|

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
  "enableModification": "Boolean",
  "enableSuggestion": "Boolean"
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
