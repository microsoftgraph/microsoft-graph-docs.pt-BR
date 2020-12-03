---
title: tipo de recurso cloudPcManagementGroupAssignmentTarget
description: 'Tipo complexo que representa o grupo de destino de atribuição. Tipo de base: CloudPcManagementAssignmentTarget'
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 5216b15a97484bf58d2e2d621dbc26435f180be4
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563835"
---
# <a name="cloudpcmanagementgroupassignmenttarget-resource-type"></a>tipo de recurso cloudPcManagementGroupAssignmentTarget

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Tipo complexo que representa o grupo de destino de atribuição.
Herda de [cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md).

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|groupId|Cadeia de caracteres|A ID do grupo de destino da atribuição|

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
