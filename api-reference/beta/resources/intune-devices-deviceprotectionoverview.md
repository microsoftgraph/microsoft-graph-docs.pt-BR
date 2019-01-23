---
title: tipo de recurso de deviceProtectionOverview
description: Informações de hardware de um determinado dispositivo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 902e3a6062d2aa50c96c27eb9d542905bf9a029d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418985"
---
# <a name="deviceprotectionoverview-resource-type"></a>tipo de recurso de deviceProtectionOverview

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Informações de hardware de um determinado dispositivo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|totalReportedDeviceCount|Int32|Contagem total de dispositivo.|
|inactiveThreatAgentDeviceCount|Int32|Dispositivo com contagem de agente de ameaça inativa|
|unknownStateThreatAgentDeviceCount|Int32|Dispositivo com o estado de agente de ameaça como contagem desconhecido.|
|pendingSignatureUpdateDeviceCount|Int32|Dispositivo com a contagem de assinatura antigo.|
|cleanDeviceCount|Int32|Limpar a contagem do dispositivo.|
|pendingFullScanDeviceCount|Int32|Contagem de dispositivo pendentes verificação completa.|
|pendingRestartDeviceCount|Int32|Contagem de reinicialização pendente do dispositivo.|
|pendingManualStepsDeviceCount|Int32|Contagem de dispositivo pendentes etapas manuais.|
|pendingOfflineScanDeviceCount|Int32|Contagem de dispositivo pendentes verificação offline.|
|criticalFailuresDeviceCount|Int32|Contagem de falhas críticas do dispositivo.|

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
  "criticalFailuresDeviceCount": 1024
}
```




