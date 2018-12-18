---
title: tipo de recurso de alertTrigger
description: Contém informações sobre as propriedades que disparou uma detecção (Propriedades existirem na entidade alerta).
author: Preetikr
ms.openlocfilehash: f0888e6caf78d806909f818a8b72fb21320e7796
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341263"
---
# <a name="alerttrigger-resource-type"></a>tipo de recurso de alertTrigger

Contém informações sobre as propriedades que disparou uma detecção (Propriedades existirem na entidade alerta).

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|name|String|Nome da propriedade servindo como um gatilho de detecção.|
|type|String|Tipo da propriedade no par de chave: valor de interpretação. Por exemplo, String, Boolean, etc.|
|valor|String|Valor da propriedade servindo como um gatilho de detecção.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertTrigger"
}-->

```json
{
  "name": "String",
  "type": "String",
  "value": "String"
}

```

## <a name="example"></a>Exemplo

```json
{
  "name": "hostState.privateIpAddress",
  "type": "String",
  "value": "10.154.9.40"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->