---
title: Tipo de recurso simulationReport
description: Representa um relatório de uma campanha de simulação e treinamento de ataque.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 8f3e5991192d3d3f72e37e8ac5117a01d0138369
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979477"
---
# <a name="simulationreport-resource-type"></a>Tipo de recurso simulationReport

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um relatório de uma campanha de simulação e treinamento de ataque, incluindo uma visão geral e usuários da campanha.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|visão geral|[simulationReportOverview](../resources/simulationreportoverview.md)|Visão geral de uma campanha de treinamento e simulação de ataque.|
|simulationUsers|[Coleção userSimulationDetails](../resources/usersimulationdetails.md)|Representa os usuários de um locatário e suas ações online em uma campanha de simulação e treinamento de ataques.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.simulationReport"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.simulationReport",
  "overview": {
    "@odata.type": "microsoft.graph.simulationReportOverview"
  },
  "simulationUsers": [
    {
      "@odata.type": "microsoft.graph.userSimulationDetails"
    }
  ]
}
```

