---
title: Tipo de recurso entitlementManagementSchedule
description: Um cronograma de gerenciamento de direitos pode ser incluído em uma solicitação de atribuição de pacote de acesso e está presente em uma atribuição de pacote de acesso.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 18c814c0426deaa89709505816f21282c75b1757
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650899"
---
# <a name="entitlementmanagementschedule-complex-type"></a>tipo complexo entitlementManagementSchedule

Namespace: microsoft.graph

No gerenciamento de direitos do [Azure AD,](entitlementmanagement-overview.md)uma solicitação de atribuição de pacote de acesso é criada por um usuário que deseja obter uma atribuição de pacote de acesso. Essa solicitação pode incluir um cronograma para quando o usuário gostaria de ter uma atribuição.  Uma atribuição de pacote de acesso que resulta de tal solicitação também tem um cronograma.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|expiration|[expirationPattern](../resources/expirationpattern.md)|Quando o acesso deve expirar.|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|Para acesso recorrente. Não é usado no momento.|
|startDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.entitlementManagementSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.entitlementManagementSchedule",
  "startDateTime": "String (timestamp)",
  "expiration": {
    "@odata.type": "microsoft.graph.expirationPattern"
  },
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  }
}
```


