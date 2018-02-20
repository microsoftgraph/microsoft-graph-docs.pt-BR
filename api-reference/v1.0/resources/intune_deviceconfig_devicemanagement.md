# <a name="devicemanagement-resource-type"></a>Tipo de recurso deviceManagement

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagement](../api/intune_deviceconfig_devicemanagement_get.md)|[deviceManagement](../resources/intune_deviceconfig_devicemanagement.md)|Propriedades de leitura e relações do objeto [deviceManagement](../resources/intune_deviceconfig_devicemanagement.md).|
|[Atualizar deviceManagement](../api/intune_deviceconfig_devicemanagement_update.md)|[deviceManagement](../resources/intune_deviceconfig_devicemanagement.md)|Atualiza as propriedades de um objeto [deviceManagement](../resources/intune_deviceconfig_devicemanagement.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo|
|settings|[deviceManagementSettings](../resources/intune_deviceconfig_devicemanagementsettings.md)|Configurações de nível da conta.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|deviceConfigurations|Coleção [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|As configurações de dispositivos.|
|deviceCompliancePolicies|Coleção [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|As políticas de conformidade do dispositivo.|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md)|O resumo do status de atualização do software.|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)|O resumo do estado de conformidade dos dispositivos para esta conta.|
|deviceCompliancePolicySettingStateSummaries|Coleção [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)|Os estados resumidos das configurações da política de conformidade para esta conta.|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)|O resumo do estado de configuração de dispositivos para esta conta.|
|iosUpdateStatuses|Coleção [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md)|Os status de instalação de atualizações de software do iOS para esta conta.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "settings": {
    "@odata.type": "microsoft.graph.deviceManagementSettings",
    "deviceComplianceCheckinThresholdDays": 1024,
    "isScheduledActionEnabled": true,
    "secureByDefault": true
  }
}
```



