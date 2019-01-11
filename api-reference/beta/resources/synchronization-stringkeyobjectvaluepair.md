---
title: tipo de recurso de stringKeyObjectValuePair
description: Representa um par de chave-valor em que a chave é uma cadeia de caracteres e o valor é um objeto JSON arbitrário. Este é um tipo de open do OData que espera tem uma propriedade denominada `value` ou seja um objeto JSON válido.
localization_priority: Normal
ms.openlocfilehash: 8545a4ef5a4931d3b886c95b4f39218bc418f53d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831448"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a>tipo de recurso de stringKeyObjectValuePair

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa um par de chave-valor em que a chave é uma cadeia de caracteres e o valor é um objeto JSON arbitrário. Este é um tipo de open do OData que espera tem uma propriedade denominada `value` ou seja um objeto JSON válido.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|key|Cadeia de caracteres|Chave.|
|valor|Qualquer|Objeto JSON arbitrário.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyObjectValuePair"
}-->

```json
{
  "key": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "stringKeyObjectValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
