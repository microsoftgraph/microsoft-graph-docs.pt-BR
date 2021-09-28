---
title: Tipo de recurso simulationEventsContent
description: Representa eventos de simulação em uma campanha de simulação e treinamento de ataque.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 0a35ce8a743a358ab319388dc9aa25fe88e32dec
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979465"
---
# <a name="simulationeventscontent-resource-type"></a>Tipo de recurso simulationEventsContent

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa eventos de simulação em uma campanha de simulação e treinamento de ataque.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|compromisedRate|Duplo|Porcentagem real de usuários que cairam no ataque simulado em uma campanha de simulação e treinamento de ataque.|
|events|[Coleção simulationEvent](../resources/simulationevent.md)|Lista de eventos de simulação em uma campanha de simulação e treinamento de ataque.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.simulationEventsContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.simulationEventsContent",
  "compromisedRate": "Double",
  "events": [
    {
      "@odata.type": "microsoft.graph.simulationEvent"
    }
  ]
}
```

