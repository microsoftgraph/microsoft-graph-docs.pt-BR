---
title: Tipo de recurso attackSimulationTrainingUserCoverage
description: Representa a cobertura de treinamento para um usuário em simulação de ataque e treinamento.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: ac8772817fa4c5887a1ae84c80165794b4bed16c
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979494"
---
# <a name="attacksimulationtrainingusercoverage-resource-type"></a>Tipo de recurso attackSimulationTrainingUserCoverage

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa dados de treinamento acumulados para um usuário em simulação de ataque e treinamento.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|attackSimulationUser|[attackSimulationUser](../resources/attacksimulationuser.md)|Usuário em uma campanha de treinamento e simulação de ataque.|
|userTrainings|[Coleção userTrainingStatusInfo](../resources/usertrainingstatusinfo.md)|Lista de treinamentos atribuídos e seus status para o usuário.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attackSimulationTrainingUserCoverage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attackSimulationTrainingUserCoverage",
  "userTrainings": [
    {
      "@odata.type": "microsoft.graph.userTrainingStatusInfo"
    }
  ],
  "attackSimulationUser": {
    "@odata.type": "microsoft.graph.attackSimulationUser"
  }
}
```

