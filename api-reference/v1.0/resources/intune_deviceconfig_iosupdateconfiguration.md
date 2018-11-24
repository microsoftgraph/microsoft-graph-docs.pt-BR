# <a name="iosupdateconfiguration-resource-type"></a>iosUpdateConfiguration resource type

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

A Configuração de Atualização do iOS permite que você configure a janela de tempo na semana para instalar atualizações do iOS

Herda de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosUpdateConfigurations](../api/intune_deviceconfig_iosupdateconfiguration_list.md)|Coleção [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md)|Lista propriedades e relações dos objetos [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md).|
|[Obter iosUpdateConfiguration](../api/intune_deviceconfig_iosupdateconfiguration_get.md)|[iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md)|Propriedades de leitura e relações do objeto [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md).|
|[Criar iosUpdateConfiguration](../api/intune_deviceconfig_iosupdateconfiguration_create.md)|[iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md)|Cria um novo objeto [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md).|
|[Excluir iosUpdateConfiguration](../api/intune_deviceconfig_iosupdateconfiguration_delete.md)|Nenhum|Exclui um [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md).|
|[Atualizar iosUpdateConfiguration](../api/intune_deviceconfig_iosupdateconfiguration_update.md)|[iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md)|Atualiza as propriedades de um objeto [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|activeHoursStart|TimeOfDay|Início do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)|
|activeHoursEnd|TimeOfDay|Término do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)|
|scheduledInstallDays|coleção [dayOfWeek](../resources/intune_deviceconfig_dayofweek.md)|Dias na semana para os quais o horário ativo está configurado. Essa coleção pode conter um máximo de 7 elementos.|
|utcTimeOffsetInMinutes|Int32|Deslocamento do horário UTC indicado em minutos|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|Status de instalação da configuração do dispositivo por dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)|Status de instalação da configuração de dispositivo por usuário. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Visão geral de status de dispositivos para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Visão geral de status de usuários para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Visão geral de dispositivos de configuração para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosUpdateConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "activeHoursStart": "String (time of day)",
  "activeHoursEnd": "String (time of day)",
  "scheduledInstallDays": [
    "String"
  ],
  "utcTimeOffsetInMinutes": 1024
}
```



<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune_deviceconfig_iosupdateconfiguration.md/microsoft.graph.iosUpdateConfiguration/scheduledInstallDays:
      Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->
