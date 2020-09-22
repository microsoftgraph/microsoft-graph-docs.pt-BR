---
title: tipo de recurso targetPolicyEndpoints
description: Representa as plataformas que estão sendo direcionadas para notificações do usuário.
localization_priority: Normal
ms.prod: notifications
doc_type: resourcePageType
author: merzink
ms.openlocfilehash: daac7a8424666d3974512c1cc1b17ec8e6878d7e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985661"
---
# <a name="targetpolicyendpoints-resource-type"></a>tipo de recurso targetPolicyEndpoints

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as plataformas que podem ser direcionadas para receber notificações enviadas ao usuário.  Eles incluem Windows, iOS, Android e Web. 


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|platformTypes|Coleção de cadeias de caracteres|Use para filtrar a distribuição de notificação para uma plataforma ou plataformas específicas. Os valores válidos `Windows` são `iOS` , `Android` e `WebPush` . Por padrão, todos os tipos de ponto de extremidade de envio (Windows, iOS, Android e webpush) estão habilitados. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetPolicyEndpoints",
  "baseType": null
}-->

```json
{
  "platformTypes": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetPolicyEndpoints resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

