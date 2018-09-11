# <a name="deviceconfiguration-resource-type"></a>Tipo de recurso deviceConfiguration

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Configuração do dispositivo.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceConfigurations](../api/intune_deviceconfig_deviceconfiguration_list.md)|Conjunto [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|Listar propriedades e relações de objetos de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|[Obter deviceConfiguration](../api/intune_deviceconfig_deviceconfiguration_get.md)|[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|Ler propriedades e relações de objetos de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|[atribuir ação](../api/intune_deviceconfig_deviceconfiguration_assign.md)|Conjunto [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|lastModifiedDateTime|DateTimeOffset|Última modificação de DateTime do objeto.|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado.|
|descrição|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo.|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo.|
|version|Int32|Versão da configuração do dispositivo.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo.|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|Status de instalação da configuração de dispositivo por dispositivo.|
|userStatuses|coleção [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)|Status de instalação da configuração do dispositivo por usuário.|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Visão geral do status dos dispositivos da configuração de dispositivos|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Visão geral do status dos usuários da configuração de dispositivos|
|deviceSettingStateSummaries|Conjunto [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Resumo do dispositivo do estado de definição de configuração do dispositivo|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024
}
```








