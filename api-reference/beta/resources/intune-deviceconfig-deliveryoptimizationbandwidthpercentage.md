---
title: tipo de recurso deliveryOptimizationBandwidthPercentage
description: Limites de largura de banda especificados como uma porcentagem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 85053c5e02b9ac429a3251c1c302c786f6a8f6db
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526794"
---
# <a name="deliveryoptimizationbandwidthpercentage-resource-type"></a>tipo de recurso deliveryOptimizationBandwidthPercentage

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Limites de largura de banda especificados como uma porcentagem.


Herda de [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|maximumBackgroundBandwidthPercentage|Int32|Especifica a largura de banda de download máximo que a otimização de entrega usa em todas as atividades de download simultâneas como uma porcentagem de largura de banda de download disponível (0-100). Valores válidos de 0 a 100
O valor padrão 0 (zero) significa que a otimização de entrega é ajustada dinamicamente para usar a largura de banda disponível para downloads em segundo plano. Valores válidos de 0 a 100|
|maximumForegroundBandwidthPercentage|Int32|Especifica a largura de banda máxima de download de primeiro plano que a otimização de entrega usa em todas as atividades de download simultâneos como uma porcentagem de largura de banda de download disponível (0-100). Valores válidos de 0 a 100
O valor padrão 0 (zero) significa que a otimização de entrega é ajustada dinamicamente para usar a largura de banda disponível para downloads de primeiro plano. Valores válidos de 0 a 100|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthPercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthPercentage",
  "maximumBackgroundBandwidthPercentage": 1024,
  "maximumForegroundBandwidthPercentage": 1024
}
```



