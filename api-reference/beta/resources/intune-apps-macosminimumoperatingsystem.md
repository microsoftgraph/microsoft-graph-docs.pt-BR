---
title: tipo de recurso macOSMinimumOperatingSystem
description: O sistema operacional mínimo necessário para um aplicativo do MacOS.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f6975690361c981d6b5aaf1d9dae959ad6f8be5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169934"
---
# <a name="macosminimumoperatingsystem-resource-type"></a>tipo de recurso macOSMinimumOperatingSystem

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O sistema operacional mínimo necessário para um aplicativo do MacOS.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|v10_7|Boolean|Mac OS 10,7 ou posterior.|
|v10_8|Boolean|Mac OS 10,8 ou posterior.|
|v10_9|Boolean|Mac OS 10,9 ou posterior.|
|v10_10|Boolean|Mac OS 10,10 ou posterior.|
|v10_11|Boolean|Mac OS 10,11 ou posterior.|
|v10_12|Boolean|Mac OS 10,12 ou posterior.|
|v10_13|Boolean|Mac OS 10,13 ou posterior.|

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




