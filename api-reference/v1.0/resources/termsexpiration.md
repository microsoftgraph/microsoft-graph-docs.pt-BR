---
title: tipo de recurso termsExpiration
description: Fornece configurações adicionais para a expiração agendada do contrato.
localization_priority: Normal
ms.prod: governance
author: raprakasMSFT
doc_type: resourcePageType
ms.openlocfilehash: 80be295857a48854b404da59f2f8f479590fefdc
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722500"
---
# <a name="termsexpiration-resource-type"></a>tipo de recurso termsExpiration

Namespace: microsoft.graph

Fornece configurações adicionais para a expiração agendada do contrato.

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| startDateTime|DateTimeOffset | DateTime quando o contrato está definido para expirar para todos os usuários. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.|
| frequency| Duration | Representa a frequência na qual os termos expiram, após sua primeira expiração, conforme definido em **startDateTime**. O valor é representado no formato ISO 8601 por durações. Por exemplo, `PT1M` representa um período de tempo de 1 mês.|

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON desse recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.termsExpiration",
}-->

```json
{
   "startDateTime": "2018-10-01T00:00:00.0000000Z",
   "frequency": "Duration"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "termsExpiration complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


