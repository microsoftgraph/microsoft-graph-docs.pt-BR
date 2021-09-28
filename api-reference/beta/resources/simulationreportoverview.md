---
title: Tipo de recurso simulationReportOverview
description: Representa o relatório de visão geral de uma campanha de simulação e treinamento de ataque.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 5f096dbe931959707ad067ce3d11fcf0afac4bdb
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979502"
---
# <a name="simulationreportoverview-resource-type"></a>Tipo de recurso simulationReportOverview

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma visão geral de uma campanha de simulação e treinamento de ataque.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|recommendedActions|[Coleção recommendedAction](../resources/recommendedaction.md)|Lista de ações recomendadas para um locatário melhorar sua postura de segurança com base na simulação de ataque e no tipo de ataque de campanha de treinamento.|
|resolvedTargetsCount|Int32|Número de usuários válidos na campanha de simulação e treinamento de ataque.|
|simulationEventsContent|[simulationEventsContent](../resources/simulationeventscontent.md)|Resumo dos eventos de simulação na campanha de simulação e treinamento de ataque.|
|trainingEventsContent|[trainingEventsContent](../resources/trainingeventscontent.md)|Resumo dos treinamentos atribuídos na campanha de simulação e treinamento de ataque.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.simulationReportOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.simulationReportOverview",
  "resolvedTargetsCount": "Integer",
  "simulationEventsContent": {
    "@odata.type": "microsoft.graph.simulationEventsContent"
  },
  "trainingEventsContent": {
    "@odata.type": "microsoft.graph.trainingEventsContent"
  },
  "recommendedActions": [
    {
      "@odata.type": "microsoft.graph.recommendedAction"
    }
  ]
}
```

