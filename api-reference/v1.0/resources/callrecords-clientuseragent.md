---
title: Tipo de recurso clientUserAgent
description: O tipo clientUserAgent
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6c1150cf60b3b042358ff1a854944b14722e2a9717daaed064d9d63392e475aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54212210"
---
# <a name="clientuseragent-resource-type"></a>Tipo de recurso clientUserAgent

Namespace: microsoft.graph.callRecords

Representa um agente de usuário cliente de um ponto de extremidade em uma chamada. Herda do [tipo userAgent.](callrecords-useragent.md)

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|applicationVersion|String|Identifica a versão do software de aplicativo usado por esse ponto de extremidade.|
|headerValue|Cadeia de caracteres|Valor de header do agente do usuário relatado por esse ponto de extremidade.|
|plataforma|microsoft.graph.callRecords.clientPlatform|Identifica a plataforma usada por esse ponto de extremidade. Os valores possíveis são: `unknown`, `windows`, `macOS`, `iOS`, `android`, `web`, `ipPhone`, `roomSystem`, `surfaceHub`, `holoLens`, `unknownFutureValue`.|
|productFamily|microsoft.graph.callRecords.productFamily|Identifica a família de softwares de aplicativos usados por esse ponto de extremidade. Os valores possíveis são: `unknown`, `teams`, `skypeForBusiness`, `lync`, `unknownFutureValue`.|

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
