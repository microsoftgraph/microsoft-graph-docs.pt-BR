---
title: tipo de recurso cloudPcManagementGroupAssignmentTarget
description: 'Tipo complexo que representa o grupo de destino de atribuição. Tipo de base: CloudPcManagementAssignmentTarget'
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7a6d046452bb3e9944712746ec7ef72914737186
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378264"
---
# <a name="cloudpcmanagementgroupassignmenttarget-resource-type"></a>tipo de recurso cloudPcManagementGroupAssignmentTarget

Namespace: microsoft.graph

Tipo complexo que representa o grupo de destino de atribuição.
Herda de [cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md).

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
