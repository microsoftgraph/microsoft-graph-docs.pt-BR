---
title: Tipo de recurso clientUserAgent
description: O tipo clientUserAgent
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 7c3c97e73d77f16f451c5096bad2105240bf7a9b
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61343676"
---
# <a name="clientuseragent-resource-type"></a>Tipo de recurso clientUserAgent

Namespace: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um agente de usuário cliente de um ponto de extremidade em uma chamada. Herda do [tipo userAgent.](callrecords-useragent.md)

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|applicationVersion|String|Identifica a versão do software de aplicativo usado por esse ponto de extremidade.|
|headerValue|String|Valor de header do agente do usuário relatado por esse ponto de extremidade.|
|plataforma|microsoft.graph.callRecords.clientPlatform|Identifica a plataforma usada por esse ponto de extremidade. Os valores possíveis são: `unknown`, `windows`, `macOS`, `iOS`, `android`, `web`, `ipPhone`, `roomSystem`, `surfaceHub`, `holoLens`, `unknownFutureValue`.|
|productFamily|microsoft.graph.callRecords.productFamily|Identifica a família de softwares de aplicativos usados por esse ponto de extremidade. Os possíveis valores são: `unknown`, `teams`, `skypeForBusiness`, `lync`, `unknownFutureValue`, `azureCommunicationServices`.  Observe que você deve usar o header de solicitação para obter os seguintes valores nesta `Prefer: include-unknown-enum-members` [enum evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `azureCommunicationServices` .|

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

