---
title: tipo de recurso deliveryOptimizationMaxCacheSizeAbsolute
description: Tipo absoluto de tamanho máximo de cache da otimização de entrega.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dfb158b30c8c2d75a58ddcbab190eaa37e9153bd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294715"
---
# <a name="deliveryoptimizationmaxcachesizeabsolute-resource-type"></a>tipo de recurso deliveryOptimizationMaxCacheSizeAbsolute

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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




