---
title: tipo de recurso cloudPcOnPremisesConnectionStatusDetails
description: Os detalhes de status de uma conexão local do PC de nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: db40df3bcd89ac21eb50870e82fe6a34ced86828
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563769"
---
# <a name="cloudpconpremisesconnectionstatusdetails-resource-type"></a>tipo de recurso cloudPcOnPremisesConnectionStatusDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os detalhes de status de um [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|startDateTime|DateTimeOffset|A hora de início da verificação de integridade da conexão. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.|
|endDateTime|DateTimeOffset|A hora de término da verificação de integridade da conexão. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.|
|healthChecks|coleção [cloudPcOnPremisesConnectionHealthCheck](../resources/cloudpconpremisesconnectionhealthcheck.md)|Todas as verificações realizadas na conexão.|

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
