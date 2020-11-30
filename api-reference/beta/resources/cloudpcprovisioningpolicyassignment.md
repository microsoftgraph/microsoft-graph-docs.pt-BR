---
title: tipo de recurso cloudPcProvisioningPolicyAssignment
description: Atribuições de política de provisionamento do CloudPC
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fbbdf76dfb184efdae7279b5d4970367995c0a6c
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378241"
---
# <a name="cloudpcprovisioningpolicyassignment-resource-type"></a>tipo de recurso cloudPcProvisioningPolicyAssignment

Namespace: microsoft.graph

Representa uma coleção definida de atribuições de política de provisionamento.


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
