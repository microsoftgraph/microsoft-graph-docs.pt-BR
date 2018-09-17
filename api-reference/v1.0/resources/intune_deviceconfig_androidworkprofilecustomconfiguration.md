# <a name="androidworkprofilecustomconfiguration-resource-type"></a>Tipo de recurso de androidWorkProfileCustomConfiguration

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Configuração personalizada do Perfil de Trabalho do Android

Herda de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista androidWorkProfileCustomConfigurations](../api/intune_deviceconfig_androidworkprofilecustomconfiguration_list.md)|Coleção [androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md)|Propriedades da lista e relacionamentos de objetos [androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md).|
|[Obter androidWorkProfileCustomConfiguration](../api/intune_deviceconfig_androidworkprofilecustomconfiguration_get.md)|[androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md)|Propriedades de leitura e relacionamentos do objeto [androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md) .|
|[Criar androidWorkProfileCustomConfiguration](../api/intune_deviceconfig_androidworkprofilecustomconfiguration_create.md)|[androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md)|Crie um novo objeto [androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md) .|
|[Excluir androidWorkProfileCustomConfiguration](../api/intune_deviceconfig_androidworkprofilecustomconfiguration_delete.md)|Nenhum|Exclui um [androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md).|
|[Atualizar androidWorkProfileCustomConfiguration](../api/intune_deviceconfig_androidworkprofilecustomconfiguration_update.md)|[androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md)|Atualizar as propriedades de um objeto [androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|descrição|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|omaSettings|Coleção [omaSetting](../resources/intune_deviceconfig_omasetting.md)|Configurações OMA. Esta coleção pode conter um máximo de 500 elementos.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|atribuições|Coleção [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|Status de instalação da configuração do dispositivo por dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)|Status de instalação da configuração do dispositivo por usuário. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Visão geral de status dos dispositivos na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Visão geral de status dos usuários na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Resumo de dispositivo de estado de configuração do dispositivo Herdada do [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceConfiguration",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidWorkProfileCustomConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "String",
      "description": "String",
      "omaUri": "String",
      "value": 1024
    }
  ]
}
```








