---
title: tipo de recurso clientUserAgent
description: O tipo clientUserAgent
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8a21133cfe70f7c887f8d0ecbc782f1b872d0940
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491921"
---
# <a name="clientuseragent-resource-type"></a>tipo de recurso clientUserAgent

Namespace: microsoft.graph.callRecords

Representa um agente de usuário do cliente de um ponto de extremidade em uma chamada. Herda do tipo [UserAgent](callrecords-useragent.md) .

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|applicationVersion|String|Identifica a versão do software do aplicativo usado por esse ponto de extremidade.|
|headerValue|String|Valor do cabeçalho do agente de usuário relatado por esse ponto de extremidade.|
|platform|Microsoft. Graph. callRecords. clientPlatform|Identifica a plataforma usada por esse ponto de extremidade. Os valores possíveis são: `unknown`, `windows`, `macOS`, `iOS`, `android`, `web`, `ipPhone`, `roomSystem`, `surfaceHub`, `holoLens`, `unknownFutureValue`.|
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