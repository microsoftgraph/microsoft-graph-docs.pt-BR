# <a name="macosgeneraldeviceconfiguration-resource-type"></a>Tipo de recurso macOSGeneralDeviceConfiguration

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso macOSGeneralDeviceConfiguration.

Herda de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar macOSGeneralDeviceConfigurations](../api/intune_deviceconfig_macosgeneraldeviceconfiguration_list.md)|Coleção [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md)|Lista propriedades e relações dos objetos [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md).|
|[Obter macOSGeneralDeviceConfiguration](../api/intune_deviceconfig_macosgeneraldeviceconfiguration_get.md)|[macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md)|Propriedades de leitura e relações do objeto [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md).|
|[Criar macOSGeneralDeviceConfiguration](../api/intune_deviceconfig_macosgeneraldeviceconfiguration_create.md)|[macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md)|Cria um novo objeto [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md).|
|[Excluir macOSGeneralDeviceConfiguration](../api/intune_deviceconfig_macosgeneraldeviceconfiguration_delete.md)|Nenhum|Exclui um [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md).|
|[Atualizar macOSGeneralDeviceConfiguration](../api/intune_deviceconfig_macosgeneraldeviceconfiguration_update.md)|[macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md)|Atualiza as propriedades de um objeto [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|compliantAppsList|Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)|Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType). Essa coleção pode conter um máximo de 10.000 elementos.|
|compliantAppListType|[appListType](../resources/intune_deviceconfig_applisttype.md)|Lista que está em CompliantAppsList. Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|emailInDomainSuffixes|Coleção de sequência de caracteres|Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.|
|passwordBlockSimple|Booleano|Bloquear senhas simples.|
|passwordExpirationDays|Int32|Número de dias antes da expiração da senha.|
|passwordMinimumCharacterSetCount|Int32|Número de conjuntos de caracteres que uma senha deve conter. Valores válidos de 0 a 4|
|passwordMinimumLength|Int32|Comprimento mínimo das senhas.|
|passwordMinutesOfInactivityBeforeLock|Int32|Minutos de inatividade necessários antes que uma senha seja necessária.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Minutos de inatividade necessários antes que a tela atinja o tempo limite.|
|passwordPreviousPasswordBlockCount|Int32|Número de senhas anteriores para bloquear.|
|passwordRequiredType|[requiredPasswordType](../resources/intune_deviceconfig_requiredpasswordtype.md)|Tipo de senha necessária. Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordRequired|Booleano|Se uma senha deve ou não ser exigida.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|Status de instalação da configuração do dispositivo por dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatuses|Conjunto [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)|Status de instalação da configuração do dispositivo por usuário. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Visão geral de status dos dispositivos na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Visão geral de status dos usuários na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Resumo de dispositivo de estado de configuração do dispositivo Herdada do [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceConfiguration",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSGeneralDeviceConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "compliantAppListType": "String",
  "emailInDomainSuffixes": [
    "String"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordRequiredType": "String",
  "passwordRequired": true
}
```








