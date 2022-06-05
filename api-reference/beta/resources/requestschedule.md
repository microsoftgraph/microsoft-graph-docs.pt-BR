---
title: Tipo de recurso requestSchedule
description: Um agendamento de solicitação pode ser incluído em uma solicitação de atribuição de pacote de acesso e está presente em uma atribuição de pacote de acesso. No PIM, use esse recurso para definir o agendamento para quando a entidade de segurança terá uma atribuição de função qualificada ou ativa.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 1e8988f70ba9ee108248bbb7ce2322bb0136d00f
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899124"
---
# <a name="requestschedule-resource-type"></a>Tipo de recurso requestSchedule

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [gerenciamento de direitos do Azure AD](entitlementmanagement-overview.md), uma solicitação de atribuição de pacote de acesso é criada por um usuário que deseja obter uma atribuição de pacote de acesso. Essa solicitação pode incluir um agendamento para quando o usuário gostaria de ter uma atribuição.  Uma atribuição de pacote de acesso resultante dessa solicitação também tem um agendamento.

No PIM, use esse recurso para definir o agendamento para quando a entidade de segurança terá uma atribuição de função qualificada ou ativa.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|startDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. No PIM, quando a atribuição qualificada ou ativa se torna ativa.|
|Expiração|[expirationPattern](expirationpattern.md)|No gerenciamento de direitos, quando o acesso deve expirar.|
|recurrence|[patternedRecurrence](patternedrecurrence.md)|Para acesso recorrente ou atribuição qualificada ou ativa. No momento, essa propriedade não tem suporte no gerenciamento de direitos e PIM.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.requestSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.requestSchedule",
  "startDateTime": "String (timestamp)",
  "expiration": {
    "@odata.type": "microsoft.graph.expirationPattern"
  },
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
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


