---
title: tipo de recurso cloudPcOnPremisesConnectionHealthCheck
description: O resultado de uma verificação de integridade de conexão local do PC de nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 16dea9278c9471996e4a5beaf20d5f9ec5c2d5c5
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563831"
---
# <a name="cloudpconpremisesconnectionhealthcheck-resource-type"></a>tipo de recurso cloudPcOnPremisesConnectionHealthCheck

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O resultado de uma verificação de integridade de conexão local do PC de nuvem.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[RunHealthChecks do cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-runhealthcheck.md)|Nenhum|Execute as verificações de integridade de um [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome de exibição deste item de verificação de integridade.|
|status|cloudPcOnPremisesConnectionStatus|O status do item de verificação de integridade. Somente leitura. Os valores possíveis são: `Pending`, `Running`, `Passed`, `Failed`, `UnknownFutureValue`.|
|startDateTime|DateTimeOffset|A hora de início do item de verificação de integridade. Somente leitura.|
|endDateTime|DateTimeOffset|A hora de término do item de verificação de integridade. Somente leitura.|
|Error|cloudPcOnPremisesConnectionHealthCheckErrorType|O tipo de erro que ocorreu durante esta verificação de integridade. Os valores possíveis são: `DnsCheckFqdnNotFound`, `DnsCheckUnknownError`, `AdJoinCheckFqdnNotFound`, `AdJoinCheckIncorrectCredentials`, `AdJoinCheckOrganizationalUnitNotFound`, `AdJoinCheckOrganizationalUnitIncorrectFormat`, `AdJoinCheckUnknownError`, `EndpointConnectivityCheckUrlNotWhitelisted`, `EndpointConnectivityCheckUnknownError`, `AadConnectivityCheckUnknownError`.|
|recomendado|String|A ação recomendada para corrigir o erro correspondente.|
|additionalDetails|String|Detalhes adicionais sobre a verificação de integridade ou a ação recomendada.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
  "displayName": "String",
  "status": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "errorType": "String",
  "recommendedAction": "String",
  "additionalDetails": "String"
}
```
