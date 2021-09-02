---
title: Tipo de recurso windowsProtectionState
description: Entidade de status de proteção de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 640198171fd9b83c6522a8c8b07b84fa186657ab
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803234"
---
# <a name="windowsprotectionstate-resource-type"></a>Tipo de recurso windowsProtectionState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade de status de proteção de dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter windowsProtectionState](../api/intune-devices-windowsprotectionstate-get.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Leia propriedades e relações do [objeto windowsProtectionState.](../resources/intune-devices-windowsprotectionstate.md)|
|[Atualizar windowsProtectionState](../api/intune-devices-windowsprotectionstate-update.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Atualize as propriedades de um [objeto windowsProtectionState.](../resources/intune-devices-windowsprotectionstate.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O Identificador exclusivo do objeto de status de proteção do dispositivo. Esta é a ID do dispositivo|
|malwareProtectionEnabled|Boleano|O anti malware está habilitado ou não|
|deviceState|[windowsDeviceHealthState](../resources/intune-devices-windowsdevicehealthstate.md)|Estado do computador (como verificação completa ou pendente ou reinicialização pendente etc.). Os possíveis valores são: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.|
|realTimeProtectionEnabled|Booliano|A proteção em tempo real está habilitada ou não?|
|networkInspectionSystemEnabled|Boleano|Sistema de inspeção de rede habilitado ou não?|
|quickScanOverdue|Boleano|Verificação rápida atrasada ou não?|
|fullScanOverdue|Boleano|Verificação completa atrasada ou não?|
|signatureUpdateOverdue|Boleano|Assinatura desa datada ou não?|
|rebootRequired|Boleano|Reiniciar obrigatório ou não?|
|fullScanRequired|Boleano|Verificação completa necessária ou não?|
|engineVersion|Cadeia de caracteres|Versão atual do mecanismo de proteção de ponto de extremidade|
|signatureVersion|Cadeia de caracteres|Versão atual das definições de malware|
|antiMalwareVersion|Cadeia de caracteres|Versão anti malware atual|
|lastQuickScanDateTime|DateTimeOffset|Data da última verificação rápida|
|lastFullScanDateTime|DateTimeOffset|Data da última verificação rápida|
|lastQuickScanSignatureVersion|Cadeia de caracteres|Última versão de assinatura de verificação rápida|
|lastFullScanSignatureVersion|Cadeia de caracteres|Última versão de assinatura de verificação completa|
|lastReportedDateTime|DateTimeOffset|Tempo de notificado do último status de saúde do dispositivo|
|productStatus|[windowsDefenderProductStatus](../resources/intune-devices-windowsdefenderproductstatus.md)|Status do produto Windows Defender Antivírus. Os valores possíveis são: `noStatus` , , , , , , , , `serviceNotRunning` `serviceStartedWithoutMalwareProtection` `pendingFullScanDueToThreatAction` `pendingRebootDueToThreatAction` `pendingManualStepsDueToThreatAction` `avSignaturesOutOfDate` `asSignaturesOutOfDate` `noQuickScanHappenedForSpecifiedPeriod` `noFullScanHappenedForSpecifiedPeriod` `systemInitiatedScanInProgress` `systemInitiatedCleanInProgress` `samplesPendingSubmission` `productRunningInEvaluationMode` , `productRunningInNonGenuineMode` `productExpired` `offlineScanRequired` `serviceShutdownAsPartOfSystemShutdown` `threatRemediationFailedCritically` `threatRemediationFailedNonCritically` `noStatusFlagsSet` `platformOutOfDate` `platformUpdateInProgress` `platformAboutToBeOutdated` `signatureOrPlatformEndOfLifeIsPastOrIsImpending` `windowsSModeSignaturesInUseOnNonWin10SInstall`|
|isVirtualMachine|Boleano|Indica se o dispositivo é uma máquina virtual.|
|tamperProtectionEnabled|Boleano|Indica se o recurso Windows Defender proteção contra adulteração está habilitado.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|detectedMalwareState|[Coleção windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)|Lista de malware de dispositivo|

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



