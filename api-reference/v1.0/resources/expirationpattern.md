---
title: Tipo de recurso expirationPattern
description: O padrão de expiração define quando uma solicitação ou atribuição expira.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 03810c04707d9b53a0254cbb4d322f4d5696b0d0
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133193"
---
# <a name="expirationpattern-resource-type"></a>Tipo de recurso expirationPattern

Namespace: microsoft.graph

No [Azure AD de](entitlementmanagement-overview.md) direitos, uma solicitação de atribuição de pacote de acesso é criada por um usuário que deseja obter uma atribuição de pacote de acesso. Essa solicitação pode incluir um agendamento para quando o usuário gostaria de ter uma atribuição. Uma atribuição de pacote de acesso resultante dessa solicitação também tem um agendamento. O campo de expiração [de um direitoManagementSchedule](entitlementmanagementschedule.md) indica quando a atribuição do pacote de acesso deve expirar.

No PIM, use esse recurso para definir quando um [objeto unifiedRoleAssignmentScheduleRequest](unifiedroleassignmentschedulerequest.md) ou [unifiedRoleEligibilityScheduleRequest](unifiedroleeligibilityschedulerequest.md) expirar.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|duração|Duração|A duração desejada do acesso do solicitante representada no formato ISO 8601 por durações. Por exemplo, PT3H refere-se a três horas.  Se especificado em uma solicitação, **endDateTime** não deve estar presente e a propriedade **type** deve ser definida como `afterDuration`.|
|endDateTime|DateTimeOffset|Carimbo de data e hora de informações usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|type|[expirationPatternType](#expirationpatterntype-values)|O tipo de padrão de expiração desejado do solicitante. Os valores possíveis são: `notSpecified`, `noExpiration`, `afterDateTime`, `afterDuration`. |

### <a name="expirationpatterntype-values"></a>Valores expirationPatternType

| Member | Descrição |
|:---------------|:--------|
|Notspecified|Nenhum agendamento de expiração foi especificado.|
|noExpiration|O solicitante não queria que o acesso expirar.|
|afterDateTime|O acesso expirará após uma data e hora especificadas.|
|afterDuration|O acesso expirará após uma duração especificada em relação ao acesso que está sendo concedido. Obrigatório quando a **propriedade duration** é especificada.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.expirationPattern"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.expirationPattern",
  "endDateTime": "String (timestamp)",
  "duration": "String (duration)",
  "type": "String"
}
```


