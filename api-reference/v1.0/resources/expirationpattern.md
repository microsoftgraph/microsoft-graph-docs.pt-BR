---
title: Tipo de recurso expirationPattern
description: O padrão de expiração define quando uma solicitação ou atribuição expira.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a42454acfb8c6dc50077fdd85fc7fcf9fa8086e5
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461328"
---
# <a name="expirationpattern-resource-type"></a>Tipo de recurso expirationPattern

Namespace: microsoft.graph

No [Azure AD de](entitlementmanagement-overview.md) direitos, uma solicitação de atribuição de pacote de acesso é criada por um usuário que deseja obter uma atribuição de pacote de acesso. Essa solicitação pode incluir um agendamento para quando o usuário gostaria de ter uma atribuição. Uma atribuição de pacote de acesso resultante dessa solicitação também tem um agendamento. O campo de expiração [de um direitoManagementSchedule](entitlementmanagementschedule.md) indica quando a atribuição do pacote de acesso deve expirar.

No PIM, use esse recurso para definir quando um [objeto unifiedRoleAssignmentScheduleRequest](unifiedroleassignmentschedulerequest.md) ou [unifiedRoleEligibilityScheduleRequest](unifiedroleeligibilityschedulerequest.md) expirar. As configurações permitidas para esse objeto dependem das [configurações para a Azure AD função](../api/unifiedrolemanagementpolicy-list-rules.md). Por exemplo, se as configurações da função Azure AD especificam que as atribuições qualificadas permanentes não são permitidas, `noExpiration` especificar para a propriedade **type** retornará um erro.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|duração|Duration|A duração desejada do acesso do solicitante representada no formato ISO 8601 por durações. Por exemplo, PT3H refere-se a três horas.  Se especificado em uma solicitação, **endDateTime** não deve estar presente e a propriedade **type** deve ser definida como `afterDuration`.|
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


