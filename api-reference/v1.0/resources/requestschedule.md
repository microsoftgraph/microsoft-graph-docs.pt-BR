---
title: Tipo de recurso requestSchedule
description: No PIM, use esse recurso para definir o agendamento para quando a entidade de segurança terá uma função qualificada ou ativa.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 67fb91da3601c467e33725064ca68753f35eab86
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133888"
---
# <a name="requestschedule-resource-type"></a>Tipo de recurso requestSchedule

Namespace: microsoft.graph

No PIM, use esse recurso para definir o agendamento para quando a entidade de segurança terá uma atribuição de função qualificada ou ativa.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Expiração|[expirationPattern](../resources/expirationpattern.md)|Quando a atribuição qualificada ou ativa expirar.|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|A frequência da atribuição qualificada ou ativa. No momento, não há suporte para essa propriedade no PIM.|
|startDateTime|DateTimeOffset|Quando a atribuição qualificada ou ativa se torna ativa.|

## <a name="relationships"></a>Relações
Nenhum

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

