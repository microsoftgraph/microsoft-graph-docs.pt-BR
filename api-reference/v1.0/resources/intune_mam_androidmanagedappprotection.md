# <a name="androidmanagedappprotection-resource-type"></a>Tipo de recurso androidManagedAppProtection

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Política usada para definir configurações de gerenciamento detalhadas direcionadas a grupos de segurança específicos e para um conjunto especificado de aplicativos em um dispositivo Android

Herda de [targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar androidManagedAppProtections](../api/intune_mam_androidmanagedappprotection_list.md)|Coleção [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md)|Listar propriedades e relações dos objetos [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md).|
|[Obter androidManagedAppProtection](../api/intune_mam_androidmanagedappprotection_get.md)|[androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md)|Ler propriedades e relações do objeto [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md).|
|[Criar androidManagedAppProtection](../api/intune_mam_androidmanagedappprotection_create.md)|[androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md)|Cria um novo objeto [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md).|
|[Excluir androidManagedAppProtection](../api/intune_mam_androidmanagedappprotection_delete.md)|Nenhum|Excluir um [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md).|
|[Atualizar androidManagedAppProtection](../api/intune_mam_androidmanagedappprotection_update.md)|[androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md)|Atualizar as propriedades de um objeto [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome de exibição da política. Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|description|Cadeia de caracteres|A descrição da política. Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|createdDateTime|DateTimeOffset|A data e a hora da criação da política. Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|Última vez em que a política foi modificada. Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|version|Cadeia de caracteres|Versão da entidade. Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|periodOfflineBeforeAccessCheck|Duração|Período após o qual o acesso é verificado quando o dispositivo não está conectado à Internet. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|periodOnlineBeforeAccessCheck|Duração|Período após o qual o acesso é verificado quando o dispositivo está conectado à Internet. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|allowedInboundDataTransferSources|Cadeia de caracteres|Fontes dos quais os dados podem ser transferidos. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md). Os possíveis valores são: `allApps`, `managedApps`, `none`.|
|allowedOutboundDataTransferDestinations|Cadeia de caracteres|Destinos para os quais os dados podem ser transferidos. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md). Os possíveis valores são: `allApps`, `managedApps`, `none`.|
|organizationalCredentialsRequired|Booliano|Indica se as credenciais organizacionais são obrigatórias para o uso do aplicativo. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|allowedOutboundClipboardSharingLevel|Cadeia de caracteres|O nível em que a área de transferência pode ser compartilhada entre os aplicativos no dispositivo gerenciado. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md). Os possíveis valores são: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|dataBackupBlocked|Booliano|Indica se o backup de dados de um aplicativo gerenciado está bloqueado. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|deviceComplianceRequired|Booliano|Indica se a compatibilidade de dispositivos é necessária. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|managedBrowserToOpenLinksRequired|Booliano|Indica se os links da Internet devem ser abertos no aplicativo de navegador gerenciado. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|saveAsBlocked|Booliano|Indica se os usuários podem usar o item de menu "Salvar como" para salvar uma cópia dos arquivos protegidos. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|periodOfflineBeforeWipeIsEnforced|Duração|A quantidade de tempo que um aplicativo pode permanecer desconectado da Internet antes que todos os dados gerenciados sejam apagados. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|pinRequired|Booliano|Indica se é necessário um pin no nível do aplicativo. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|maximumPinRetries|Int32|Número máximo de tentativas incorretas de pin antes que o aplicativo gerenciado seja apagado. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|simplePinBlocked|Booliano|Indica se simplePin está bloqueado. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|minimumPinLength|Int32|Tamanho mínimo de pin necessário para um pin no nível do aplicativo se PinRequired estiver definido como True Herdada de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|pinCharacterSet|Cadeia de caracteres|Conjunto de caracteres que poderá ser usado para um pin no nível do aplicativo se PinRequired estiver definido como True. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md). Os possíveis valores são: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Duração|TimePeriod antes que o pin em todos os níveis tenha que ser redefinido, caso PinRequired esteja definido como True. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|allowedDataStorageLocations|Coleção String|Locais de armazenamento de dados em que um usuário pode armazenar dados gerenciados. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|contactSyncBlocked|Booliano|Indica se os contatos podem ser sincronizados com o dispositivo do usuário. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|printBlocked|Booliano|Indica se a impressão a partir de aplicativos gerenciados é permitida. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|fingerprintBlocked|Booliano|Indica se será permitido o uso do leitor de impressão digital em vez de um pin se PinRequired estiver definido como True. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|disableAppPinIfDevicePinIsSet|Booliano|Indica se o uso do pin do aplicativo será obrigatório se o pin do dispositivo estiver definido. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|minimumRequiredOsVersion|Cadeia de caracteres|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|minimumWarningOsVersion|Cadeia de caracteres|Versões anteriores à versão especificada resultarão em uma mensagem de aviso no aplicativo gerenciado. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|minimumRequiredAppVersion|Cadeia de caracteres|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|minimumWarningAppVersion|Cadeia de caracteres|Versões anteriores à versão especificada resultarão em uma mensagem de aviso no aplicativo gerenciado. Herdado de [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|isAssigned|Booliano|Indica se a política foi implantada a grupos de inclusão ou não. Herdado de [targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md)|
|screenCaptureBlocked|Booliano|Indica se um usuário gerenciado pode fazer capturas de tela dos aplicativos gerenciados|
|disableAppEncryptionIfDeviceEncryptionIsEnabled|Booliano|Quando essa configuração estiver habilitada, a criptografia no nível do aplicativo será desabilitada se a criptografia no nível do dispositivo for habilitada|
|encryptAppData|Booliano|Indica se os dados de aplicativos gerenciados devem ser criptografados|
|deployedAppCount|Int32|Contagem de aplicativos em que a política atual é implantada.|
|minimumRequiredPatchVersion|Cadeia de caracteres|Define o nível mais antigo de patch de segurança do Android necessário que um usuário pode ter para obter acesso seguro ao aplicativo.|
|minimumWarningPatchVersion|Cadeia de caracteres|Define o nível mais antigo de patch de segurança do Android recomendado que um usuário pode ter para obter acesso seguro ao aplicativo.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|Coleção [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)|Propriedades de navegação para lista de grupos de inclusão e exclusão às quais a política é implantada. Herdado de [targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md)|
|aplicativos|Coleção [managedMobileApp](../resources/intune_mam_managedmobileapp.md)|Lista de aplicativos em que a política é implantada.|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md)|Propriedade de navegação para o resumo de implantação da configuração.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedAppProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedAppProtection",
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
  "isAssigned": true,
  "screenCaptureBlocked": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "encryptAppData": true,
  "deployedAppCount": 1024,
  "minimumRequiredPatchVersion": "String",
  "minimumWarningPatchVersion": "String"
}
```



