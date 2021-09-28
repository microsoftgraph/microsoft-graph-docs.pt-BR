---
title: Tipo de recurso trainingEventsContent
description: Representa eventos de treinamento em uma campanha de simulação e treinamento de ataque.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 489e3b996f86a28f1d555489a30861e5251229f8
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979506"
---
# <a name="trainingeventscontent-resource-type"></a>Tipo de recurso trainingEventsContent

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa eventos de treinamento em uma campanha de simulação e treinamento de ataque.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|assignedTrainingsInfos|[coleção assignedTrainingInfo](../resources/assignedtraininginfo.md)|Lista de treinamentos atribuídos e suas informações em uma campanha de simulação e treinamento de ataque.|
|trainingsAssignedUserCount|Int32|Número de usuários que foram atribuídos treinamentos em uma campanha de simulação e treinamento de ataque.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.trainingEventsContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.trainingEventsContent",
  "trainingsAssignedUserCount": "Integer",
  "assignedTrainingsInfos": [
    {
      "@odata.type": "microsoft.graph.assignedTrainingInfo"
    }
  ]
}
```

