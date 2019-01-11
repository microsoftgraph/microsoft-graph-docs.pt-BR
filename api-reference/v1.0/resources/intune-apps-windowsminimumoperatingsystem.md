---
title: Tipo de recurso windowsMinimumOperatingSystem
description: O sistema operacional mínimo obrigatório para um aplicativo móvel do Windows.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d80a7c957b4a03132b349ebd609e21481322021a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863788"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a>Tipo de recurso windowsMinimumOperatingSystem

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

O sistema operacional mínimo obrigatório para um aplicativo móvel do Windows.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|v8_0|Booliano|Windows 8.0 ou posterior.|
|v8_1|Booliano|Windows 8.1 ou posterior.|
|v10_0|Booliano|Windows 10.0 ou posterior.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMinimumOperatingSystem",
  "v8_0": true,
  "v8_1": true,
  "v10_0": true
}
```



