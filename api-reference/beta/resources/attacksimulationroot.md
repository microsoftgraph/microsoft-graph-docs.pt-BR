---
title: Tipo de recurso attackSimulationRoot
description: Fornece aos locatários a capacidade de iniciar ataques de phishing realistas e aprender com ele.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: e38107d7c6d95706508ea5260fa9e88c87774672
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519737"
---
# <a name="attacksimulationroot-resource-type"></a>Tipo de recurso attackSimulationRoot

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece aos locatários a capacidade de iniciar ataques de phishing realistas e aprender com ele.
Esse é um tipo abstrato.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar simulações](../api/attacksimulationroot-list-simulations.md)|[coleção simulation](../resources/simulation.md)|Obter os recursos de simulação da propriedade de navegação de simulações.|

## <a name="properties"></a>Propriedades
Nenhum.

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

