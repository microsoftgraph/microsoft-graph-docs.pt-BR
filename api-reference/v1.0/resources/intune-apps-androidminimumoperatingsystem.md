---
title: Tipo de recurso androidMinimumOperatingSystem
description: Contém propriedades para o sistema operacional mínimo obrigatório para um aplicativo móvel Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 100a6923ab64a8a2d8629ccd6aace36db9263fdd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032365"
---
# <a name="androidminimumoperatingsystem-resource-type"></a>Tipo de recurso androidMinimumOperatingSystem

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o sistema operacional mínimo obrigatório para um aplicativo móvel Android.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|v4_0|Booliano|Versão 4.0 ou posterior.|
|v4_0_3|Booliano|Versão 4.0.3 ou posterior.|
|v4_1|Booliano|Versão 4.1 ou posterior.|
|v4_2|Booliano|Versão 4.2 ou posterior.|
|v4_3|Booliano|Versão 4.3 ou posterior.|
|v4_4|Booliano|Versão 4.4 ou posterior.|
|v5_0|Booliano|Versão 5.0 ou posterior.|
|v5_1|Booliano|Versão 5.1 ou posterior.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMinimumOperatingSystem",
  "v4_0": true,
  "v4_0_3": true,
  "v4_1": true,
  "v4_2": true,
  "v4_3": true,
  "v4_4": true,
  "v5_0": true,
  "v5_1": true
}
```



