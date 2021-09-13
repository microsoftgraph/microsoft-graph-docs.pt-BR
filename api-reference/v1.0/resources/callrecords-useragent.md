---
title: Tipo de recurso userAgent
description: O tipo userAgent
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a4154992fd6e187b54a3a794b770e7c53966ce52
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113732"
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
