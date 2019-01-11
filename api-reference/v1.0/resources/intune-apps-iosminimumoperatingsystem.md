---
title: Tipo de recurso iosMinimumOperatingSystem
description: Contém as propriedades do sistema operacional mínimo obrigatório para um aplicativo móvel iOS.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7243b337a53cca31054f99ae807e5c17cdd3e372
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876263"
---
# <a name="iosminimumoperatingsystem-resource-type"></a>Tipo de recurso iosMinimumOperatingSystem

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém as propriedades do sistema operacional mínimo obrigatório para um aplicativo móvel iOS.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|v8_0|Booliano|Versão 8.0 ou posterior.|
|v9_0|Booliano|Versão 9.0 ou posterior.|
|v10_0|Booliano|Versão 10.0 ou posterior.|
|v11_0|Booliano|Versão 11.0 ou posterior.|
|v12_0|Booliano|Versão 12.0 ou posterior.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMinimumOperatingSystem",
  "v8_0": true,
  "v9_0": true,
  "v10_0": true,
  "v11_0": true,
  "v12_0": true
}
```



