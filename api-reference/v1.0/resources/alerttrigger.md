---
title: Tipo de recurso alertTrigger
description: Contém informações sobre as propriedades que dispararam uma detecção (existem propriedades na entidade de alerta).
author: preetikr
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 78cfe6afd2495291dd3d4b358ab500b41dab25d0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59089876"
---
# <a name="alerttrigger-resource-type"></a>Tipo de recurso alertTrigger

Namespace: microsoft.graph

Contém informações sobre as propriedades que dispararam uma detecção (existem propriedades na entidade de alerta).

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|nome|String|Nome da propriedade que serve como um gatilho de detecção.|
|tipo|String|Tipo da propriedade no par key:value para interpretação. Por exemplo, String, Boolean etc.|
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

