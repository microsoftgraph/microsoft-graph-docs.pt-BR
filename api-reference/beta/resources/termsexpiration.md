---
title: tipo de recurso termsExpiration
description: Fornece configurações adicionais ao definir a expiração agendada do contrato.
localization_priority: Normal
ms.prod: microsoft-identity-platform
author: raprakasMSFT
doc_type: resourcePageType
ms.openlocfilehash: e811e4816fa63e98201d1a14403d6c3525ace2c0
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/12/2020
ms.locfileid: "46644022"
---
# <a name="termsexpiration-resource-type"></a>tipo de recurso termsExpiration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece configurações adicionais ao definir a expiração agendada do contrato.

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| startDateTime|DateTimeOffset | O DateTime quando o contrato é definido como expire para todos os usuários. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.|
| proje| Duração | Isso representa a frequência com a qual os termos expiram, após a primeira expiração definida em ' startDatetime '. O valor é representado no formato ISO 8601 para durações.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON desse recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.termsExpiration",
  "baseType": ""
}-->

```json
{
   "startDateTime": "2018-10-01T00:00:00.0000000Z",
   "frequency": ""
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
