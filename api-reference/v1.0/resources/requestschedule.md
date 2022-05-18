---
title: Tipo de recurso requestSchedule
description: No PIM, use esse recurso para definir o agendamento para quando a entidade de segurança terá uma função qualificada ou ativa.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 59adc6589ea351d565248797aeb9384b9ae3f890
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461440"
---
# <a name="requestschedule-resource-type"></a>Tipo de recurso requestSchedule

Namespace: microsoft.graph

No PIM ao criar ou atualizar um objeto [unifiedRoleAssignmentScheduleRequest](unifiedroleassignmentschedulerequest.md) ou [unifiedRoleEligibilityScheduleRequest](unifiedroleeligibilityschedulerequest.md) , use esse recurso para definir o agendamento de quando a entidade de segurança terá uma atribuição de função qualificada ou ativa. As configurações permitidas para esse objeto dependem das [configurações para a Azure AD função](../api/unifiedrolemanagementpolicy-list-rules.md).

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

