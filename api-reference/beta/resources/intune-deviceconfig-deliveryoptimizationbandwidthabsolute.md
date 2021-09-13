---
title: tipo de recurso deliveryOptimizationBandwidthAbsolute
description: Limites de largura de banda em quilobytes por segundo.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a8d625892c0d8651de284037d5a2ba4158a3b34a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147987"
---
# <a name="deliveryoptimizationbandwidthabsolute-resource-type"></a>tipo de recurso deliveryOptimizationBandwidthAbsolute

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Limites de largura de banda em quilobytes por segundo.


Herda de [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|maximumDownloadBandwidthInKilobytesPerSecond|Int64|Especifica a largura de banda máxima de download em KiloBytes/segundo que o dispositivo pode usar em todas as atividades de download simultâneas usando a Otimização de Entrega. Valores válidos de 0 a 4294967295
O valor 0 (zero) significa que a Otimização de Entrega ajusta dinamicamente o uso da largura de banda disponível para downloads. Valores válidos de 0 a 4294967295|
|maximumUploadBandwidthInKilobytesPerSecond|Int64|Especifica a largura de banda de carregamento máxima em KiloBytes/segundo que um dispositivo usará em todas as atividades de carregamento simultâneas usando a Otimização de Entrega (0-4000000). Valores válidos de 0 a 4000000
O valor padrão é 0, o que permite largura de banda ilimitada possível (otimizada para o uso mínimo da largura de banda de carregamento). Valores válidos de 0 a 4000000|

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



