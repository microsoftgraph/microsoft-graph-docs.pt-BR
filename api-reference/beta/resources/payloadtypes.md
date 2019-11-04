---
title: tipo de recurso payloadTypes
description: Representa o conteúdo de dados de uma notificação de usuário bruto ou Visual que será entregue e consumida pelo cliente do aplicativo que está recebendo esta notificação.
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: 2d740c5b19b363fa2534984bf059cd186b065e89
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939604"
---
# <a name="payloadtypes-resource-type"></a>tipo de recurso payloadTypes

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Esse recurso representa o conteúdo de dados de uma notificação de usuário bruto ou Visual que será entregue e consumido pelo cliente do aplicativo que está recebendo essa notificação.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|rawContent|String|O conteúdo de notificação de uma notificação de usuário bruto que será entregue e consumido pelo cliente de aplicativo em todas as plataformas suportadas (Windows, iOS, Android ou webpush) recebendo esta notificação. Pelo menos um dos payloads. RawContent ou Payload. VisualContent precisa ser válido para uma solicitação de notificação POST.|
|visualContent|[visualproperties](visualproperties.md)|O conteúdo visual de uma notificação de usuário visual, que será consumida pela plataforma de notificação em cada plataforma suportada (Windows, iOS e Android somente) e renderizada para o usuário. Pelo menos um dos payloads. RawContent ou Payload. VisualContent precisa ser válido para uma solicitação de notificação POST.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.payloadTypes",
  "baseType": null
}-->

```json
{
  "rawContent": "String",
  "visualContent": {"@odata.type": "microsoft.graph.visualProperties"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "payloadTypes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->