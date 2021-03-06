---
title: tipo de recurso Windowsprotectionstate foi
description: Entidade de status de proteção de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b2651aa9fad173654d8fff554bdf89f7ab36da14
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49207558"
---
# <a name="windowsprotectionstate-resource-type"></a>tipo de recurso Windowsprotectionstate foi

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade de status de proteção de dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter Windowsprotectionstate foi](../api/intune-devices-windowsprotectionstate-get.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Leia as propriedades e as relações do objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .|
|[Atualizar Windowsprotectionstate foi](../api/intune-devices-windowsprotectionstate-update.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Atualiza as propriedades de um objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do objeto de status de proteção de dispositivo. Esta é a ID do dispositivo|
|malwareProtectionEnabled|Booliano|O anti-malware está habilitado ou não|
|DeviceState|[windowsDeviceHealthState](../resources/intune-devices-windowsdevicehealthstate.md)|Estado do computador (como verificação completa ou pendente ou reinicialização pendente, etc.). Os possíveis valores são: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.|
|realTimeProtectionEnabled|Booliano|A proteção em tempo real está habilitada ou não?|
|networkInspectionSystemEnabled|Booliano|Sistema de inspeção de rede habilitado ou não?|
|quickScanOverdue|Booliano|Verificação rápida em atraso ou não?|
|fullScanOverdue|Booliano|Verificação completa em atraso ou não?|
|signatureUpdateOverdue|Booliano|Assinatura desatualizada ou não?|
|rebootRequired|Booliano|Reinicialização necessária ou não?|
|fullScanRequired|Booliano|Verificação completa necessária ou não?|
|engineVersion|String|Versão atual do mecanismo do Endpoint Protection|
|signatureVersion|String|Versão atual de definições de malware|
|antiMalwareVersion|String|Versão Antimalware atual|
|lastQuickScanDateTime|DateTimeOffset|Data e hora da última verificação rápida|
|lastFullScanDateTime|DateTimeOffset|Data e hora da última verificação rápida|
|lastQuickScanSignatureVersion|String|Versão da última assinatura de verificação rápida|
|lastFullScanSignatureVersion|String|Versão da última assinatura de verificação completa|
|lastReportedDateTime|DateTimeOffset|Hora do último status de integridade do dispositivo relatado|
|productStatus|[windowsDefenderProductStatus](../resources/intune-devices-windowsdefenderproductstatus.md)|Status do produto do Windows Defender antivírus. Os valores possíveis são:,,,,,,,,,,,,,,, `noStatus` `serviceNotRunning` `serviceStartedWithoutMalwareProtection` `pendingFullScanDueToThreatAction` `pendingRebootDueToThreatAction` `pendingManualStepsDueToThreatAction` `avSignaturesOutOfDate` `asSignaturesOutOfDate` `noQuickScanHappenedForSpecifiedPeriod` `noFullScanHappenedForSpecifiedPeriod` `systemInitiatedScanInProgress` `systemInitiatedCleanInProgress` `samplesPendingSubmission` `productRunningInEvaluationMode` `productRunningInNonGenuineMode` `productExpired` `offlineScanRequired` , `serviceShutdownAsPartOfSystemShutdown` , `threatRemediationFailedCritically` , `threatRemediationFailedNonCritically` `noStatusFlagsSet` `platformOutOfDate` `platformUpdateInProgress` `platformAboutToBeOutdated` `signatureOrPlatformEndOfLifeIsPastOrIsImpending` `windowsSModeSignaturesInUseOnNonWin10SInstall` ,,,,,,,,,,,,,,,.|
|isVirtualMachine|Booliano|Indica se o dispositivo é uma máquina virtual.|
|tamperProtectionEnabled|Booliano|Indica se o recurso proteção de violação do Windows Defender está habilitado.|

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
  "lastReportedDateTime": "String (timestamp)",
  "productStatus": "String",
  "isVirtualMachine": true,
  "tamperProtectionEnabled": true
}
```




