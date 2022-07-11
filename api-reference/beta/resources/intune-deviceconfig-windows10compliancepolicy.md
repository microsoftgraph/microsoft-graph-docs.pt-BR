---
title: Tipo de recurso windows10CompliancePolicy
description: Essa classe contém configurações de conformidade para o Windows 10.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 63c2fe7b80b7b7aadacb95174fd56faeb00fa3ed
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668409"
---
# <a name="windows10compliancepolicy-resource-type"></a>Tipo de recurso windows10CompliancePolicy

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Essa classe contém configurações de conformidade para o Windows 10.


Herda de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windows10CompliancePolicies](../api/intune-deviceconfig-windows10compliancepolicy-list.md)|Coleção [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)|Lista propriedades e relações dos objetos [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).|
|[Obter windows10CompliancePolicy](../api/intune-deviceconfig-windows10compliancepolicy-get.md)|[windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)|Propriedades de leitura e relações do objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).|
|[Criar windows10CompliancePolicy](../api/intune-deviceconfig-windows10compliancepolicy-create.md)|[windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)|Cria um novo objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).|
|[Excluir windows10CompliancePolicy](../api/intune-deviceconfig-windows10compliancepolicy-delete.md)|Nenhum|Exclui um [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).|
|[Atualizar windows10CompliancePolicy](../api/intune-deviceconfig-windows10compliancepolicy-update.md)|[windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)|Atualiza as propriedades de um objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|roleScopeTagIds|Conjunto de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade. Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|descrição|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|version|Int32|Versão da configuração do dispositivo. Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|passwordRequired|Booliano|Exige uma senha para desbloquear o dispositivo Windows.|
|passwordBlockSimple|Booliano|Indica se a senha simples deve ou não ser bloqueada.|
|passwordRequiredToUnlockFromIdle|Booliano|Exige uma senha para desbloquear o dispositivo ocioso.|
|passwordMinutesOfInactivityBeforeLock|Int32|Minutos de inatividade antes que uma senha seja necessária.|
|passwordExpirationDays|Int32|A expiração da senha em dias.|
|passwordMinimumLength|Int32|Comprimento mínimo da senha.|
|passwordMinimumCharacterSetCount|Int32|O número de conjuntos de caracteres necessários na senha.|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|O tipo de senha necessária. Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordPreviousPasswordBlockCount|Int32|O número de senhas anteriores cujo uso deve ser evitado.|
|requireHealthyDeviceReport|Booliano|Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.|
|osMinimumVersion|Cadeia de caracteres|Versão mínima do Windows 10.|
|osMaximumVersion|Cadeia de caracteres|Versão máxima do Windows 10.|
|mobileOsMinimumVersion|Cadeia de caracteres|Versão mínima do Windows Phone.|
|mobileOsMaximumVersion|Cadeia de caracteres|Versão máxima do Windows Phone.|
|earlyLaunchAntiMalwareDriverEnabled|Boolean|Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.|
|bitLockerEnabled|Boolean|Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado|
|secureBootEnabled|Boolean|Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.|
|codeIntegrityEnabled|Boolean|Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.|
|storageRequireEncryption|Boolean|Exige criptografia em dispositivos Windows.|
|activeFirewallRequired|Booliano|Exigir firewall ativo em dispositivos Windows.|
|defenderEnabled|Booliano|Exigir Windows Defender Antimalware em dispositivos Windows.|
|defenderVersion|Cadeia de Caracteres|Exigir Windows Defender versão mínima do Antimalware em dispositivos Windows.|
|signatureOutOfDate|Booleano|Exigir Windows Defender Assinatura Antimalware esteja atualizada em dispositivos Windows.|
|rtpEnabled|Booleano|Exigir Windows Defender antimalware Real-Time proteção em dispositivos Windows.|
|antivirusRequired|Booleano|Exigir que qualquer solução antivírus registrada no Centro de Segurança do Windows esteja ativada e monitorando (por exemplo, Symantec, Windows Defender).|
|antiSpywareRequired|Booleano|Exigir que qualquer solução AntiSpyware registrada no Centro de Decurity do Windows esteja ativada e monitorando (por exemplo, Symantec, Windows Defender).|
|validOperatingSystemBuildRanges|[Coleção operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)|Os intervalos de build do sistema operacional válidos em dispositivos Windows. Essa coleção pode conter um máximo de 10.000 elementos.|
|deviceThreatProtectionEnabled|Boolean|Exige que os dispositivos tenham habilitada a proteção contra ameaças.|
|deviceThreatProtectionRequiredSecurityLevel|[deviceThreatProtectionLevel](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|Exigir nível mínimo de risco da Proteção contra Ameaças do Dispositivo para relatar não conformidade. Os possíveis valores são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.|
|configurationManagerComplianceRequired|Booleano|É necessário considerar o estado de Conformidade do SCCM em consideração para o Intune de Conformidade.|
|tpmRequired|Booleano|Exigir que o TPM (Trusted Platform Module) esteja presente.|
|deviceCompliancePolicyScript|[deviceCompliancePolicyScript](../resources/intune-deviceconfig-devicecompliancepolicyscript.md)|Ainda não documentado|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|scheduledActionsForRule|Coleção [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|A lista de ações agendadas por regra para essa política de conformidade. Essa é uma propriedade necessária ao criar políticas de conformidade individuais por plataforma. Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|deviceStatuses|Coleção [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)|Lista de DeviceComplianceDeviceStatus. Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|userStatuses|Coleção [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)|Lista de DeviceComplianceUserStatus. Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|Visão geral de status de dispositivos para Conformidade de dispositivo. Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|Visão geral de status de usuários para Conformidade de dispositivo. Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Visão geral de dispositivos de estado para Configuração de Conformidade. Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|assignments|Coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|A coleção de atribuições para essa política de conformidade. Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10CompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordRequiredType": "String",
  "passwordPreviousPasswordBlockCount": 1024,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "mobileOsMinimumVersion": "String",
  "mobileOsMaximumVersion": "String",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "defenderEnabled": true,
  "defenderVersion": "String",
  "signatureOutOfDate": true,
  "rtpEnabled": true,
  "antivirusRequired": true,
  "antiSpywareRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "String",
      "lowestVersion": "String",
      "highestVersion": "String"
    }
  ],
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "String",
  "configurationManagerComplianceRequired": true,
  "tpmRequired": true,
  "deviceCompliancePolicyScript": {
    "@odata.type": "microsoft.graph.deviceCompliancePolicyScript",
    "deviceComplianceScriptId": "String",
    "rulesContent": "binary"
  }
}
```




