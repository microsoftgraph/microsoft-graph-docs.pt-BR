---
title: Tipo de recurso traceRouteHop
description: Representa os saltos de rota de rastreamento de rede coletados para um fluxo de mídia.
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 31e64989212bc5666b2010d2319bc55bdce11fb6
ms.sourcegitcommit: 69b150e408c0b9a0705bf33229269f6e5371bc6c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2022
ms.locfileid: "65924185"
---
# <a name="traceroutehop-resource-type"></a>Tipo de recurso traceRouteHop

Namespace: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os saltos de rota de rastreamento de rede coletados para um [fluxo de mídia](callrecords-mediastream.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|hopCount|Int32|A contagem de caminho de rede desse salto que foi usado para calcular o RTT.|
|ipAddress|Cadeia de caracteres|Endereço IP usado para esse salto no rastreamento de rede.|
|Roundtriptime|Duration|A hora em que o pacote de rota de rastreamento foi enviado do cliente para esse salto e de volta para o cliente, indicado no [formato ISO 8601][] . Por exemplo, 1 segundo é indicado `PT1S`como , em que P é o designador de duração, T é o designador de tempo e S é o segundo designador.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callRecords.traceRouteHop"
}-->

```json
{
  "hopCount": "Int32",
  "ipAddress": "String",
  "roundTripTime": "String (duration)"
}
```

[ISO 8601]: https://www.iso.org/iso/iso8601
