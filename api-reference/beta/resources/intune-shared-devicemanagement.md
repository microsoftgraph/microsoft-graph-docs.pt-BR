---
title: Tipo de recurso deviceManagement
description: 'O recurso deviceManagement representa um contêiner cujo conteúdo varia de acordo com o fluxo de trabalho, incluindo:  '
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a04fd011fc1f06911fdabe5dfa69d33e7cc6d18f
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792888"
---
# <a name="devicemanagement-resource-type"></a>Tipo de recurso deviceManagement

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso deviceManagement representa um contêiner cujo conteúdo varia de acordo com o fluxo de trabalho, incluindo:  

- Configurações do Android for Work
- Eventos de auditoria
- Termos e condições corporativos 
- Perfis de registro corporativo
- Definições de configuração do dispositivo
- Configurações de intenção de dispositivo
- Gerenciamento de dispositivo
- SIM (ESIM) eletrônico
- Isolamento
- Análise de política de grupo
- Notificações
- Políticas de integração, configurações e detalhes
- Conjunto de políticas
- Política de acesso de recursos
- Acesso remoto
- Parceiros de assistência remota
- Políticas de controle de acesso baseado em função (RBAC)
- Reporting
- Parceiros de gerenciamento do expanse de telecomunicações
- Solucionando problemas de eventos
- Resumos da proteção de informações do Windows

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagement](../api/intune-shared-devicemanagement-get.md)|Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).|
|[Atualizar deviceManagement](../api/intune-shared-devicemanagement-update.md)|Atualizar as propriedades de um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).|
|**Configuração do dispositivo**|
|[ação enableLegacyPcManagement](../api/intune-shared-devicemanagement-enablelegacypcmanagement.md)|Nenhuma|Ainda não documentado|
|**Gerenciamento de dispositivos**|
|[ação sendCustomNotificationToCompanyPortal](../api/intune-shared-devicemanagement-sendcustomnotificationtocompanyportal.md)|Nenhuma|Ainda não documentado|
|**Integração**|
|[Função verifyWindowsEnrollmentAutoDiscovery](../api/intune-shared-devicemanagement-verifywindowsenrollmentautodiscovery.md)|Booliano|Ainda não documentado|
|**Controle de acesso baseado em função (RBAC)**|
|[Função getEffectivePermissions](../api/intune-shared-devicemanagement-geteffectivepermissions.md)|Conjunto [rolePermission](../resources/intune-rbac-rolepermission.md)|Recupera permissões efetivas de usuário autenticado no momento|
|[função Funçãogetrolescopetagsbyids](../api/intune-shared-devicemanagement-getrolescopetagsbyids.md)|coleção [roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Ainda não documentado|
|[função getRoleScopeTagsByResource](../api/intune-shared-devicemanagement-getrolescopetagsbyresource.md)|coleção [roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Ainda não documentado|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo associado ao dispositivo.|
|**Configuração do dispositivo**|
|intuneAccountId|Guid|ID da conta do Intune para determinado locatário|
|legacyPcManangementEnabled|Booliano|A propriedade para habilitar o gerenciamento de computador herdado não MDM gerenciado para esta conta. Essa propriedade é somente leitura.|
|maximumDepTokens|Int32|Número máximo de tokens DEP permitidos por locatário.|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|Configurações de nível da conta.|
|**Gerenciamento de dispositivos**|
|accountMoveCompletionDateTime|DateTimeOffset|A data & hora em que os dados do locatário são movidos entre o ScaleUnits.|
|adminConsent|[adminConsent](../resources/intune-devices-adminconsent.md)|Informações de consentimento do administrador.|
|deviceProtectionOverview|[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)|Visão geral da proteção de dispositivo.|
|managedDeviceCleanupSettings|[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)|Regra de limpeza de dispositivo|
|subscriptionState|[deviceManagementSubscriptionState](../resources/intune-devices-devicemanagementsubscriptionstate.md)|Estado de assinatura de gerenciamento de dispositivo móvel do locatário. Os valores possíveis são: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|
|assinaturas|[deviceManagementSubscriptions](../resources/intune-devices-devicemanagementsubscriptions.md)|Assinatura do locatário. Os possíveis valores são: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/intune-devices-windowsmalwareoverview.md)|Visão geral de malware para dispositivos Windows.|
|**Análise de política de grupo**|
|groupPolicyObjectFiles|coleção [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|Uma lista de arquivos de objeto de diretiva de grupo carregados.|
|**Integração**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.|
|**Odj**|
|domainJoinConnectors|coleção [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|Uma lista de objetos conector.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|
|:---|:---|:---|
|**Android para trabalho**|
|androidDeviceOwnerEnrollmentProfiles|coleção [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|Entidades de perfil de registro do proprietário do dispositivo Android.|
|androidForWorkAppConfigurationSchemas|Coleção [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)|Entidades do esquema de configuração do aplicativo Android for Work.|
|androidForWorkEnrollmentProfiles|Coleção [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|Entidades do perfil de registro do Android for Work.|
|androidForWorkSettings|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|A entidade singleton de configurações do Android for Work.|
|androidManagedStoreAccountEnterpriseSettings|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)|A entidade singleton de configurações corporativas da conta de repositório gerenciado Android.|
|androidManagedStoreAppConfigurationSchemas|coleção [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|Entidades de esquema de configuração do aplicativo empresarial Android.|
|**Auditoria**|
|auditEvents|Conjunto [auditEvent](../resources/intune-auditing-auditevent.md)|Eventos de auditoria|
|**Termos da empresa**|
|termsAndConditions|Conjunto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Os termos e condições associados ao gerenciamento do dispositivo da empresa.|
|**Registro corporativo**|
|enrollmentProfiles|coleção [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Os perfis de registro.|
|importedAppleDeviceIdentities|coleção [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|As identidades importadas do dispositivo Apple.|
|importedDeviceIdentities|coleção [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|As identidades de dispositivo importadas.|
|**Configuração do dispositivo**|
|advancedThreatProtectionOnboardingStateSummary|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|O estado de resumo do estado de integração ATP para esta conta.|
|cartToClassAssociations|coleção [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|O carrinho para associações de classe.|
|deviceCompliancePolicies|Coleção [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|As políticas de conformidade do dispositivo.|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|O resumo do estado de conformidade dos dispositivos para esta conta.|
|deviceCompliancePolicySettingStateSummaries|Coleção [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|Os estados resumidos das configurações da política de conformidade para esta conta.|
|deviceConfigurationConflictSummary|coleção [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Resumo das políticas em estado de conflito para esta conta.|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|O resumo do estado de configuração de dispositivos para esta conta.|
|deviceConfigurationRestrictedAppsViolations|coleção [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Violações de aplicativos restritos para esta conta.|
|deviceConfigurations|Coleção [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|As configurações de dispositivos.|
|deviceConfigurationUserStateSummaries|[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)|O resumo de estado do usuário de configuração do dispositivo para esta conta.|
|iosUpdateStatuses|Coleção [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)|Os status de instalação de atualizações de software do iOS para esta conta.|
|ndesConnectors|coleção [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|A coleção de conectores NDES para esta conta.|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|O resumo do status de atualização do software.|
|**Intenção do dispositivo**|
|tentativas|coleção [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|As tentativas de gerenciamento de dispositivo|
|settingDefinitions|coleção [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|Definições de configuração da intenção de gerenciamento de dispositivo|
|modelo|coleção [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|Os modelos disponíveis|
|categories|coleção [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|As categorias disponíveis|
|**Gerenciamento de dispositivos**|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Certificado de notificação por push da Apple.|
|dataSharingConsents|coleção [dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|O compartilhamento de dados é enviado.|
|detectedApps|Conjunto [detectedApp](../resources/intune-devices-detectedapp.md)|A lista de aplicativos detectados associados a um dispositivo.|
|deviceManagementScripts|coleção [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|A lista de scripts de gerenciamento de dispositivo associados ao locatário.|
|deviceShellScripts|coleção [deviceShellScript](../resources/intune-devices-deviceshellscript.md)|A lista de scripts do Shell de dispositivo associados ao locatário.|
|deviceHealthScripts|coleção [deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|A lista de scripts de integridade do dispositivo associados ao locatário.|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|Visão geral do dispositivo|
|managedDevices|Conjunto [managedDevice](../resources/intune-devices-manageddevice.md)|A lista de dispositivos gerenciados.|
|remoteActionAudits|coleção [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|A lista de auditorias de ação remota do dispositivo com o locatário.|
|windowsMalwareInformation|coleção [windowsmalwareinformation foram adicionadas](../resources/intune-devices-windowsmalwareinformation.md)|A lista de malwares afetados no locatário.|
|mobileAppTroubleshootingEvents|coleção [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|A Propriedade Collection de MobileAppTroubleshootingEvent.|
|userExperienceAnalyticsOverview|[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)|Visão geral da análise da experiência do usuário|
|userExperienceAnalyticsBaselines|coleção [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|Linhas de base de análise da experiência do usuário|
|userExperienceAnalyticsCategories|coleção [userExperienceAnalyticsCategory](../resources/intune-devices-userExperienceAnalyticsCategory.md)|Categorias de análise da experiência do usuário|
|userExperienceAnalyticsDevicePerformance|coleção [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|Desempenho do dispositivo de análise da experiência do usuário|
|userExperienceAnalyticsRegressionSummary|[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)|Resumo de regressão da análise da experiência do usuário|
|userExperienceAnalyticsDeviceStartupHistory|coleção [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|Histórico de inicialização do dispositivo de análise da experiência do usuário|
|userExperienceAnalyticsDeviceStartupProcesses|coleção [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|Processos de inicialização do dispositivo de análise da experiência do usuário|
|userExperienceAnalyticsDeviceStartupProcessPerformance|coleção [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)|Desempenho do processo de inicialização do dispositivo de análise de experiência do usuário|
|**Enrollmentid**|
|depOnboardingSettings|coleção [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Este conjunto de vários tokens DEP por locatário.|
|importedDeviceIdentities|coleção [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|As identidades de dispositivo importadas.|
|importedWindowsAutopilotDeviceIdentities|Coleção [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|Coleção de dispositivos do Windows AutoPilot importados.|
|windowsAutopilotDeploymentProfiles|coleção [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|Perfis de implantação do piloto automático do Windows|
|windowsAutopilotDeviceIdentities|coleção [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Coleção de identidades de dispositivo do Windows AutoPilot contidas.|
|windowsAutopilotSettings|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|As configurações da conta do Windows AutoPilot.|
|**SIM incorporado**|
|embeddedSIMActivationCodePools|coleção [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Os pools de código de ativação do SIM incorporados criados por esta conta.|
|**Isolamento**|
|managementConditions|coleção [managementCondition](../resources/intune-fencing-managementcondition.md)|As condições de gerenciamento associadas ao gerenciamento de dispositivos da empresa.|
|managementConditionStatements|coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|As instruções de condição de gerenciamento associadas ao gerenciamento de dispositivos da empresa.|
|**Análise de política de grupo**|
|groupPolicyMigrationReports|coleção [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|Uma lista de relatórios de migração de política de grupo.|
|**Notificações**|
|notificationMessageTemplates|Conjunto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Os modelos de mensagens de notificação.|
|**Integração**|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|As configurações de acesso condicional do Exchange no local. O acesso condicional no local exigirá que os dispositivos sejam registrados e estejam em conformidade para o acesso ao email|
|deviceCategories|Coleção [deviceCategory](../resources/intune-shared-devicecategory.md)|A lista de categorias de dispositivo com o locatário.|
|deviceEnrollmentConfigurations|Coleção [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|A lista de configurações de registro de dispositivos|
|deviceManagementPartners|Coleção [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|A lista de Parceiros de gerenciamento de dispositivos configurados pelo locatário.|
|exchangeConnectors|Coleção [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|A lista dos Conectores do Exchange configurados pelo locatário.|
|exchangeOnPremisesPolicies|coleção [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|A lista de políticas do Exchange no premisis configuradas pelo locatário.|
|exchangeOnPremisesPolicy|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|A política que controla o acesso de dispositivos móveis para o Exchange no local|
|mobileThreatDefenseConnectors|Coleção [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|A lista dos conectores de defesa contra ameaças móveis configurados pelo locatário.|
|**Conjunto de políticas**|
|deviceManagementScripts|coleção [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|A lista de scripts de gerenciamento de dispositivo associados ao locatário.|
|deviceConfigurations|Coleção [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|A lista de configurações de dispositivo associadas ao locatário.|
|deviceCompliancePolicies|Coleção [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|A lista de políticas de conformidade do dispositivo associadas ao locatário.|
|windowsAutopilotDeploymentProfiles|coleção [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|Perfis de implantação do piloto automático do Windows|
|deviceEnrollmentConfigurations|Coleção [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|A lista de configurações de registro de dispositivos|
|**Polcy de acesso a recursos**|
|derivedCredentials|coleção [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|Coleção de configurações de credenciais derivadas associadas à conta.|
|**Acesso remoto**|
|userPfxCertificates|coleção [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Coleção de certificados PFX associados a um usuário.|
|**Assistência remota**|
|remoteAssistancePartners|Conjunto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Os parceiros de assistência remota.|
|**Controle de acesso baseado em função (RBAC)**|
|resourceOperations|Conjunto [resourceOperation](../resources/intune-rbac-resourceoperation.md)|As operações de recurso.|
|roleAssignments|Conjunto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|As atribuições da função|
|roleDefinitions|Conjunto [roleDefinition](../resources/intune-rbac-roledefinition.md)|As definições da função.|
|roleScopeTags|coleção [roleScopeTag](../resources/intune-rbac-rolescopetag.md)|As marcas de escopo da função.|
|**Relatórios**|
|relatórios|[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)|Singleton de relatórios|
|**Atualização de software**|
|windowsFeatureUpdateProfiles|coleção [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|Uma coleção de perfis de atualização de recursos do Windows|
|**Gerenciamento de despesas de telecomunicações (tem)**|
|telecomExpenseManagementPartners|Conjunto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|Os parceiros de gerenciamento de despesas de telecomunicações.|
|**Solução de Problemas**|
|troubleshootingEvents|Conjunto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|A lista de eventos de solução de problemas para o locatário.|
|**Proteção de Informações do Windows**|
|Navegaçãointunebrandingprofiles|coleção [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Perfis de identidade visual do Intune direcionados para grupos do AAD|
|windowsInformationProtectionAppLearningSummaries|Conjunto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)|Os resumos de aprendizagem de aplicativos da proteção de informações do Windows.|
|windowsInformationProtectionNetworkLearningSummaries|Conjunto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)|Os resumos de aprendizagem de redes da proteção de informações do Windows.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "subscriptionState": "String"
}
```



