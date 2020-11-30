---
title: tipo de recurso cloudPcOnPremisesConnectionHealthCheck
description: O resultado de uma verificação de integridade de conexão local do PC de nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 188d9db2dbef3b3e731e0c95a48f6637e3e00101
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378224"
---
# <a name="cloudpconpremisesconnectionhealthcheck-resource-type"></a>tipo de recurso cloudPcOnPremisesConnectionHealthCheck

Namespace: microsoft.graph

O resultado de uma verificação de integridade de conexão local do PC de nuvem.

## <a name="methods"></a>Methods

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
|recomendado|Cadeia de Caracteres|A ação recomendada para corrigir o erro correspondente.|
|additionalDetails|Cadeia de Caracteres|Detalhes adicionais sobre a verificação de integridade ou a ação recomendada.|

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
