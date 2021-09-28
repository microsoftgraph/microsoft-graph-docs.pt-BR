---
title: Tipo de recurso attackSimulationRepeatOffender
description: Representa o usuário infrator repetido em simulação de ataque e treinamento.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: a78d474514a4975584425c18da71451dc0352e25
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979451"
---
# <a name="attacksimulationrepeatoffender-resource-type"></a>Tipo de recurso attackSimulationRepeatOffender

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um usuário em um locatário que deu lugar a ataques mais de uma vez em várias campanhas de simulação e treinamento de ataques.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|attackSimulationUser|[attackSimulationUser](../resources/attacksimulationuser.md)|Usuário em uma campanha de treinamento e simulação de ataque.|
|repeatOffenceCount|Int32|Número de ofensas repetidas do usuário em campanhas de simulação e treinamento de ataques.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attackSimulationRepeatOffender"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attackSimulationRepeatOffender",
  "repeatOffenceCount": "Integer",
  "attackSimulationUser": {
    "@odata.type": "microsoft.graph.attackSimulationUser"
  }
}
```

