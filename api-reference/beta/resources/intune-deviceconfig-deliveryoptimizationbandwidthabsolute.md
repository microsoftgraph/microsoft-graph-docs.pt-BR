---
title: tipo de recurso deliveryOptimizationBandwidthAbsolute
description: Limites de largura de banda em quilobytes por segundo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9eca95ad33ced19e437e760663a73158aacc25d0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30178266"
---
# <a name="deliveryoptimizationbandwidthabsolute-resource-type"></a>tipo de recurso deliveryOptimizationBandwidthAbsolute

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Limites de largura de banda em quilobytes por segundo.


Herda de [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|maximumDownloadBandwidthInKilobytesPerSecond|Int64|Especifica a largura de banda máxima de download em quilobytes/segundo que o dispositivo pode usar em todas as atividades de download simultâneos usando a otimização de entrega. Valores válidos de 0 a 4294967295
O valor 0 (zero) significa que a otimização de entrega é ajustada dinamicamente para usar a largura de banda disponível para downloads. Valores válidos de 0 a 4294967295|
|maximumUploadBandwidthInKilobytesPerSecond|Int64|Especifica a largura de banda de upload máxima em KiloBytes/segundo que um dispositivo usará em toda a atividade de upload simultâneo usando a otimização de entrega (0-4000000). Valores válidos de 0 a 4 milhões
O valor padrão é 0, que permite uma largura de banda possivelmente ilimitada (otimizada para uso mínimo da largura de banda de upload). Valores válidos de 0 a 4 milhões|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthAbsolute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthAbsolute",
  "maximumDownloadBandwidthInKilobytesPerSecond": 1024,
  "maximumUploadBandwidthInKilobytesPerSecond": 1024
}
```




