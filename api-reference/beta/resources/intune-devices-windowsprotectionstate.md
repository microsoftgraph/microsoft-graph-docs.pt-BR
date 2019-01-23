---
title: tipo de recurso de windowsProtectionState
description: Entidade de status de proteção do dispositivo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1ef6c86983475abc687055ac2322ba02fae27ecd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423584"
---
# <a name="windowsprotectionstate-resource-type"></a>tipo de recurso de windowsProtectionState

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

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




