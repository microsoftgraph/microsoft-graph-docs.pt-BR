---
title: Tipo de recurso requestSchedule
description: Um agendamento de solicitação pode ser incluído em uma solicitação de atribuição de pacote de acesso e está presente em uma atribuição de pacote de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 74fa9589552ba860962c73814e66332eda1c8e8f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132535"
---
# <a name="requestschedule-resource-type"></a>Tipo de recurso requestSchedule

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)uma solicitação de atribuição de pacote de acesso é criada por um usuário que deseja obter uma atribuição de pacote de acesso. Essa solicitação pode incluir um cronograma para quando o usuário gostaria de ter uma atribuição.  Uma atribuição de pacote de acesso que resulta de tal solicitação também tem um cronograma.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|startDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|expiration|[expirationPattern](expirationpattern.md)|Quando o acesso deve expirar.|
|recurrence|[patternedRecurrence](patternedrecurrence.md)|Para acesso recorrente. Não usado no momento.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestSchedule"
}-->

```json
{
    "startDateTime": "2020-08-11T23:06:53.307Z",
    "expiration": {
        "endDateTime": "2020-09-10T23:06:53.307Z",
        "type": "afterDateTime"
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requestSchedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


