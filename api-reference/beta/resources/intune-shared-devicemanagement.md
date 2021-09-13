---
title: Tipo de recurso deviceManagement
description: 'O recurso deviceManagement representa um contêiner cujo conteúdo varia de acordo com o fluxo de trabalho, incluindo:  '
ms.localizationpriority: medium
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c1562f91f3728830f4d220063651d03823c052eb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039130"
---
# <a name="devicemanagement-resource-type"></a>Tipo de recurso deviceManagement

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso deviceManagement representa um contêiner cujo conteúdo varia de acordo com o fluxo de trabalho, incluindo:  

- Configurações do Android for Work
- Eventos de auditoria
- Termos e condições corporativos 
- Perfis de registro corporativo
- Configurações de dispositivo
- Configurações de intenção de dispositivo
- Gerenciamento de dispositivo
- SIM Eletrônico (ESIM)
- Esgrima
- Análise de Política de Grupo
- Notificações
- Políticas, configurações e detalhes de integração
- Conjunto de Políticas
- Política de Acesso a Recursos
- Acesso remoto
- Parceiros de assistência remota
- Políticas de controle de acesso baseado em função (RBAC)
- Relatórios
- Parceiros de gerenciamento de expansão de telecomunicações
- Solução de problemas de eventos
- Windows Resumos da Proteção de Informações

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagement](../api/intune-shared-devicemanagement-get.md)|Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).|
|[Atualizar deviceManagement](../api/intune-shared-devicemanagement-update.md)|Atualizar as propriedades de um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).|
|**Configuração do dispositivo**|
|[ação enableLegacyPcManagement](../api/intune-shared-devicemanagement-enablelegacypcmanagement.md)|Nenhuma|Ainda não documentado|
|**Gerenciamento de dispositivo**|
|[ação sendCustomNotificationToCompanyPortal](../api/intune-shared-devicemanagement-sendcustomnotificationtocompanyportal.md)|Nenhuma|Ainda não documentado|
|**Integração**|
|[Função verifyWindowsEnrollmentAutoDiscovery](../api/intune-shared-devicemanagement-verifywindowsenrollmentautodiscovery.md)|Booliano|Ainda não documentado|
|**Controle de acesso baseado em função (RBAC)**|
|[Função getEffectivePermissions](../api/intune-shared-devicemanagement-geteffectivepermissions.md)|Conjunto [rolePermission](../resources/intune-rbac-rolepermission.md)|Recupera permissões efetivas de usuário autenticado no momento|
|[Função getRoleScopeTagsByIds](../api/intune-shared-devicemanagement-getrolescopetagsbyids.md)|[Coleção roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Ainda não documentado|
|[Função getRoleScopeTagsByResource](../api/intune-shared-devicemanagement-getrolescopetagsbyresource.md)|[Coleção roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Ainda não documentado|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo associado ao dispositivo.|
|**Configuração do dispositivo**|
|intuneAccountId|Guid|ID da conta do Intune para determinado locatário|
|legacyPcManangementEnabled|Boleano|A propriedade para habilitar o gerenciamento de computador herdado não-MDM gerenciado para essa conta. Essa propriedade é somente leitura.|
|maximumDepTokens|Int32|Número máximo de tokens DEP permitidos por locatário.|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|Configurações de nível da conta.|
|**Gerenciamento de dispositivo**|
|accountMoveCompletionDateTime|DateTimeOffset|A data & hora em que os dados do locatário foram movidos entre as unidades de escala.|
|adminConsent|[adminConsent](../resources/intune-devices-adminconsent.md)|Informações de consentimento do administrador.|
|deviceProtectionOverview|[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)|Visão geral da proteção do dispositivo.|
|managedDeviceCleanupSettings|[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)|Regra de limpeza de dispositivo|
|subscriptionState|[deviceManagementSubscriptionState](../resources/intune-devices-devicemanagementsubscriptionstate.md)|Estado de assinatura de gerenciamento de dispositivo móvel do locatário. Os valores possíveis são: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|
|assinaturas|[deviceManagementSubscriptions](../resources/intune-devices-devicemanagementsubscriptions.md)|Assinatura do locatário. Os possíveis valores são: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/intune-devices-windowsmalwareoverview.md)|Visão geral do malware para dispositivos windows.|
|**Análise de Política de Grupo**|
|groupPolicyObjectFiles|[coleção groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|Uma lista de arquivos de Objeto de Política de Grupo carregados.|
|**Integração**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.|
|**Odj**|
|domainJoinConnectors|[Coleção deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|Uma lista de objetos do conector.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|
|:---|:---|:---|
|**Android for Work**|
|androidDeviceOwnerEnrollmentProfiles|[coleção androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|Entidades de perfil de registro do proprietário do dispositivo Android.|
|androidForWorkAppConfigurationSchemas|Coleção [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)|Entidades do esquema de configuração do aplicativo Android for Work.|
|androidForWorkEnrollmentProfiles|Coleção [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|Entidades do perfil de registro do Android for Work.|
|androidForWorkSettings|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|A entidade singleton de configurações do Android for Work.|
|androidManagedStoreAccountEnterpriseSettings|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)|A entidade de configurações corporativas de conta gerenciada do Android singleton.|
|androidManagedStoreAppConfigurationSchemas|[coleção androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|Entidades Enterprise esquema de configuração de aplicativos do Android.|
|**Auditoria**|
|auditEvents|Conjunto [auditEvent](../resources/intune-auditing-auditevent.md)|Eventos de auditoria|
|**Termos da empresa**|
|termsAndConditions|Conjunto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Os termos e condições associados ao gerenciamento do dispositivo da empresa.|
|**Políticas de Configuração**|
|configurationPolicies|[Coleção deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-deviceManagementConfigurationPolicy.md)|Lista de todas as políticas de configuração|
|configurationSettings|[Coleção deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-deviceManagementConfigurationSettingDefinition.md)|Lista de todos os ConfigurationSettings|
|configurationCategories|[Coleção deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-deviceManagementConfigurationCategory.md)|Lista de todas as Categorias de Configuração|
|**Registro corporativo**|
|enrollmentProfiles|[Coleção enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Os perfis de registro.|
|importedAppleDeviceIdentities|[Coleção importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|As identidades de dispositivo Apple importadas.|
|importedDeviceIdentities|[Coleção importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|As identidades dos dispositivos importados.|
|**Configuração do dispositivo**|
|advancedThreatProtectionOnboardingStateSummary|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|O estado de resumo do estado de integração da ATP para essa conta.|
|cartToClassAssociations|[Coleção cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Associações de carrinho para classe.|
|deviceCompliancePolicies|Coleção [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|As políticas de conformidade do dispositivo.|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|O resumo do estado de conformidade dos dispositivos para esta conta.|
|deviceCompliancePolicySettingStateSummaries|Coleção [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|Os estados resumidos das configurações da política de conformidade para esta conta.|
|deviceConfigurationConflictSummary|[Coleção deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Resumo das políticas em estado de conflito para essa conta.|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|O resumo do estado de configuração de dispositivos para esta conta.|
|deviceConfigurationRestrictedAppsViolations|[Coleção restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Violações de aplicativos restritos para essa conta.|
|deviceConfigurations|Coleção [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|As configurações de dispositivos.|
|deviceConfigurationUserStateSummaries|[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)|O resumo do estado do usuário de configuração do dispositivo para essa conta.|
|iosUpdateStatuses|Coleção [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)|Os status de instalação de atualizações de software do iOS para esta conta.|
|ndesConnectors|[Coleção ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|A coleção de conectores Ndes para essa conta.|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|O resumo do status de atualização do software.|
|**Intenção do dispositivo**|
|intents|[Coleção deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|As intenções de gerenciamento de dispositivo|
|settingDefinitions|[Coleção deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|Definições de configuração de intenção de gerenciamento de dispositivos|
|templates|[Coleção deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|Os modelos disponíveis|
|categories|[Coleção deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|As categorias disponíveis|
|**Gerenciamento de dispositivo**|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Certificado de notificação por push da Apple.|
|dataSharingConsents|[Coleção dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Consentimentos de compartilhamento de dados.|
|detectedApps|Conjunto [detectedApp](../resources/intune-devices-detectedapp.md)|A lista de aplicativos detectados associados a um dispositivo.|
|deviceManagementScripts|[Coleção deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|A lista de scripts de gerenciamento de dispositivos associados ao locatário.|
|deviceShellScripts|[Coleção deviceShellScript](../resources/intune-devices-deviceshellscript.md)|A lista de scripts de shell de dispositivo associados ao locatário.|
|deviceHealthScripts|[Coleção deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|A lista de scripts de saúde do dispositivo associados ao locatário.|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|Visão geral do dispositivo|
|managedDevices|Conjunto [managedDevice](../resources/intune-devices-manageddevice.md)|A lista de dispositivos gerenciados.|
|remoteActionAudits|[Coleção remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|A lista de auditorias de ação remota do dispositivo com o locatário.|
|windowsMalwareInformation|[Coleção windowsMalwareInformation](../resources/intune-devices-windowsmalwareinformation.md)|A lista de malware afetados no locatário.|
|mobileAppTroubleshootingEvents|[Coleção mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|A propriedade collection de MobileAppTroubleshootingEvent.|
|userExperienceAnalyticsOverview|[userExperienceAnalyticsOverview](../resources/userExperienceAnalyticsOverview.md)|Visão geral da análise da experiência do usuário|
|userExperienceAnalyticsBaselines|[Coleção userExperienceAnalyticsBaseline](../resources/userExperienceAnalyticsBaseline.md)|Linhas de base de análise de experiência do usuário|
|userExperienceAnalyticsCategories|[coleção userExperienceAnalyticsCategory](../resources/userExperienceAnalyticsCategory.md)|Categorias de análise de experiência do usuário|
|userExperienceAnalyticsDevicePerformance|[coleção userExperienceAnalyticsDevicePerformance](../resources/userExperienceAnalyticsDevicePerformance.md)|Desempenho do dispositivo de análise de experiência do usuário|
|userExperienceAnalyticsRegressionSummary|[userExperienceAnalyticsRegressionSummary](../resources/userExperienceAnalyticsRegressionSummary.md)|Resumo de regressão de análise de experiência do usuário|
|userExperienceAnalyticsDeviceStartupHistory|[coleção userExperienceAnalyticsDeviceStartupHistory](../resources/userExperienceAnalyticsDeviceStartupHistory.md)|Histórico de inicialização do dispositivo de análise de experiência do usuário|
|userExperienceAnalyticsDeviceStartupProcesses|[Coleção userExperienceAnalyticsDeviceStartupProcess](../resources/userExperienceAnalyticsDeviceStartupProcess.md)|Processos de inicialização do dispositivo de análise de experiência do usuário|
|userExperienceAnalyticsDeviceStartupProcessPerformance|[coleção userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/userExperienceAnalyticsDeviceStartupProcessPerformance.md)|Desempenho do processo de inicialização do dispositivo de análise de experiência do usuário|
|**Inscrição**|
|depOnboardingSettings|[Coleção depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Essas coleções de vários tokens DEP por locatário.|
|importedDeviceIdentities|[Coleção importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|As identidades dos dispositivos importados.|
|importedWindowsAutopilotDeviceIdentities|Coleção [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|Coleção de dispositivos do Windows AutoPilot importados.|
|windowsAutopilotDeploymentProfiles|[Coleção windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|Windows de implantação piloto automático|
|windowsAutopilotDeviceIdentities|[Coleção windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|As Windows do dispositivo autopilot continham coleção.|
|windowsAutopilotSettings|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|As Windows configurações da conta do piloto automático.|
|**SIM incorporado**|
|embeddedSIMActivationCodePools|[Coleção embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Os pools de código de ativação de SIM incorporados criados por essa conta.|
|**Esgrima**|
|managementConditions|[coleção managementCondition](../resources/intune-fencing-managementcondition.md)|As condições de gerenciamento associadas ao gerenciamento de dispositivos da empresa.|
|managementConditionStatements|[coleção managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|As instruções de condição de gerenciamento associadas ao gerenciamento de dispositivos da empresa.|
|**Análise de Política de Grupo**|
|groupPolicyMigrationReports|[coleção groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|Uma lista de relatórios de migração da Política de Grupo.|
|**MicrosoftTunnel**|
|microsoftTunnelConfigurations|[coleção microsoftTunnelConfiguration](../resources/intune-mstunnel-microsoftTunnelConfiguration.md)|Coleção de configurações do MicrosoftTunnelConfiguration associadas à conta.|
|microsoftTunnelSites|[Coleção microsoftTunnelSite](../resources/intune-mstunnel-microsoftTunnelSite.md)|Coleção de configurações do MicrosoftTunnelSite associadas à conta.|
|**Notificações**|
|notificationMessageTemplates|Conjunto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Os modelos de mensagens de notificação.|
|**Integração**|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|As configurações de acesso condicional do Exchange no local. O acesso condicional no local exigirá que os dispositivos sejam registrados e estejam em conformidade para o acesso ao email|
|deviceCategories|Coleção [deviceCategory](../resources/intune-shared-devicecategory.md)|A lista de categorias de dispositivo com o locatário.|
|deviceEnrollmentConfigurations|Coleção [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|A lista de configurações de registro de dispositivos|
|deviceManagementPartners|Coleção [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|A lista de Parceiros de gerenciamento de dispositivos configurados pelo locatário.|
|exchangeConnectors|Coleção [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|A lista dos Conectores do Exchange configurados pelo locatário.|
|exchangeOnPremisesPolicies|[Coleção deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|A lista de Exchange políticas on-premisis configuradas pelo locatário.|
|exchangeOnPremisesPolicy|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|A política que controla o acesso de dispositivo móvel Exchange local|
|mobileThreatDefenseConnectors|Coleção [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|A lista dos conectores de defesa contra ameaças móveis configurados pelo locatário.|
|**Conjunto de Políticas**|
|deviceManagementScripts|[Coleção deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|A lista de scripts de gerenciamento de dispositivos associados ao locatário.|
|deviceConfigurations|Coleção [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|A lista de configurações de dispositivos associadas ao locatário.|
|deviceCompliancePolicies|Coleção [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|A lista de políticas de conformidade de dispositivos associadas ao locatário.|
|windowsAutopilotDeploymentProfiles|[Coleção windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|Windows de implantação piloto automático|
|deviceEnrollmentConfigurations|Coleção [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|A lista de configurações de registro de dispositivos|
|**Política de Acesso a Recursos**|
|derivedCredentials|[Coleção deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|Coleção de configurações de credenciais derivadas associadas à conta.|
|**Acesso remoto**|
|userPfxCertificates|[Coleção userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Coleção de certificados PFX associados a um usuário.|
|**Assistência remota**|
|remoteAssistancePartners|Conjunto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Os parceiros de assistência remota.|
|**Controle de acesso baseado em função (RBAC)**|
|resourceOperations|Conjunto [resourceOperation](../resources/intune-rbac-resourceoperation.md)|As operações de recurso.|
|roleAssignments|Conjunto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|As atribuições da função|
|roleDefinitions|Conjunto [roleDefinition](../resources/intune-rbac-roledefinition.md)|As definições da função.|
|roleScopeTags|[Coleção roleScopeTag](../resources/intune-rbac-rolescopetag.md)|As Marcas de Escopo de Função.|
|**Relatórios**|
|reports|[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)|Singleton de relatórios|
|**Atualização de Software**|
|windowsFeatureUpdateProfiles|[Coleção windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|Uma coleção de perfis de atualização de recursos do Windows|
|**Gerenciamento de despesas de telecomunicações (TEM)**|
|telecomExpenseManagementPartners|Conjunto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|Os parceiros de gerenciamento de despesas de telecomunicações.|
|**Solução de Problemas**|
|troubleshootingEvents|Conjunto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|A lista de eventos de solução de problemas para o locatário.|
|**Proteção de Informações do Windows**|
|intuneBrandingProfiles|[Coleção intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Perfis de identidade visual do Intune direcionados a grupos do AAD|
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



