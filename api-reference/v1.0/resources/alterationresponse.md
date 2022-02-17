---
title: Tipo de recurso de alterationResponse
description: Fornece informações relacionadas a correções ortográficas na resposta à alteração.
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: b26b3aee1db86018b8a32f5e2a4bb1b245ee7c5a
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2022
ms.locfileid: "62879259"
---
# <a name="alterationresponse-resource-type"></a>Tipo de recurso de alterationResponse

Namespace: microsoft.graph

Fornece informações relacionadas a correções ortográficas na resposta à alteração.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|originalQueryString|Cadeia de caracteres| Define a cadeia de caracteres de consulta do usuário original.|
|queryAlteration|[searchAlteration](searchalteration.md)| Define os detalhes das informações de alteração para a correção ortográfica.|
|queryAlterationType|searchAlterationType| Define o tipo de correção ortográfica. Os valores possíveis são: `suggestion` e `modification`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alterationResponse",
  "baseType": null
}-->

```json
{
  "originalQueryString": "String",
  "queryAlteration": "String",
  "queryAlterationType": "String"
}
```
