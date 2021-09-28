---
title: Tipo de recurso userSimulationDetails
description: Representa um usuário de um locatário e suas ações online em uma campanha de simulação e treinamento de ataques.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 9ca7adee31eef9d197ac6ecba180be5fbaa7d697
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979478"
---
# <a name="usersimulationdetails-resource-type"></a>Tipo de recurso userSimulationDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um usuário de um locatário e as ações online do usuário em uma campanha de simulação e treinamento de ataques.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|assignedTrainingsCount|Int32|Número de treinamentos atribuídos a um usuário em uma campanha de simulação e treinamento de ataque.|
|completedTrainingsCount|Int32|Número de treinamentos concluídos por um usuário em uma campanha de simulação e treinamento de ataques.|
|compromisedDateTime|DateTimeOffset|Data e hora da ação comprometedora online por um usuário em uma campanha de simulação e treinamento de ataque.|
|inProgressTrainingsCount|Int32|Número de treinamentos em andamento por um usuário em uma campanha de simulação e treinamento de ataque.|
|isCompromised|Boleano|Sinalizador representando se o usuário foi comprometido em uma simulação de ataque e campanha de treinamento.|
|reportedPhishDateTime|DateTimeOffset|Data e hora em que o usuário relatou a entrega da carga como phishing na campanha de simulação e treinamento de ataque.|
|simulationEvents|[Coleção userSimulationEventInfo](../resources/usersimulationeventinfo.md)|Lista de eventos de simulação de um usuário na campanha de simulação e treinamento de ataque.|
|simulationUser|[attackSimulationUser](../resources/attacksimulationuser.md)|Usuário em uma campanha de treinamento e simulação de ataque.|
|trainingEvents|[Coleção userTrainingEventInfo](../resources/usertrainingeventinfo.md)|Lista de eventos de treinamento de um usuário na campanha de simulação e treinamento de ataque.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userSimulationDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userSimulationDetails",
  "isCompromised": "Boolean",
  "compromisedDateTime": "String (timestamp)",
  "simulationEvents": [
    {
      "@odata.type": "microsoft.graph.userSimulationEventInfo"
    }
  ],
  "trainingEvents": [
    {
      "@odata.type": "microsoft.graph.userTrainingEventInfo"
    }
  ],
  "assignedTrainingsCount": "Integer",
  "completedTrainingsCount": "Integer",
  "inProgressTrainingsCount": "Integer",
  "reportedPhishDateTime": "String (timestamp)",
  "simulationUser": {
    "@odata.type": "microsoft.graph.attackSimulationUser"
  }
}
```

