---
title: Tipo de recurso attackSimulationRoot
description: Fornece aos locatários a capacidade de iniciar ataques de phishing realistas e aprender com ele.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 56c0f8f8ce514e21b39e24494132ee6fec123d31
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979493"
---
# <a name="attacksimulationroot-resource-type"></a>Tipo de recurso attackSimulationRoot

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece aos locatários a capacidade de iniciar ataques de phishing realistas e aprender com ele.
Esse é um tipo abstrato.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar simulações](../api/attacksimulationroot-list-simulations.md)|[coleção simulation](../resources/simulation.md)|Obter os recursos de simulação da propriedade de navegação de simulações.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|simulações|[coleção simulation](../resources/simulation.md)|Represente a simulação de ataque e a campanha de treinamento de um locatário.|

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

