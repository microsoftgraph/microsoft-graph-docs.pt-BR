# <a name="targetedmanagedappprotection-resource-type"></a>Tipo de recurso targetedManagedAppProtection

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Política usada para definir configurações de gerenciamento detalhadas direcionadas a grupos de segurança específicos

Herda de [managedAppProtection](../resources/intune_mam_managedappprotection.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar targetedManagedAppProtections](../api/intune_mam_targetedmanagedappprotection_list.md)|Coleção [targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md)|Listar propriedades e relações dos objetos [targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md).|
|[Obter targetedManagedAppProtection](../api/intune_mam_targetedmanagedappprotection_get.md)|[targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md)|Ler propriedades e relações do objeto [targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md).|
|[Ação assign](../api/intune_mam_targetedmanagedappprotection_assign.md)|Nenhum|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome para exibição da política. Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|description|Cadeia de caracteres|A descrição da política. Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|createdDateTime|DateTimeOffset|A data e a hora da criação da política. Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|Última vez em que a política foi modificada. Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|id|String|Chave da entidade. Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|version|Cadeia de caracteres|Versão da entidade. Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|periodOfflineBeforeAccessCheck|Duração|Período após o qual o acesso é verificado quando o dispositivo não está conectado à Internet. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|periodOnlineBeforeAccessCheck|Duração|Período após o qual o acesso é verificado quando o dispositivo está conectado à Internet. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|allowedInboundDataTransferSources|String|Fontes das quais os dados podem ser transferidos. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md). Os possíveis valores são: `allApps`, `managedApps`, `none`.|
|allowedOutboundDataTransferDestinations|String|Destinos para os quais os dados podem ser transferidos. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md). Os possíveis valores são: `allApps`, `managedApps`, `none`.|
|organizationalCredentialsRequired|Boolean|Indica se as credenciais organizacionais são obrigatórias para o uso do aplicativo. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|allowedOutboundClipboardSharingLevel|String|O nível em que a área de transferência pode ser compartilhada entre os aplicativos no dispositivo gerenciado. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md). Os possíveis valores são: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|dataBackupBlocked|Boolean|Indica se o backup de dados de um aplicativo gerenciado está bloqueado. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|deviceComplianceRequired|Boolean|Indica se a compatibilidade de dispositivos é necessária. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|managedBrowserToOpenLinksRequired|Boolean|Indica se os links da Internet devem ser abertos no aplicativo de navegador gerenciado. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|saveAsBlocked|Boolean|Indica se os usuários podem usar o item de menu "Salvar como" para salvar uma cópia dos arquivos protegidos. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|periodOfflineBeforeWipeIsEnforced|Duração|A quantidade de tempo que um aplicativo pode permanecer desconectado da Internet antes que todos os dados gerenciados sejam apagados. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|pinRequired|Boolean|Indica se é necessário um pin no nível do aplicativo. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|maximumPinRetries|Int32|Número máximo de tentativas incorretas de pin antes que o aplicativo gerenciado seja apagado. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|simplePinBlocked|Boolean|Indica se simplePin está bloqueado. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|minimumPinLength|Int32|Tamanho mínimo de pin necessário para um pin no nível do aplicativo se PinRequired estiver definido como True Herdad de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|pinCharacterSet|String|Conjunto de caracteres que poderá ser usado para um pin no nível do aplicativo se PinRequired estiver definido como True. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md). Os possíveis valores são: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Duração|TimePeriod antes que o pin em todos os níveis tenha que ser redefinido, caso PinRequired esteja definido como True. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|allowedDataStorageLocations|String collection|Locais de armazenamento de dados em que um usuário pode armazenar dados gerenciados. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|contactSyncBlocked|Boolean|Indica se os contatos podem ser sincronizados com o dispositivo do usuário. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|printBlocked|Boolean|Indica se a impressão a partir de aplicativos gerenciados é permitida. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|fingerprintBlocked|Boolean|Indica se será permitido o uso do leitor de impressão digital em vez de um pin se PinRequired estiver definido como True. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|disableAppPinIfDevicePinIsSet|Boolean|Indica se o uso do pin do aplicativo será obrigatório se o pin do dispositivo estiver definido. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|minimumRequiredOsVersion|String|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|minimumWarningOsVersion|String|Versões anteriores à versão especificada resultarão em uma mensagem de aviso no aplicativo gerenciado ao acessar dados da empresa. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|minimumRequiredAppVersion|String|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|minimumWarningAppVersion|String|Versões anteriores à versão especificada resultarão em uma mensagem de aviso no aplicativo gerenciado. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|isAssigned|Boolean|Indica se a política foi implantada a grupos de inclusão ou não.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|Coleção targetedManagedAppPolicyAssignment|Propriedades de navegação para lista de grupos de inclusão e exclusão às quais a política é implantada.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.targetedManagedAppProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppProtection",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "periodOfflineBeforeAccessCheck": "String (duration)",
  "periodOnlineBeforeAccessCheck": "String (duration)",
  "allowedInboundDataTransferSources": "String",
  "allowedOutboundDataTransferDestinations": "String",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "String",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "String (duration)",
  "pinRequired": true,
  "maximumPinRetries": 1024,
  "simplePinBlocked": true,
  "minimumPinLength": 1024,
  "pinCharacterSet": "String",
  "periodBeforePinReset": "String (duration)",
  "allowedDataStorageLocations": [
    "String"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "String",
  "minimumWarningOsVersion": "String",
  "minimumRequiredAppVersion": "String",
  "minimumWarningAppVersion": "String",
  "isAssigned": true
}
```



