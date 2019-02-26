---
title: tipo de recurso deliveryOptimizationBandwidthHoursWithPercentage
description: Limite de largura de banda como uma porcentagem com horário comercial.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fb4fa251e9f1cb936da0ada158050df42e0aab6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30178238"
---
# <a name="deliveryoptimizationbandwidthhourswithpercentage-resource-type"></a>tipo de recurso deliveryOptimizationBandwidthHoursWithPercentage

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Limite de largura de banda como uma porcentagem com horário comercial.


Herda de [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|bandwidthBackgroundPercentageHours|[deliveryOptimizationBandwidthBusinessHoursLimit](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|Porcentagem de tempo de download em segundo plano.|
|bandwidthForegroundPercentageHours|[deliveryOptimizationBandwidthBusinessHoursLimit](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|Porcentagem de tempo de download do primeiro plano.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthHoursWithPercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthHoursWithPercentage",
  "bandwidthBackgroundPercentageHours": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
    "bandwidthBeginBusinessHours": 1024,
    "bandwidthEndBusinessHours": 1024,
    "bandwidthPercentageDuringBusinessHours": 1024,
    "bandwidthPercentageOutsideBusinessHours": 1024
  },
  "bandwidthForegroundPercentageHours": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
    "bandwidthBeginBusinessHours": 1024,
    "bandwidthEndBusinessHours": 1024,
    "bandwidthPercentageDuringBusinessHours": 1024,
    "bandwidthPercentageOutsideBusinessHours": 1024
  }
}
```




