---
title: tipo de recurso UserAgent
description: O tipo UserAgent
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 952cdc1aa293b393c55491590a7da7a25f6f9507
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394655"
---
# <a name="useragent-resource-type"></a>tipo de recurso UserAgent

Namespace: Microsoft. Graph. callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o agente do usuário de um ponto de extremidade em uma chamada.
Os tipos [clientUserAgent](callrecords-clientuseragent.md) e [serviceUserAgent](callrecords-serviceuseragent.md)) são herdados desse tipo.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|applicationVersion|String|Identifica a versão do software do aplicativo usado por esse ponto de extremidade.|
|headerValue|String|Valor do cabeçalho do agente de usuário relatado por esse ponto de extremidade.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.userAgent",
  "baseType": null
}-->

```json
{
  "applicationVersion": "String",
  "headerValue": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userAgent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->