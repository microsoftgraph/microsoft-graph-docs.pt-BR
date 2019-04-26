---
title: Tipo de recurso androidMinimumOperatingSystem
description: Contém propriedades para o sistema operacional mínimo obrigatório para um aplicativo móvel Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f2402ad007b794e7d6824e52cce8ff7144c6c33b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32560869"
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



