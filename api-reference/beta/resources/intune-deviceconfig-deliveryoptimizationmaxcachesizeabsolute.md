---
title: tipo de recurso deliveryOptimizationMaxCacheSizeAbsolute
description: Tipo absoluto de tamanho máximo de cache da otimização de entrega.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a955197e1e75ecb1f953f5ddc50b33b7e01a574b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565874"
---
# <a name="deliveryoptimizationmaxcachesizeabsolute-resource-type"></a>tipo de recurso deliveryOptimizationMaxCacheSizeAbsolute

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo absoluto de tamanho máximo de cache da otimização de entrega.


Herda de [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|maximumCacheSizeInGigabytes|Int64|Especifica o tamanho máximo em GB de cache de otimização de entrega. Valores válidos de 0 a 4294967295
O valor 0 (zero) significa cache "ilimitado". A otimização de entrega limpará o cache quando o dispositivo estiver com pouco espaço em disco. Valores válidos de 0 a 4294967295|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSizeAbsolute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationMaxCacheSizeAbsolute",
  "maximumCacheSizeInGigabytes": 1024
}
```





