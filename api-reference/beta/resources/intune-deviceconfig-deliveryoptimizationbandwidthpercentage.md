---
title: tipo de recurso deliveryOptimizationBandwidthPercentage
description: Limites de largura de banda especificados como porcentagem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8f1aab20ff6bbb7ab4e353e6d82fd2b19dd62281
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58820454"
---
# <a name="deliveryoptimizationbandwidthpercentage-resource-type"></a>tipo de recurso deliveryOptimizationBandwidthPercentage

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Limites de largura de banda especificados como porcentagem.


Herda de [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|maximumBackgroundBandwidthPercentage|Int32|Especifica a largura de banda máxima de download em segundo plano que a Otimização de Entrega usa em todas as atividades de download simultâneas como uma porcentagem da largura de banda de download disponível (0-100). Valores válidos de 0 a 100
O valor padrão 0 (zero) significa que a Otimização de Entrega ajusta dinamicamente o uso da largura de banda disponível para downloads em segundo plano. Valores válidos de 0 a 100|
|maximumForegroundBandwidthPercentage|Int32|Especifica a largura de banda máxima de download em primeiro plano que a Otimização de Entrega usa em todas as atividades de download simultâneas como uma porcentagem da largura de banda de download disponível (0-100). Valores válidos de 0 a 100
O valor padrão 0 (zero) significa que a Otimização de Entrega ajusta dinamicamente o uso da largura de banda disponível para downloads em primeiro plano. Valores válidos de 0 a 100|

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



