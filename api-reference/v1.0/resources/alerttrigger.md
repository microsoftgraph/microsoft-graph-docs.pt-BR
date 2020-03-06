---
title: tipo de recurso alertTrigger
description: Contém informações sobre as propriedades que acionaram uma detecção (as propriedades existem na entidade de alerta).
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 75663b351004d31884f58c53a1ce91e035b0414c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532150"
---
# <a name="alerttrigger-resource-type"></a>tipo de recurso alertTrigger

Namespace: microsoft.graph

Contém informações sobre as propriedades que acionaram uma detecção (as propriedades existem na entidade de alerta).

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|nome|String|Nome da propriedade servindo como um gatilho de detecção.|
|type|String|Tipo da propriedade no par chave: valor para interpretação. Por exemplo, String, Boolean, etc.|
|value|Cadeia de caracteres|O valor da propriedade servindo como um gatilho de detecção.|

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
