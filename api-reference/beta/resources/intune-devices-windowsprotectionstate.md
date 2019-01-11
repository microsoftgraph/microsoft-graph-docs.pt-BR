---
title: tipo de recurso de windowsProtectionState
description: Entidade de status de proteção do dispositivo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5a21cc27039f3119836e0027b2558cadadab1b5d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884102"
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
|id|Cadeia de caracteres|O identificador exclusivo para o objeto de status de proteção do dispositivo. Este é o id do dispositivo do dispositivo|
|malwareProtectionEnabled|Booliano|Anti-malware está habilitado ou não|
|deviceState|[windowsDeviceHealthState](../resources/intune-devices-windowsdevicehealthstate.md)|Estado do computador (como limpar ou verificação completa ou pendentes reinicialização etc.). Os possíveis valores são: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.|
|realTimeProtectionEnabled|Booliano|Proteção em tempo real está habilitada ou não?|
|networkInspectionSystemEnabled|Booliano|Sistema de inspeção de rede habilitado ou não?|
|quickScanOverdue|Booliano|Verificação rápida vencidos ou não?|
|fullScanOverdue|Booliano|Completos exame vencido ou não?|
|signatureUpdateOverdue|Booliano|Assinatura desatualizada ou não?|
|rebootRequired|Booliano|Reinicialização necessária ou não?|
|fullScanRequired|Booliano|Verificação completa necessária ou não?|
|engineVersion|Cadeia de caracteres|Versão do mecanismo de proteção de ponto de extremidade atual|
|signatureVersion|Cadeia de caracteres|Versão atual de definições de malware|
|antiMalwareVersion|Cadeia de caracteres|Atual anti-malware versão|
|lastQuickScanDateTime|DateTimeOffset|Última data/hora de verificação rápida|
|lastFullScanDateTime|DateTimeOffset|Última data/hora de verificação rápida|
|lastQuickScanSignatureVersion|Cadeia de caracteres|Última versão de assinatura de verificação rápida|
|lastFullScanSignatureVersion|Cadeia de caracteres|Última versão de assinatura de verificação completa|
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





