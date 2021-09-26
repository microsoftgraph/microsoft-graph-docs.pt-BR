---
title: Tipo de recurso cloudPcManagementGroupAssignmentTarget
description: 'Tipo complexo que representa o grupo de destino de atribuição. Tipo de base: CloudPcManagementAssignmentTarget'
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: a3841cc775b1b0ed9221d193a5ca5d44c61bc6f0
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59765659"
---
# <a name="cloudpcmanagementgroupassignmenttarget-resource-type"></a>Tipo de recurso cloudPcManagementGroupAssignmentTarget

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Tipo complexo que representa o grupo de destino de atribuição.
Herda de [cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md).

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|groupId|Cadeia de caracteres|A id do grupo de destino da atribuição|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.cloudPcManagementAssignmentTarget",
  "@odata.type": "microsoft.graph.cloudPcManagementGroupAssignmentTarget"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcManagementGroupAssignmentTarget",
  "groupId": "String"
}
```
