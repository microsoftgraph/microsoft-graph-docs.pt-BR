---
title: Tipo de recurso macOSCompliancePolicy
description: Essa classe contém configurações de conformidade para o Mac OS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6d33b4e3ac57206a664dc1faaf722e6dad03c736
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268759"
---
# <a name="macoscompliancepolicy-resource-type"></a>Tipo de recurso macOSCompliancePolicy

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Essa classe contém configurações de conformidade para o Mac OS.


Herda de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar macOSCompliancePolicies](../api/intune-deviceconfig-macoscompliancepolicy-list.md)|Coleção [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md)|Lista propriedades e relações dos objetos [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).|
|[Obter macOSCompliancePolicy](../api/intune-deviceconfig-macoscompliancepolicy-get.md)|[macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md)|Propriedades de leitura e relações do objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).|
|[Criar macOSCompliancePolicy](../api/intune-deviceconfig-macoscompliancepolicy-create.md)|[macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md)|Cria um novo objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).|
|[Excluir macOSCompliancePolicy](../api/intune-deviceconfig-macoscompliancepolicy-delete.md)|Nenhum|Exclui um [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).|
|[Atualizar macOSCompliancePolicy](../api/intune-deviceconfig-macoscompliancepolicy-update.md)|[macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md)|Atualiza as propriedades de um objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|id|String|Chave da entidade. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|description|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|version|Int32|Versão da configuração do dispositivo. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|passwordRequired|Boolean|Se uma senha deve ou não ser exigida.|
|passwordBlockSimple|Booliano|Indica se senhas simples devem ou não ser bloqueadas.|
|passwordExpirationDays|Int32|Número de dias antes da expiração da senha. Valores válidos de 1 a 65535|
|passwordMinimumLength|Int32|Comprimento mínimo da senha. Valores válidos de 4 a 14|
|passwordMinutesOfInactivityBeforeLock|Int32|Minutos de inatividade antes que uma senha seja necessária.|
|passwordPreviousPasswordBlockCount|Int32|Número de senhas anteriores para bloquear. Valores válidos de 1 a 24|
|passwordMinimumCharacterSetCount|Int32|O número de conjuntos de caracteres necessários na senha.|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|O tipo de senha necessária. Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.|
|osMinimumVersion|String|Versão mínima do MacOS.|
|osMaximumVersion|String|Versão máxima do MacOS.|
|osMinimumBuildVersion|String|Versão mínima do MacOS.|
|osMaximumBuildVersion|String|Versão máxima do MacOS.|
|systemIntegrityProtectionEnabled|Booliano|Exige que dispositivos tenham habilitado a proteção de integridade do sistema.|
|deviceThreatProtectionEnabled|Boolean|Exige que os dispositivos tenham habilitada a proteção contra ameaças.|
|deviceThreatProtectionRequiredSecurityLevel|[deviceThreatProtectionLevel](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade. Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.|
|storageRequireEncryption|Booliano|Exige criptografia em dispositivos Mac OS.|
|gatekeeperAllowedAppSource|[macOSGatekeeperAppSources](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|Configuração de sistema e privacidade que determina quais locais de download os aplicativos podem ser executados em um dispositivo macOS. Os valores possíveis são: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.|
|firewallEnabled|Booliano|Se o firewall deve ser habilitado ou não.|
|firewallBlockAllIncoming|Booliano|Corresponde à opção "bloquear todas as conexões de entrada".|
|firewallEnableStealthMode|Booliano|Corresponde a "Habilitar modo oculto".|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|scheduledActionsForRule|Coleção [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|A lista de ações agendadas para esta regra. Herdado de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|deviceStatuses|Coleção [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)|Lista de DeviceComplianceDeviceStatus. Herdado de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|userStatuses|Coleção [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)|Lista de DeviceComplianceUserStatus. Herdado de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|Visão geral de status de dispositivos para Conformidade de dispositivo. Herdado de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|Visão geral de status de usuários para Conformidade de dispositivo. Herdado de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Visão geral de dispositivos de estado para Configuração de Conformidade. Herdado de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|assignments|Coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|A coleção de atribuições para essa política de conformidade. Herdado de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
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
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordRequiredType": "String",
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "osMinimumBuildVersion": "String",
  "osMaximumBuildVersion": "String",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "String",
  "storageRequireEncryption": true,
  "gatekeeperAllowedAppSource": "String",
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```




