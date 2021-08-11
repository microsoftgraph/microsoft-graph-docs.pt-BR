---
title: Tipo de recurso alertTrigger
description: Contém informações sobre as propriedades que dispararam uma detecção (existem propriedades na entidade de alerta).
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: a25f3b624d6e4d725386958a3c26c739276f4aaff207cf2c9bca50f196754d3a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189874"
---
# <a name="alerttrigger-resource-type"></a>Tipo de recurso alertTrigger

Namespace: microsoft.graph

Contém informações sobre as propriedades que dispararam uma detecção (existem propriedades na entidade de alerta).

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|nome|Cadeia de caracteres|Nome da propriedade que serve como um gatilho de detecção.|
|tipo|Cadeia de caracteres|Tipo da propriedade no par key:value para interpretação. Por exemplo, String, Boolean etc.|
|value|Cadeia de caracteres|Valor da propriedade que serve como um gatilho de detecção.|

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

