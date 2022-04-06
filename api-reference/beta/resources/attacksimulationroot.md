---
title: Tipo de recurso attackSimulationRoot
description: Fornece a capacidade de iniciar um ataque de phishing realista que as organizações podem aprender.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: b83d13c6541b036bf3096f6ba6e99a9f4dfb79f5
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757651"
---
# <a name="attacksimulationroot-resource-type"></a>Tipo de recurso attackSimulationRoot

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece a capacidade de iniciar um ataque de phishing realista que as organizações podem aprender.
Esse é um tipo abstrato.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar simulações](../api/attacksimulationroot-list-simulations.md)|[coleção simulation](../resources/simulation.md)|Obter uma lista de campanhas de treinamento de simulação de ataque para um locatário.|
|[Listar simulationAutomations](../api/attacksimulationroot-list-simulationautomations.md)|[Coleção simulationAutomation](../resources/simulationautomation.md)|Obter uma lista de automações de simulação de ataque para um locatário.|

## <a name="properties"></a>Propriedades
Nenhum.

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|simulações|[coleção simulation](../resources/simulation.md)|Representa uma campanha de treinamento de simulação de ataque em um locatário.|
|simulationAutomations|[Coleção simulationAutomation](../resources/simulationautomation.md)|Representa automações de simulação criadas para executar em um locatário.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attackSimulationRoot",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attackSimulationRoot"
}
```

