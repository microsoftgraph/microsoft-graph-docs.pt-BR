---
title: tipo de recurso targetPolicyEndpoints
description: Representa as plataformas que estão sendo direcionadas para notificações do usuário.
localization_priority: Normal
ms.prod: notifications
doc_type: resourcePageType
author: merzink
ms.openlocfilehash: 92ff6d0748e24fd58154f596188f25c51bdc6403
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519999"
---
# <a name="targetpolicyendpoints-resource-type"></a>tipo de recurso targetPolicyEndpoints

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as plataformas que podem ser direcionadas para receber notificações enviadas ao usuário.  Eles incluem Windows, iOS, Android e Web. 


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|platformTypes|String collection|Use para filtrar a distribuição de notificação para uma plataforma ou plataformas específicas. Os valores válidos `Windows`são `iOS`, `Android` e `WebPush`. Por padrão, todos os tipos de ponto de extremidade de envio (Windows, iOS, Android e webpush) estão habilitados. |

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