---
title: Tipo de recurso androidMinimumOperatingSystem
description: Contém propriedades para o sistema operacional mínimo obrigatório para um aplicativo móvel Android.
author: tfitzmac
ms.openlocfilehash: 3c477a624377febe6001b92f6694fe27b0666cf5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350467"
---
# <a name="androidminimumoperatingsystem-resource-type"></a>Tipo de recurso androidMinimumOperatingSystem

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

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



