---
title: tipo de recurso cloudPcProvisioningPolicyAssignment
description: Atribuições de política de provisionamento do CloudPC
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 06a90efc67b483fed569a4e7029a74dac4f7f9ee
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563692"
---
# <a name="cloudpcprovisioningpolicyassignment-resource-type"></a>tipo de recurso cloudPcProvisioningPolicyAssignment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma coleção definida de atribuições de política de provisionamento.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo da atribuição de política de provisionamento. Somente leitura. Se `target` for um grupo de usuários, a ID será mostrada como {PolicyId} _ {GroupId}.|
|destino|[cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md)|O destino da atribuição para a política de provisionamento. Atualmente, o único destino com suporte para essa política é um grupo de usuários.|

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
