---
title: tipo de recurso clientUserAgent
description: O tipo clientUserAgent
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c22a957262c471fad480dd0313595c05c05ec83d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601768"
---
# <a name="clientuseragent-resource-type"></a>tipo de recurso clientUserAgent

Namespace: microsoft.graph.callRecords

Representa um agente de usuário do cliente de um ponto de extremidade em uma chamada. Herda do tipo [UserAgent](callrecords-useragent.md) .

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|applicationVersion|String|Identifica a versão do software do aplicativo usado por esse ponto de extremidade.|
|headerValue|String|Valor do cabeçalho do agente de usuário relatado por esse ponto de extremidade.|
|plataforma|Microsoft. Graph. callRecords. clientPlatform|Identifica a plataforma usada por esse ponto de extremidade. Os valores possíveis são: `unknown`, `windows`, `macOS`, `iOS`, `android`, `web`, `ipPhone`, `roomSystem`, `surfaceHub`, `holoLens`, `unknownFutureValue`.|
|productFamily|Microsoft. Graph. callRecords. productFamily|Identifica a família de software de aplicativo usada por esse ponto de extremidade. Os valores possíveis são: `unknown`, `teams`, `skypeForBusiness`, `lync`, `unknownFutureValue`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.clientUserAgent",
  "baseType": "microsoft.graph.callRecords.userAgent"
}-->

```json
{
  "applicationVersion": "String",
  "headerValue": "String",
  "platform": "String",
  "productFamily": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "clientUserAgent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
