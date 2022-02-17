---
title: tipo de recurso searchAlteration
description: Fornece os detalhes sobre a alteração de pesquisa para correção ortográfica.
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 9c89193a3d57f8dcb701e57e98160ee69b8a8a91
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878672"
---
# <a name="searchalteration-resource-type"></a>tipo de recurso searchAlteration

Namespace: microsoft.graph

Fornece os detalhes sobre a alteração de pesquisa para correção ortográfica.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|alteredHighlightedQueryString|Cadeia de caracteres| Define a cadeia de caracteres de consulta realçada alterada com correção ortográfica. A anotação em torno do segmento corrigido é: `\ue000, \ue001`.|
|alteredQueryString|Cadeia de caracteres| Define a cadeia de caracteres de consulta alterada com correção ortográfica.|
|alteredQueryTokens|[Coleção alteredQueryToken](alteredquerytoken.md)| Representa segmentos alterados relacionados a uma consulta de usuário original.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchAlteration",
  "baseType": null
}-->

```json
{
  "alteredHighlightedQueryString": "String",
  "alteredQueryString": "String",
  "alteredQueryTokens": [{"@odata.type": "microsoft.graph.alteredQueryToken"}]
}
```
