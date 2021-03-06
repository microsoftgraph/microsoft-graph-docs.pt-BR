---
title: tipo de recurso deviceProtectionOverview
description: Informações de hardware de um determinado dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f3b339f468f2fe1b67f5603ec67a16643ced53bb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267464"
---
# <a name="deviceprotectionoverview-resource-type"></a>tipo de recurso deviceProtectionOverview

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Informações de hardware de um determinado dispositivo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|totalReportedDeviceCount|Int32|Contagem total de dispositivos.|
|inactiveThreatAgentDeviceCount|Int32|Dispositivo com contagem inativa de agente de ameaça|
|unknownStateThreatAgentDeviceCount|Int32|Dispositivo com o estado do agente de ameaça como contagem desconhecida.|
|pendingSignatureUpdateDeviceCount|Int32|Dispositivo com a contagem de assinatura antiga.|
|cleanDeviceCount|Int32|Limpar contagem de dispositivos.|
|pendingFullScanDeviceCount|Int32|Contagem de dispositivos de verificação completa pendente.|
|pendingRestartDeviceCount|Int32|Contagem de dispositivos de reinicialização pendente.|
|pendingManualStepsDeviceCount|Int32|Contagem de dispositivos de etapas manuais pendentes.|
|pendingOfflineScanDeviceCount|Int32|Contagem de dispositivos de verificação offline pendente.|
|criticalFailuresDeviceCount|Int32|Contagem de dispositivos de falhas críticas.|
|pendingQuickScanDeviceCount|Int32|Contagem de dispositivos de verificação rápida pendente. Valores válidos-2147483648 a 2147483647|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceProtectionOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceProtectionOverview",
  "totalReportedDeviceCount": 1024,
  "inactiveThreatAgentDeviceCount": 1024,
  "unknownStateThreatAgentDeviceCount": 1024,
  "pendingSignatureUpdateDeviceCount": 1024,
  "cleanDeviceCount": 1024,
  "pendingFullScanDeviceCount": 1024,
  "pendingRestartDeviceCount": 1024,
  "pendingManualStepsDeviceCount": 1024,
  "pendingOfflineScanDeviceCount": 1024,
  "criticalFailuresDeviceCount": 1024,
  "pendingQuickScanDeviceCount": 1024
}
```




