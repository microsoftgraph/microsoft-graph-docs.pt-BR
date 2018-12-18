---
title: tipo de recurso de macOSMinimumOperatingSystem
description: O sistema operacional mínimo necessário para um aplicativo MacOS.
author: tfitzmac
ms.openlocfilehash: ff9d4e3fc375f17d7b3c3efdd4af16cd7e87ceb6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354772"
---
# <a name="macosminimumoperatingsystem-resource-type"></a>tipo de recurso de macOSMinimumOperatingSystem

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

O sistema operacional mínimo necessário para um aplicativo MacOS.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|v10_7|Boolean|Mac OS 10.7 ou posteriores.|
|v10_8|Boolean|Mac OS 10,8 ou posteriores.|
|v10_9|Boolean|Mac OS 10,9 ou posteriores.|
|v10_10|Boolean|Mac OS 10.10 ou posteriores.|
|v10_11|Boolean|Mac OS 10.11 ou posteriores.|
|v10_12|Boolean|Mac OS 10.12 ou posteriores.|
|v10_13|Boolean|Mac OS 10.13 ou posteriores.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSMinimumOperatingSystem",
  "v10_7": true,
  "v10_8": true,
  "v10_9": true,
  "v10_10": true,
  "v10_11": true,
  "v10_12": true,
  "v10_13": true
}
```





