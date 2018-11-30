---
title: tipo de recurso de deviceProtectionOverview
description: Informações de hardware de um determinado dispositivo.
ms.openlocfilehash: 81252fdf60c1de129a615b075968e0e6f1eca943
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038480"
---
# <a name="deviceprotectionoverview-resource-type"></a>tipo de recurso de deviceProtectionOverview

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

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





