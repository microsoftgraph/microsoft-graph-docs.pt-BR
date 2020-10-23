---
title: tipo de recurso deliveryOptimizationMaxCacheSizePercentage
description: Tipos de percentual máximo de otimização de entrega.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 02b522ccfac58a6c4ff9f9780512e83abf2cdec8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692545"
---
# <a name="deliveryoptimizationmaxcachesizepercentage-resource-type"></a>tipo de recurso deliveryOptimizationMaxCacheSizePercentage

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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





