# <a name="deviceappmanagement-resource-type"></a>Tipo de recurso deviceAppManagement

> **Importante:** as APIs na versão / beta no Microsoft Graph estão em versão prévia e, portanto, sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de aplicativos de dispositivos.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceAppManagement](../api/intune_shared_deviceappmanagement_get.md)|Ler propriedades e relações do objeto [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).|
|[Atualizar deviceAppManagement](../api/intune_shared_deviceappmanagement_update.md)|Atualizar as propriedades de um objeto [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).|
|**Integração**|
|[Ação syncMicrosoftStoreForBusinessApps](../api/intune_shared_deviceappmanagement_syncmicrosoftstoreforbusinessapps.md)|Nenhum|Sincroniza a conta do Intune com o Microsoft Store para Empresas|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|**Nível de contratação**|
|isEnabledForMicrosoftStoreForBusiness|Booleano|Se a conta está ativada para sincronizar aplicativos do Microsoft Store para Empresa.|
|microsoftStoreForBusinessLanguage|Cadeia de caracteres|As informações sobre a localidade usada para sincronizar aplicativos do Microsoft Store para Empresas. Culturas específicas de um país/região. Os nomes dessas culturas seguem a RFC 4646 (Windows Vista e mais recentes). O formato é <languagecode2>-<country/regioncode2>, onde <languagecode2> é um código em duas letras minúsculas derivado da ISO 639-1 e <country/regioncode2> é um código em duas letras maiúsculas derivado da ISO 3166. Por exemplo, en-US para inglês (Estados Unidos) é uma cultura específica.|
|microsoftStoreForBusinessLastCompletedApplicationSyncTime|DateTimeOffset|A última vez que uma sincronização de aplicativo da Microsoft Store para Empresas foi concluída.|
|microsoftStoreForBusinessLastSuccessfulSyncDateTime|DateTimeOffset|A última vez que os aplicativos da Microsoft Store para Empresas foram sincronizados com êxito para essa conta.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|**Aplicativos**|
|mobileAppCategories|Coleção [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|As categorias dos aplicativos móveis.|
|mobileAppConfigurations|Coleção [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)|As configurações de aplicativos móveis do dispositivo gerenciado.|
|mobileApps|Coleção [mobileApp](../resources/intune_apps_mobileapp.md)|Os aplicativos móveis.|
|**Livros**|
|managedEBooks|Conjunto [managedEBook](../resources/intune_books_managedebook.md)|O livro eletrônico gerenciado.|
|**Gerenciamento de aplicativo móvel (MAM)**|
|androidManagedAppProtections|Coleção [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md)|Políticas de aplicativos gerenciados para Android.|
|defaultManagedAppProtections|Coleção [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md)|Políticas padrão de aplicativos gerenciados.|
|iosManagedAppProtections|Coleção [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md)|Políticas de aplicativos gerenciados para iOS.|
|managedAppPolicies|Coleção [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|Políticas de aplicativos gerenciados.|
|managedAppRegistrations|Coleção [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|Os registros de aplicativos gerenciados.|
|managedAppStatuses|Coleção [managedAppStatus](../resources/intune_mam_managedappstatus.md)|Os status de aplicativos gerenciados.|
|mdmWindowsInformationProtectionPolicies|Coleção [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md)|Proteção de informações do Windows para aplicativos em execução em dispositivos que estão registrados no MDM.|
|targetedManagedAppConfigurations|Coleção [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md)|Configurações direcionadas de aplicativos gerenciados.|
|windowsInformationProtectionPolicies|Coleção [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md)|Proteção de informações do Windows para aplicativos em execução em dispositivos que não estão registrados no MDM.|
|**Integração**|
|vppTokens|Coleção de [vppToken](../resources/intune_onboarding_vpptoken.md)|Lista de tokens Vpp desta organização.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.  Observe que isso é apenas um exemplo; respostas de consultas reais terão as propriedades apropriadas para o contexto.  
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "String (timestamp)",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "String",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "String (timestamp)"
}
```



