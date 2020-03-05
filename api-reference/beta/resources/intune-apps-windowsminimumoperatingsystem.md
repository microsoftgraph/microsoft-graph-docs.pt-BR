---
title: Tipo de recurso windowsMinimumOperatingSystem
description: O sistema operacional mínimo obrigatório para um aplicativo móvel do Windows.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ca5eebaad444cadbc494ea978d900a40f596b556
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42489955"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a>Tipo de recurso windowsMinimumOperatingSystem

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O sistema operacional mínimo obrigatório para um aplicativo móvel do Windows.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|v8_0|Boolean|Windows 8.0 ou posterior.|
|v8_1|Booliano|Windows 8.1 ou posterior.|
|v10_0|Booliano|Windows 10.0 ou posterior.|
|v10_1607|Boolean|Windows 10 1607 ou posterior.|
|v10_1703|Boolean|Windows 10 1703 ou posterior.|
|v10_1709|Boolean|Windows 10 1709 ou posterior.|
|v10_1803|Boolean|Windows 10 1803 ou posterior.|
|v10_1809|Boolean|Windows 10 1809 ou posterior.|
|v10_1903|Boolean|Windows 10 1903 ou posterior.|

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
  "v10_0": true,
  "v10_1607": true,
  "v10_1703": true,
  "v10_1709": true,
  "v10_1803": true,
  "v10_1809": true,
  "v10_1903": true
}
```



