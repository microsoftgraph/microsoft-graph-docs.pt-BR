---
title: Tipo de recurso userAgent
description: O tipo userAgent
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3a32c74957d0d0a2c41323c1f76d4e990897d61948892821e2d56154eceec271
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189916"
---
# <a name="useragent-resource-type"></a>Tipo de recurso userAgent

Namespace: microsoft.graph.callRecords

Representa o agente do usuário de um ponto de extremidade em uma chamada.
Os [tipos clientUserAgent](callrecords-clientuseragent.md) [e serviceUserAgent](callrecords-serviceuseragent.md)) herdam desse tipo.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|applicationVersion|String|Identifica a versão do software de aplicativo usado por esse ponto de extremidade.|
|headerValue|Cadeia de caracteres|Valor de header do agente do usuário relatado por esse ponto de extremidade.|

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
