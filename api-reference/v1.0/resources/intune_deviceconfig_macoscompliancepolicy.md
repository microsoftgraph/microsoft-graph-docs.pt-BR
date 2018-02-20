# <a name="macoscompliancepolicy-resource-type"></a>Tipo de recurso macOSCompliancePolicy

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Essa classe contém configurações de conformidade para o Mac OS.

Herda de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar macOSCompliancePolicies](../api/intune_deviceconfig_macoscompliancepolicy_list.md)|Coleção [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md)|Lista propriedades e relações dos objetos [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md).|
|[Obter macOSCompliancePolicy](../api/intune_deviceconfig_macoscompliancepolicy_get.md)|[macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md)|Propriedades de leitura e relações do objeto [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md).|
|[Criar macOSCompliancePolicy](../api/intune_deviceconfig_macoscompliancepolicy_create.md)|[macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md)|Cria um novo objeto [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md).|
|[Excluir macOSCompliancePolicy](../api/intune_deviceconfig_macoscompliancepolicy_delete.md)|Nenhum|Exclui um [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md).|
|[Atualizar macOSCompliancePolicy](../api/intune_deviceconfig_macoscompliancepolicy_update.md)|[macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md)|Atualiza as propriedades de um objeto [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|createdDateTime|DateTimeOffset|Data e hora em que o objeto foi criado. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|description|Cadeia de caracteres|Descrição fornecida pelo administrador da Configuração do dispositivo. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|displayName|Cadeia de caracteres|Nome fornecido pelo administrador da configuração do dispositivo. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|passwordRequired|Booliano|Se uma senha deve ou não ser exigida.|
|passwordBlockSimple|Booliano|Indica se senhas simples devem ou não ser bloqueadas.|
|passwordExpirationDays|Int32|Número de dias antes da expiração da senha. Valores válidos de 1 a 65535|
|passwordMinimumLength|Int32|Comprimento mínimo da senha. Valores válidos de 4 a 14|
|passwordMinutesOfInactivityBeforeLock|Int32|Minutos de inatividade antes que uma senha seja necessária.|
|passwordPreviousPasswordBlockCount|Int32|Número de senhas anteriores para bloquear. Valores válidos de 1 a 24|
|passwordMinimumCharacterSetCount|Int32|O número de conjuntos de caracteres necessários na senha.|
|passwordRequiredType|Cadeia de caracteres|O tipo de senha necessária. Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.|
|osMinimumVersion|Cadeia de caracteres|Versão mínima do IOS.|
|osMaximumVersion|Cadeia de caracteres|Versão máxima do iOS.|
|systemIntegrityProtectionEnabled|Booliano|Exige que dispositivos tenham habilitado a proteção de integridade do sistema.|
|deviceThreatProtectionEnabled|Booliano|Exige que os dispositivos tenham habilitada a proteção contra ameaças.|
|deviceThreatProtectionRequiredSecurityLevel|Cadeia de caracteres|Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade. Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.|
|storageRequireEncryption|Booliano|Exige criptografia em dispositivos Mac OS.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|scheduledActionsForRule|Coleção [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)|A lista de ações agendadas para esta regra. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|deviceStatuses|Coleção [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md)|Lista de DeviceComplianceDeviceStatus. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|userStatuses|Coleção [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)|Lista de DeviceComplianceUserStatus. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|Visão geral de status de dispositivos para Conformidade de dispositivo. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|Visão geral de status de usuários para Conformidade de dispositivo. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Visão geral de dispositivos de estado para Configuração de Conformidade. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|assignments|Coleção [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)|A coleção de atribuições para essa política de conformidade. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|

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
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "String",
  "storageRequireEncryption": true
}
```



