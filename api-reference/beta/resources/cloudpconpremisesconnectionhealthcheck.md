---
title: Tipo de recurso cloudPcOnPremisesConnectionHealthCheck
description: O resultado de uma verificação de saúde de conexão local do computador na nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: e79f73bbe1a493e581a35db5fec396d752ff08d1
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844603"
---
# <a name="cloudpconpremisesconnectionhealthcheck-resource-type"></a>Tipo de recurso cloudPcOnPremisesConnectionHealthCheck

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O resultado de uma verificação de saúde de conexão local do computador na nuvem.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[RunHealthChecks of cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-runhealthcheck.md)|Nenhum|Execute as verificações de saúde de [uma cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição deste item de verificação de saúde.|
|status|cloudPcOnPremisesConnectionStatus|O status do item de verificação de saúde. Somente leitura. Os valores possíveis são: `Pending`, `Running`, `Passed`, `Failed`, `UnknownFutureValue`.|
|startDateTime|DateTimeOffset|A hora de início do item de verificação de saúde. Somente leitura.|
|endDateTime|DateTimeOffset|A hora de término do item de verificação de saúde. Somente leitura.|
|errorType|cloudPcOnPremisesConnectionHealthCheckErrorType|O tipo de erro que ocorreu durante a verificação de saúde. Os valores possíveis `DnsCheckFqdnNotFound` são: `DnsCheckUnknownError` , , , , `AdJoinCheckFqdnNotFound` , `AdJoinCheckIncorrectCredentials` `AdJoinCheckOrganizationalUnitNotFound` `AdJoinCheckOrganizationalUnitIncorrectFormat` `AdJoinCheckUnknownError` `EndpointConnectivityCheckUrlNotWhitelisted` , `EndpointConnectivityCheckUnknownError` `AadConnectivityCheckUnknownError` `ResourceAvailabilityCheckNoSubnetIP` `resourceAvailabilityCheckSubscriptionDisabled` `resourceAvailabilityCheckUnknownError` `permissionCheckNoSubscriptionReaderRole` `permissionCheckNoResourceGroupOwnerRole` `permissionCheckNoVNetContributorRole` `permissionCheckUnknownError` `internalServerUnknownError` .|
|recommendedAction|Cadeia de caracteres|A ação recomendada para corrigir o erro correspondente.|
|additionalDetails|Cadeia de caracteres|Detalhes adicionais sobre a verificação de saúde ou a ação recomendada.|

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
