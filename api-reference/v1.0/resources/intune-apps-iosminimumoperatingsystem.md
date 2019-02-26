---
title: Tipo de recurso iosMinimumOperatingSystem
description: Contém as propriedades do sistema operacional mínimo obrigatório para um aplicativo móvel iOS.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7490ad7b27d55fa6f2b7c6de12083025e7b4ac93
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254566"
---
# <a name="iosminimumoperatingsystem-resource-type"></a>Tipo de recurso iosMinimumOperatingSystem

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém as propriedades do sistema operacional mínimo obrigatório para um aplicativo móvel iOS.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|v8_0|Boolean|Versão 8.0 ou posterior.|
|v9_0|Boolean|Versão 9.0 ou posterior.|
|v10_0|Boolean|Versão 10.0 ou posterior.|
|v11_0|Booliano|Versão 11.0 ou posterior.|
|v12_0|Boolean|Versão 12,0 ou posterior.|

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



