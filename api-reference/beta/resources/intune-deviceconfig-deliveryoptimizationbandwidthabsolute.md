---
title: tipo de recurso deliveryOptimizationBandwidthAbsolute
description: Limites de largura de banda em quilobytes por segundo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8df502e294979ea81d26858f64cd386b83057f99
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973796"
---
# <a name="deliveryoptimizationbandwidthabsolute-resource-type"></a>tipo de recurso deliveryOptimizationBandwidthAbsolute

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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






