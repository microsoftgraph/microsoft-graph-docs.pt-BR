---
title: tipo de recurso de windowsProtectionState
description: Entidade de status de proteção do dispositivo.
author: tfitzmac
ms.openlocfilehash: 636b969ddafde5976939df764ae1180e19a181c0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328074"
---
# <a name="windowsprotectionstate-resource-type"></a>tipo de recurso de windowsProtectionState

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Entidade de status de proteção do dispositivo.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter windowsProtectionState](../api/intune-devices-windowsprotectionstate-get.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Leia as propriedades e os relacionamentos do objeto [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .|
|[Atualizar windowsProtectionState](../api/intune-devices-windowsprotectionstate-update.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Atualize as propriedades de um objeto [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo para o objeto de status de proteção do dispositivo. Este é o id do dispositivo do dispositivo|
|malwareProtectionEnabled|Boolean|Anti-malware está habilitado ou não|
|deviceState|[windowsDeviceHealthState](../resources/intune-devices-windowsdevicehealthstate.md)|Estado do computador (como limpar ou verificação completa ou pendentes reinicialização etc.). Os possíveis valores são: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.|
|realTimeProtectionEnabled|Boolean|Proteção em tempo real está habilitada ou não?|
|networkInspectionSystemEnabled|Boolean|Sistema de inspeção de rede habilitado ou não?|
|quickScanOverdue|Boolean|Verificação rápida vencidos ou não?|
|fullScanOverdue|Boolean|Completos exame vencido ou não?|
|signatureUpdateOverdue|Boolean|Assinatura desatualizada ou não?|
|rebootRequired|Boolean|Reinicialização necessária ou não?|
|fullScanRequired|Boolean|Verificação completa necessária ou não?|
|engineVersion|String|Versão do mecanismo de proteção de ponto de extremidade atual|
|signatureVersion|String|Versão atual de definições de malware|
|antiMalwareVersion|String|Atual anti-malware versão|
|lastQuickScanDateTime|DateTimeOffset|Última data/hora de verificação rápida|
|lastFullScanDateTime|DateTimeOffset|Última data/hora de verificação rápida|
|lastQuickScanSignatureVersion|String|Última versão de assinatura de verificação rápida|
|lastFullScanSignatureVersion|String|Última versão de assinatura de verificação completa|
|lastReportedDateTime|DateTimeOffset|Tempo de informado último status de integridade do dispositivo|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|detectedMalwareState|coleção [windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)|Lista de malware do dispositivo|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsProtectionState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "String (identifier)",
  "malwareProtectionEnabled": true,
  "deviceState": "String",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "String",
  "signatureVersion": "String",
  "antiMalwareVersion": "String",
  "lastQuickScanDateTime": "String (timestamp)",
  "lastFullScanDateTime": "String (timestamp)",
  "lastQuickScanSignatureVersion": "String",
  "lastFullScanSignatureVersion": "String",
  "lastReportedDateTime": "String (timestamp)"
}
```





