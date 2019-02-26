---
title: tipo de recurso deliveryOptimizationMaxCacheSizePercentage
description: Tipos de percentual máximo de otimização de entrega.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7579b95d0adefb09c9312596f4604fe9d5b05548
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177830"
---
# <a name="deliveryoptimizationmaxcachesizepercentage-resource-type"></a>tipo de recurso deliveryOptimizationMaxCacheSizePercentage

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipos de percentual máximo de otimização de entrega.


Herda de [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|maximumCacheSizePercentage|Int32|Especifica o tamanho máximo de cache que a otimização de entrega pode utilizar, como um percentual do tamanho do disco (1-100). Valores válidos de 1 a 100|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSizePercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationMaxCacheSizePercentage",
  "maximumCacheSizePercentage": 1024
}
```




