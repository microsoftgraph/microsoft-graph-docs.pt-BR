---
title: tipo de recurso attackSimulationSimulationUserCoverage
description: Representa a cobertura de simulação para um usuário em treinamento e simulação de ataque.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 9caef11c29dbe003047d1013340c1fdae193d0d6
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979462"
---
# <a name="attacksimulationsimulationusercoverage-resource-type"></a>tipo de recurso attackSimulationSimulationUserCoverage

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa dados e resultados de simulação cumulativa para um usuário em treinamento e simulação de ataque.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|attackSimulationUser|[attackSimulationUser](../resources/attacksimulationuser.md)|Usuário em uma campanha de treinamento e simulação de ataque.|
|clickCount|Int32|Número de cliques de link nas cargas recebidas pelo usuário em campanhas de simulação e treinamento de ataques.|
|compromisedCount|Int32|Número de ações comprometedoras pelo usuário em campanhas de simulação e treinamento de ataques.|
|latestSimulationDateTime|DateTimeOffset|Data e hora da campanha de treinamento e simulação de ataque mais recente em que o usuário foi incluído.|
|simulationCount|Int32|Número de campanhas de simulação de ataque e treinamento em que o usuário foi incluído.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attackSimulationSimulationUserCoverage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attackSimulationSimulationUserCoverage",
  "simulationCount": "Integer",
  "latestSimulationDateTime": "String (timestamp)",
  "clickCount": "Integer",
  "compromisedCount": "Integer",
  "attackSimulationUser": {
    "@odata.type": "microsoft.graph.attackSimulationUser"
  }
}
```

