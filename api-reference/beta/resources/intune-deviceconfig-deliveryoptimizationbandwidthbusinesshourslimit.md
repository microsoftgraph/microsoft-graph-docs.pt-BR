---
title: tipo de recurso deliveryOptimizationBandwidthBusinessHoursLimit
description: Tipo de horários comerciais e porcentagens de largura de banda
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b3b6fdc86eed3043e3f95bd2947bc24dc35d5761
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58797539"
---
# <a name="deliveryoptimizationbandwidthbusinesshourslimit-resource-type"></a>tipo de recurso deliveryOptimizationBandwidthBusinessHoursLimit

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo de horários comerciais e porcentagens de largura de banda

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|bandwidthBeginBusinessHours|Int32|Especifica o início do horário comercial usando um relógio de 24 horas (0-23). Valores válidos de 0 a 23|
|bandwidthEndBusinessHours|Int32|Especifica o fim do horário comercial usando um relógio de 24 horas (0-23). Valores válidos de 0 a 23|
|bandwidthPercentageDuringBusinessHours|Int32|Especifica a porcentagem de largura de banda a ser limitada durante o horário comercial (0-100). Valores válidos de 0 a 100|
|bandwidthPercentageOutsideBusinessHours|Int32|Especifica a porcentagem de largura de banda para limitar o horário comercial de outsidse (0-100). Valores válidos de 0 a 100|

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



