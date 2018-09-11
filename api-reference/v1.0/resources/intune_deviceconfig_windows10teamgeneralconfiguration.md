# <a name="windows10teamgeneralconfiguration-resource-type"></a>Tipo de recurso windows10TeamGeneralConfiguration

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso windows10TeamGeneralConfiguration.

Herda de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windows10TeamGeneralConfigurations](../api/intune_deviceconfig_windows10teamgeneralconfiguration_list.md)|Coleção [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md)|Lista propriedades e relações dos objetos [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md).|
|[Obter windows10TeamGeneralConfiguration](../api/intune_deviceconfig_windows10teamgeneralconfiguration_get.md)|[windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md)|LEr propriedades e relações do objeto [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md).|
|[Criar windows10TeamGeneralConfiguration](../api/intune_deviceconfig_windows10teamgeneralconfiguration_create.md)|[windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md)|Criar um novo objeto [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md).|
|[Excluir windows10TeamGeneralConfiguration](../api/intune_deviceconfig_windows10teamgeneralconfiguration_delete.md)|Nenhum|Excluir um [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md)|
|[Atualizar windows10TeamGeneralConfiguration](../api/intune_deviceconfig_windows10teamgeneralconfiguration_update.md)|[windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md)|Atualizar as propriedades de um objeto [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|descrição|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|azureOperationalInsightsBlockTelemetry|Booleano|Indica se os Insights Operacionais do Azure devem ou não ser bloqueados.|
|azureOperationalInsightsWorkspaceId|Cadeia de caracteres|A ID do espaço de trabalho dos Insights Operacionais do Azure.|
|azureOperationalInsightsWorkspaceKey|Cadeia de caracteres|A chave do espaço de trabalho dos Insights Operacionais do Azure.|
|connectAppBlockAutoLaunch|Booleano|Especifica se o aplicativo Connect deverá ser iniciado automaticamente sempre que uma projeção for iniciada.|
|maintenanceWindowBlocked|Booleano|Indica se a configuração de uma janela de manutenção para atualizações do dispositivo deverá ou não ser bloqueada.|
|maintenanceWindowDurationInHours|Int32|Duração da janela de manutenção para atualizações do dispositivo. Valores válidos: 0 a 5|
|maintenanceWindowStartTime|TimeOfDay|Hora de Início da janela de manutenção para atualizações do dispositivo.|
|miracastChannel|[miracastChannel](../resources/intune_deviceconfig_miracastchannel.md)|O canal. Os valores possíveis são: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.|
|miracastBlocked|Booleano|Indica se a projeção sem fio deve ou não ser bloqueada.|
|miracastRequirePin|Booleano|Indica se será exigido um pin para a projeção sem fio.|
|settingsBlockMyMeetingsAndFiles|Booleano|Especifica se o recurso "Meus arquivos e reuniões" no menu Iniciar, que mostra as reuniões e arquivos do usuário conectado do Office 365, deverá ser desativado.|
|settingsBlockSessionResume|Booleano|Especifica se a capacidade de retomar uma sessão quando a sessão expirar será permitida.|
|settingsBlockSigninSuggestions|Booleano|Especifica se o preenchimento automático da caixa de diálogo de entrada com os convidados de reuniões agendadas será desativado.|
|settingsDefaultVolume|Int32|Especifica o valor padrão de volume de uma nova sessão. Os valores permitidos ficam entre 0 e 100. O padrão é 45. Valores válidos de 0 a 100|
|settingsScreenTimeoutInMinutes|Int32|Especifica o número de minutos até a tela do Hub ser desligada.|
|settingsSessionTimeoutInMinutes|Int32|Especifica o número de minutos até a sessão atingir o tempo limite.|
|settingsSleepTimeoutInMinutes|Int32|Especifica o número de minutos até o Hub entrar no modo de suspensão.|
|welcomeScreenBlockAutomaticWakeUp|Booleano|Indica se a tela de boas-vindas será impedida de ser desativada automaticamente quando alguém entrar na sala.|
|welcomeScreenBackgroundImageUrl|Cadeia de caracteres|A URL da imagem de fundo da tela de boas-vindas. A URL deve usar o protocolo HTTPS e retornar uma imagem PNG.|
|welcomeScreenMeetingInformation|[welcomeScreenMeetingInformation](../resources/intune_deviceconfig_welcomescreenmeetinginformation.md)|As informações da reunião mostradas na tela de boas-vindas. Os valores possíveis são: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.|

## <a name="relationships"></a>Relacionamentos
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
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
  "@odata.type": "microsoft.graph.windows10TeamGeneralConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "String",
  "azureOperationalInsightsWorkspaceKey": "String",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 1024,
  "maintenanceWindowStartTime": "String (time of day)",
  "miracastChannel": "String",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 1024,
  "settingsScreenTimeoutInMinutes": 1024,
  "settingsSessionTimeoutInMinutes": 1024,
  "settingsSleepTimeoutInMinutes": 1024,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "String",
  "welcomeScreenMeetingInformation": "String"
}
```








