---
title: tipo de recurso de macOSMinimumOperatingSystem
description: O sistema operacional mínimo necessário para um aplicativo MacOS.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d1b5bb3c31f876cb7444ff90cad5060c08d2f60b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425922"
---
# <a name="macosminimumoperatingsystem-resource-type"></a>tipo de recurso de macOSMinimumOperatingSystem

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

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




