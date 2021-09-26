---
title: Tipo de recurso cloudPcUserSettingAssignment
description: Representa uma coleção definida de atribuições de configuração do usuário.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 8924dd6339017bbe848747e8d00df49c2f4c71cd
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766947"
---
# <a name="cloudpcusersettingassignment--resource-type"></a>Tipo de recurso cloudPcUserSettingAssignment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma coleção definida de atribuições de configuração do usuário.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da atribuição de configuração do usuário. Somente leitura. Se `target` for um grupo de usuários, a ID terá essa estrutura: {policyID} \_ {groupID}.|
|destino|[cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md)|O destino de atribuição para a configuração do usuário. Atualmente, o único destino com suporte para essa configuração de usuário é um grupo de usuários. Para obter detalhes, [consulte cloudPcManagementGroupAssignmentTarget](cloudpcmanagementgroupassignmenttarget.md).|
|createdDateTime|DateTimeOffset|A data e a hora em que essa atribuição foi criada. O tipo Timestamp representa as informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 tem esta aparência: '2014-01-01T00:00:00Z'.  |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcUserSettingAssignment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcUserSettingAssignment",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "target": {
    "@odata.type": "microsoft.graph.cloudPcManagementAssignmentTarget"
  }
}
```
