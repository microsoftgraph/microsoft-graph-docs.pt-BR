# <a name="ioscustomconfiguration-resource-type"></a>iosCustomConfiguration resource type

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso iosCustomConfiguration.

Herda de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosCustomConfigurations](../api/intune_deviceconfig_ioscustomconfiguration_list.md)|Coleção [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md)|Lista propriedades e relações dos objetos [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md).|
|[Obter iosCustomConfiguration](../api/intune_deviceconfig_ioscustomconfiguration_get.md)|[iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md)|Propriedades de leitura e relações do objeto [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md).|
|[Criar iosCustomConfiguration](../api/intune_deviceconfig_ioscustomconfiguration_create.md)|[iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md)|Cria um novo objeto [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md).|
|[Excluir iosCustomConfiguration](../api/intune_deviceconfig_ioscustomconfiguration_delete.md)|Nenhum|Exclui um [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md).|
|[Atualizar iosCustomConfiguration](../api/intune_deviceconfig_ioscustomconfiguration_update.md)|[iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md)|Atualiza as propriedades de um objeto [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|Data e hora em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|description|Cadeia de caracteres|Descrição fornecida pelo administrador da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|Cadeia de caracteres|Nome fornecido pelo administrador da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|payloadName|Cadeia de caracteres|Nome que é exibido para o usuário.|
|payloadFileName|Cadeia de caracteres|O nome do arquivo de carga (*.mobileconfig | *.xml).|
|payload|Binária|Carga. (Matriz de bytes codificados em UTF8)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|Status da instalação da configuração de dispositivo por dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)|Status de instalação da configuração de dispositivo por usuário. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Visão geral de status de dispositivos para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Visão geral de status de usuários para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Visão geral de dispositivos de configuração para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosCustomConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "payloadName": "String",
  "payloadFileName": "String",
  "payload": "binary"
}
```



