---
title: Tipo de recurso simulationEvent
description: Representa o evento de simulação em uma campanha de simulação e treinamento de ataque.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 5d0abb9606b549fb1349b1e98545dcf0f25e4fb7
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979463"
---
# <a name="simulationevent-resource-type"></a>Tipo de recurso simulationEvent

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o evento de simulação em uma campanha de simulação e treinamento de ataque.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Count|Int32|Contagem da ocorrência do evento de simulação em uma campanha de simulação e treinamento de ataque.|
|eventName|Cadeia de caracteres|Nome do evento de simulação em uma campanha de simulação e treinamento de ataque.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.simulationEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.simulationEvent",
  "eventName": "String",
  "count": "Integer"
}
```

