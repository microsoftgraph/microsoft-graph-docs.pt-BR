---
title: Tipo de recurso cloudPcOnPremisesConnectionStatusDetails
description: Os detalhes de status de uma conexão local do computador na nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 7ef9847190fb851482d29535d0709f3d74bbf3aa
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722171"
---
# <a name="cloudpconpremisesconnectionstatusdetails-resource-type"></a>Tipo de recurso cloudPcOnPremisesConnectionStatusDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os detalhes de status de [um cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|startDateTime|DateTimeOffset|A hora de início da verificação de saúde da conexão. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|endDateTime|DateTimeOffset|A hora de término da verificação de saúde da conexão. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|healthChecks|[coleção cloudPcOnPremisesConnectionHealthCheck](../resources/cloudpconpremisesconnectionhealthcheck.md)|Todas as verificações feitas na conexão.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionStatusDetails"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnectionStatusDetails",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "healthChecks": [
    {
      "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
      "displayName": "String",
      "status": "String",
      "startDateTime": "String (timestamp)",
      "endDateTime": "String (timestamp)",
      "errorType": "String",
      "recommendedAction": "String",
      "additionalDetails": "String"
    }
  ]
}
```
