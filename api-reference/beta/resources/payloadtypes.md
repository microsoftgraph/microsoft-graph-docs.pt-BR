---
title: tipo de recurso payloadTypes
description: Representa o conteúdo de dados de uma notificação de usuário bruto ou Visual que será entregue e consumida pelo cliente do aplicativo que está recebendo esta notificação.
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: 034770f2614bacdb9d160f4ff8d2efb4cd0a2c24
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998090"
---
# <a name="payloadtypes-resource-type"></a>tipo de recurso payloadTypes

Namespace: microsoft.graph

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

