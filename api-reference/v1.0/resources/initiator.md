---
title: Tipo de recurso iniciador
description: Descreve quem ou o que iniciou o evento de provisionamento.
ms.localizationpriority: medium
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 5a00be289964c749adcea2b7f4df80dd477c1a99
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129856"
---
# <a name="initiator-resource-type"></a>Tipo de recurso iniciador

Namespace: microsoft.graph

Descreve quem ou o que iniciou o evento de provisionamento. 

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|displayName|String|Nome da pessoa ou serviço que iniciou o evento de provisionamento.|
|id|Cadeia de caracteres|Identifica exclusivamente a pessoa ou serviço que iniciou o evento de provisionamento.|
|initiatorType|initiatorType| Tipo de iniciador. Os valores possíveis são: `user`, `application`, `system`, `unknownFutureValue`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.initiator",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "id": "String",
  "initiatorType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "initiator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


