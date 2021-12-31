---
title: Tipo de recurso expirationPattern
description: O padrão de expiração em um cronograma de solicitação pode ser incluído em uma solicitação de atribuição de pacote de acesso e está presente em uma atribuição de pacote de acesso.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 83ec2f3cafc25787a979103f4edea5e6436b57a9
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650689"
---
# <a name="expirationpattern-resource-type"></a>Tipo de recurso expirationPattern

Namespace: microsoft.graph

No gerenciamento de direitos do [Azure AD,](entitlementmanagement-overview.md)uma solicitação de atribuição de pacote de acesso é criada por um usuário que deseja obter uma atribuição de pacote de acesso. Essa solicitação pode incluir um cronograma para quando o usuário gostaria de ter uma atribuição.  Uma atribuição de pacote de acesso que resulta de tal solicitação também tem um cronograma.  O campo de expiração [de um direitoManagementSchedule](entitlementmanagementschedule.md) indica quando a atribuição do pacote de acesso deve expirar.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|duração|Duração|A duração desejada do acesso do solicitante representada no formato ISO 8601 por durações. Por exemplo, PT3H refere-se a três horas.  Se especificado em uma solicitação, **endDateTime** não deve estar presente e a propriedade **type** deve ser definida como `afterDuration` .|
|endDateTime|DateTimeOffset|Data e hora de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|type|[expirationPatternType](#expirationpatterntype-values)|O tipo de padrão de expiração desejado do solicitante. Os valores possíveis são: `notSpecified`, `noExpiration`, `afterDateTime`, `afterDuration`. |

### <a name="expirationpatterntype-values"></a>valores expirationPatternType

| Member | Descrição |
|:---------------|:--------|
|notSpecified|Nenhum cronograma de expiração foi especificado.|
|noExpiration|O solicitante não desejou que o acesso expirar.|
|afterDateTime|O acesso expirará após uma data e hora especificadas.|
|afterDuration|O acesso expirará após uma duração especificada relativa ao acesso que está sendo concedido. Obrigatório quando a **propriedade duration** for especificada.|

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


