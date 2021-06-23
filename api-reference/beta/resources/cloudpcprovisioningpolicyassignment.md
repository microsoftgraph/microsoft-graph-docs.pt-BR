---
title: Tipo de recurso cloudPcProvisioningPolicyAssignment
description: Atribuições de política de provisionamento do CloudPC
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: a96c3717b97b3f721c77b1150841f1eb51ded89f
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082234"
---
# <a name="cloudpcprovisioningpolicyassignment-resource-type"></a>Tipo de recurso cloudPcProvisioningPolicyAssignment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma coleção definida de atribuições de política de provisionamento.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para a atribuição de política de provisionamento. Somente leitura. Se `target` for um grupo de usuários, a ID será mostrada como {policyId} \_ {groupId}.|
|destino|[cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md)|O destino da atribuição da política de provisionamento. Atualmente, o único destino com suporte para essa política é um grupo de usuários. Para obter detalhes, [consulte cloudPcManagementGroupAssignmentTarget](cloudpcmanagementgroupassignmenttarget.md). |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicyAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.cloudPcManagementGroupAssignmentTarget",
    "groupId": "String"
  }
}
```
