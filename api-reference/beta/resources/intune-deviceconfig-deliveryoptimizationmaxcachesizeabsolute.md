---
title: tipo de recurso deliveryOptimizationMaxCacheSizeAbsolute
description: Tipo absoluto de tamanho absoluto de tamanho máximo de cache de Otimização de Entrega.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 37eab02840f088cc77744388e8a1c7f07b0e92dd
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58771236"
---
# <a name="deliveryoptimizationmaxcachesizeabsolute-resource-type"></a>tipo de recurso deliveryOptimizationMaxCacheSizeAbsolute

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo absoluto de tamanho absoluto de tamanho máximo de cache de Otimização de Entrega.


Herda de [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|maximumCacheSizeInGigabytes|Int64|Especifica o tamanho máximo em GB de cache de Otimização de Entrega. Valores válidos de 0 a 4294967295
O valor 0 (zero) significa cache "unlimited". A Otimização de Entrega limpará o cache quando o dispositivo estiver com pouco espaço em disco. Valores válidos de 0 a 4294967295|

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



