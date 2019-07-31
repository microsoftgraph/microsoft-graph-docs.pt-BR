---
title: tipo de recurso deliveryOptimizationBandwidthBusinessHoursLimit
description: Tipo de tempo de largura de banda e tipos de porcentagem
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cbd94f135ae893e5e30ab2256ade2574efb771a7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970812"
---
# <a name="deliveryoptimizationbandwidthbusinesshourslimit-resource-type"></a>tipo de recurso deliveryOptimizationBandwidthBusinessHoursLimit

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo de tempo de largura de banda e tipos de porcentagem

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|bandwidthBeginBusinessHours|Int32|Especifica o início do horário comercial usando um relógio de 24 horas (0-23). Valores válidos de 0 a 23|
|bandwidthEndBusinessHours|Int32|Especifica o fim do horário comercial usando um relógio de 24 horas (0-23). Valores válidos de 0 a 23|
|bandwidthPercentageDuringBusinessHours|Int32|Especifica a porcentagem de largura de banda a ser limite durante o horário comercial (0-100). Valores válidos de 0 a 100|
|bandwidthPercentageOutsideBusinessHours|Int32|Especifica a porcentagem de largura de banda para limitar o horário comercial de outsids (0-100). Valores válidos de 0 a 100|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
  "bandwidthBeginBusinessHours": 1024,
  "bandwidthEndBusinessHours": 1024,
  "bandwidthPercentageDuringBusinessHours": 1024,
  "bandwidthPercentageOutsideBusinessHours": 1024
}
```





