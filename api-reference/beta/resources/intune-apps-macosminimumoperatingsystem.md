---
title: tipo de recurso macOSMinimumOperatingSystem
description: O sistema operacional mínimo necessário para um aplicativo do MacOS.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b329947398d034d8b50922f278f0b55314ec0c9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552237"
---
# <a name="macosminimumoperatingsystem-resource-type"></a>tipo de recurso macOSMinimumOperatingSystem

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O sistema operacional mínimo necessário para um aplicativo do MacOS.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|v10_7|Booliano|Mac OS 10,7 ou posterior.|
|v10_8|Booliano|Mac OS 10,8 ou posterior.|
|v10_9|Booliano|Mac OS 10,9 ou posterior.|
|v10_10|Booliano|Mac OS 10,10 ou posterior.|
|v10_11|Booliano|Mac OS 10,11 ou posterior.|
|v10_12|Booliano|Mac OS 10,12 ou posterior.|
|v10_13|Booliano|Mac OS 10,13 ou posterior.|

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





