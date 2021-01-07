---
title: tipo de recurso expirationPattern
description: O padrão de validade em um agendamento de solicitação pode ser incluído em uma solicitação de atribuição de pacote do Access e está presente em uma atribuição de pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5a6ae13816c3b59905ee66ad5d2d18f6a71270bd
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777610"
---
# <a name="expirationpattern-resource-type"></a>tipo de recurso expirationPattern

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma solicitação de atribuição de pacote de acesso é criada por um usuário que deseja obter uma atribuição de pacote do Access. Essa solicitação pode incluir um cronograma para quando o usuário quiser ter uma atribuição.  Uma atribuição de pacote do Access que resulta de tal solicitação também tem um cronograma.  O campo de expiração de um [requestSchedule](requestschedule.md) indica quando a atribuição de pacote de acesso deve expirar.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|endDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|duração|Duração|A duração de acesso desejada do solicitante. Se especificado em uma solicitação, EndDateTime não deve estar presente.|
|type|expirationPatternType|O tipo de padrão de expiração desejado do solicitante.|

### <a name="expirationpatterntype-values"></a>valores de expirationPatternType

| Membro | Valor| Descrição |
|:---------------|:--------|:----------|
|Não especificado|,0|Nenhum cronograma de expiração especificado.|
|noexpiração|1 |O solicitante não quis que o acesso expire.|
|afterDateTime|2 |O Access expirará após uma data e hora especificadas.|
|afterDuration|3 |O Access expirará após uma determinada duração relativa ao acesso concedido.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expirationPattern"
}-->

```json
{
    "endDateTime": "2020-09-10T23:06:53.307Z",
    "type": "afterDateTime"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "expirationPattern resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


