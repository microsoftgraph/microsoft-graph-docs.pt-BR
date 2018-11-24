# <a name="devicemanagement-resource-type"></a>Tipo de recurso deviceManagement

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

O recurso de deviceManagement representa um contêiner cujo conteúdo varia de acordo com o fluxo de trabalho, incluindo:  

- Eventos de auditoria  
- Termos e condições corporativas   
- Definições de configuração de dispositivo  
- Gerenciamento de dispositivo  
- Proteção de ponto de extremidade  
- Perfis de inscrição  
- Notifications  
- Detalhes, configurações e políticas de inclusão  
- Políticas de RBAC (controle) de acesso baseado em função  
- Parceiros de assistência remota  
- Parceiros de gerenciamento de extensão de telecomunicações  
- Solução de problemas de eventos  
- Resumos de proteção de informações do Windows  

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagement](../api/intune_shared_devicemanagement_get.md)|[deviceManagement](../resources/intune_shared_devicemanagement.md)|Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune_shared_devicemanagement.md).|
|[Atualizar deviceManagement](../api/intune_shared_devicemanagement_update.md)|[deviceManagement](../resources/intune_shared_devicemanagement.md)|Atualize as propriedades de um objeto [deviceManagement](../resources/intune_shared_devicemanagement.md).|
|**Inclusão**|
|[Função verifyWindowsEnrollmentAutoDiscovery](../api/intune_shared_devicemanagement_verifywindowsenrollmentautodiscovery.md)|Booliano|Ainda não documentado|
|**RBAC**|
|[Função getEffectivePermissions](../api/intune_shared_devicemanagement_geteffectivepermissions.md)|coleção [rolePermission](../resources/intune_rbac_rolepermission.md) ou conjunto de cadeia de caracteres|Recupera permissões efetivas de usuário autenticado no momento|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do dispositivo|
|**Configuração do dispositivo**|
|configurações|[deviceManagementSettings](../resources/intune_deviceconfig_devicemanagementsettings.md)|Configurações de nível da conta.|
|**Gerenciamento de dispositivos**|
|subscriptionState|Cadeia de caracteres|Estado de assinatura de gerenciamento de dispositivo móvel do locatário. Os valores possíveis são: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|
|**Inclusão**|
|intuneBrand|[intuneBrand](../resources/intune_onboarding_intunebrand.md)|intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|**Auditoria**|
|auditEvents|Conjunto [auditEvent](../resources/intune_auditing_auditevent.md)|Eventos de auditoria|
|**Termos e condições corporativas**|
|termsAndConditions|Conjunto [termsAndConditions](../resources/intune_companyterms_termsandconditions.md)|Os termos e condições associados ao gerenciamento do dispositivo da empresa.|
|**Configuração do dispositivo**|
|deviceCompliancePolicies|Coleção [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|As políticas de conformidade do dispositivo.|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)|O resumo do estado de conformidade dos dispositivos para esta conta.|
|deviceCompliancePolicySettingStateSummaries|Coleção [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)|Os estados resumidos das configurações da política de conformidade para esta conta.|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)|O resumo do estado de configuração de dispositivos para esta conta.|
|deviceConfigurations|Coleção [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|As configurações de dispositivos.|
|iosUpdateStatuses|Coleção [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md)|Os status de instalação de atualizações de software do iOS para esta conta.|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md)|O resumo do status de atualização do software.|
|**Gerenciamento de dispositivos**|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md)|Certificado de notificação por push da Apple.|
|detectedApps|Conjunto [detectedApp](../resources/intune_devices_detectedapp.md)|A lista de aplicativos detectados associados a um dispositivo.|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md)|Visão geral do dispositivo|
|managedDevices|Conjunto [managedDevice](../resources/intune_devices_manageddevice.md)|A lista de dispositivos gerenciados.|
|**Registro**|
|importedWindowsAutopilotDeviceIdentities|Coleção [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)|Coleção de dispositivos do Windows AutoPilot importados.|
|importedWindowsAutopilotDeviceIdentityUploads|coleção [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)|Coleção de piloto automático do Windows carregar de dispositivos.|
|**Notifications**|
|notificationMessageTemplates|Conjunto [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md)|Os modelos de mensagens de notificação.|
|**Inclusão**|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|As configurações de acesso condicional do Exchange no local. O acesso condicional no local exigirá que os dispositivos sejam registrados e estejam em conformidade para o acesso ao email|
|deviceCategories|Coleção [deviceCategory](../resources/intune_shared_devicecategory.md)|A lista de categorias de dispositivo com o locatário.|
|deviceEnrollmentConfigurations|Coleção [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)|A lista de configurações de registro de dispositivos|
|deviceManagementPartners|Coleção [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)|A lista de Parceiros de gerenciamento de dispositivos configurados pelo locatário.|
|exchangeConnectors|Coleção [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md)|A lista dos Conectores do Exchange configurados pelo locatário.|
|mobileThreatDefenseConnectors|Coleção [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md)|A lista dos conectores de defesa contra ameaças móveis configurados pelo locatário.|
|**RBAC**|
|resourceOperations|Conjunto [resourceOperation](../resources/intune_rbac_resourceoperation.md)|As operações de recurso.|
|roleAssignments|Conjunto [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md)|As atribuições da função|
|roleDefinitions|Conjunto [roleDefinition](../resources/intune_rbac_roledefinition.md)|As definições da função.|
|**Assistência remota**|
|remoteAssistancePartners|Conjunto [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)|Os parceiros de assistência remota.|
|**Gerenciamento de despesas de telecomunicações**|
|telecomExpenseManagementPartners|Conjunto [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md)|Os parceiros de gerenciamento de despesas de telecomunicações.|
|**Solução de problemas**|
|troubleshootingEvents|Conjunto [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)|A lista de eventos de solução de problemas para o locatário.|
|**Proteção de informações do Windows**|
|windowsInformationProtectionAppLearningSummaries|Conjunto [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)|Os resumos de aprendizagem de aplicativos da proteção de informações do Windows.|
|windowsInformationProtectionNetworkLearningSummaries|Conjunto [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)|Os resumos de aprendizagem de redes da proteção de informações do Windows.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "intuneBrand": {"@odata.type": "microsoft.graph.intuneBrand"},
  "subscriptionState": "String",
  "settings": {"@odata.type": "microsoft.graph.deviceManagementSettings"}
}
```



