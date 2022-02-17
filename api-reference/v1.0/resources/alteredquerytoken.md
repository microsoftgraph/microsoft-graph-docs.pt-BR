---
title: Tipo de recurso alteredQueryToken
description: Representa segmentos alterados relacionados a uma consulta de usuário original.
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: edd8a8d121fb28d129fb9a21bf18112ea37f545c
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2022
ms.locfileid: "62879263"
---
# <a name="alteredquerytoken-resource-type"></a>Tipo de recurso alteredQueryToken

Namespace: microsoft.graph

Representa segmentos alterados relacionados a uma consulta de usuário original.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|Comprimento|Int32| Define o comprimento de um segmento alterado.|
|offset|Int32| Define o deslocamento de um segmento alterado.|
|suggestion|String| Representa a cadeia de caracteres de segmento corrigido.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alteredQueryToken",
  "baseType": null
}-->

```json
{
  "length": "Int32",
  "offset": "Int32",
  "suggestion": "String"
}
```
