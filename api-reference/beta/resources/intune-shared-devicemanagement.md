---
title: Tipo de recurso deviceManagement
description: 'O recurso deviceManagement representa um contêiner cujo conteúdo varia de acordo com o fluxo de trabalho, incluindo:  '
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f07febfdaee04e2baf57f5403cfc07e2de13af10
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858307"
---
# <a name="devicemanagement-resource-type"></a>Tipo de recurso deviceManagement

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso deviceManagement representa um contêiner cujo conteúdo varia de acordo com o fluxo de trabalho, incluindo:  

- Configurações do Android for Work
- Eventos de auditoria
- Termos e condições corporativos 
- Perfis de registro corporativo
- Definições de configuração do dispositivo
- Configurações de intenção do dispositivo
- Gerenciamento de dispositivo
- ESIM (Electronic SIM)
- Esgrima
- Política de Grupo Analytics
- Notificações
- Políticas, configurações e detalhes de integração
- Conjunto de Políticas
- Política de Acesso a Recursos
- Acesso remoto
- Parceiros de assistência remota
- Políticas de RBAC (controle de acesso baseado em função)
- Relatórios
- Parceiros de gerenciamento de expansão de telecomunicações
- Solução de problemas de eventos
- Windows Proteção de Informações resumos

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
|**RBAC (controle de acesso baseado em função)**|
|[Função getEffectivePermissions](../api/intune-shared-devicemanagement-geteffectivepermissions.md)|Conjunto [rolePermission](../resources/intune-rbac-rolepermission.md)|Recupera permissões efetivas de usuário autenticado no momento|
|[Função getRoleScopeTagsByIds](../api/intune-shared-devicemanagement-getrolescopetagsbyids.md)|[Coleção roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Ainda não documentado|
|[Função getRoleScopeTagsByResource](../api/intune-shared-devicemanagement-getrolescopetagsbyresource.md)|[Coleção roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Ainda não documentado|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo associado ao dispositivo.|
|**Configuração do dispositivo**|
|intuneAccountId|Guid|Intune ID da conta para determinado locatário|
|legacyPcManangementEnabled|Booliano|A propriedade para habilitar o gerenciamento de pc herdado gerenciado não MDM para essa conta. Essa propriedade é somente leitura.|
|maximumDepTokens|Int32|Número máximo de tokens DEP permitidos por locatário.|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|Configurações de nível da conta.|
|**Gerenciamento de dispositivo**|
|accountMoveCompletionDateTime|DateTimeOffset|A data & hora em que os dados do locatário foram movidos entre as unidades de escala.|
|adminConsent|[adminConsent](../resources/intune-devices-adminconsent.md)|Administração informações de consentimento.|
|deviceProtectionOverview|[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)|Visão geral da proteção do dispositivo.|
|managedDeviceCleanupSettings|[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)|Regra de limpeza do dispositivo|
|subscriptionState|[deviceManagementSubscriptionState](../resources/intune-devices-devicemanagementsubscriptionstate.md)|Estado de assinatura de gerenciamento de dispositivo móvel do locatário. Os valores possíveis são: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|
|assinaturas|[deviceManagementSubscriptions](../resources/intune-devices-devicemanagementsubscriptions.md)|Assinatura do locatário. Os possíveis valores são: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/intune-devices-windowsmalwareoverview.md)|Visão geral de malware para dispositivos Windows.|
|**Política de Grupo Analytics**|
|groupPolicyObjectFiles|[coleção groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|Uma lista de arquivos Política de Grupo objeto carregados.|
|**Integração**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.|
|**Odj**|
|domainJoinConnectors|[Coleção deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|Uma lista de objetos do conector.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|
|:---|:---|:---|
|**Android for Work**|
|androidDeviceOwnerEnrollmentProfiles|[coleção androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|Android do perfil de registro do proprietário do dispositivo.|
|androidForWorkAppConfigurationSchemas|Coleção [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)|Entidades do esquema de configuração do aplicativo Android for Work.|
|androidForWorkEnrollmentProfiles|Coleção [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|Entidades do perfil de registro do Android for Work.|
|androidForWorkSettings|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|A entidade singleton de configurações do Android for Work.|
|androidManagedStoreAccountEnterpriseSettings|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)|A entidade de configurações corporativas Android conta de repositório gerenciado singleton.|
|androidManagedStoreAppConfigurationSchemas|[coleção androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|Android Enterprise de esquema de configuração de aplicativo.|
|**Auditoria**|
|auditEvents|Conjunto [auditEvent](../resources/intune-auditing-auditevent.md)|Eventos de auditoria|
|**Termos da empresa**|
|termsAndConditions|Conjunto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Os termos e condições associados ao gerenciamento do dispositivo da empresa.|
|**Políticas de configuração**|
|configurationPolicies|[Coleção deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-deviceManagementConfigurationPolicy.md)|Lista de todas as políticas de configuração|
|Configurationsettings|[Coleção deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-deviceManagementConfigurationSettingDefinition.md)|Lista de todos os ConfigurationSettings|
|configurationCategories|[Coleção deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-deviceManagementConfigurationCategory.md)|Lista de todas as categorias de configuração|
|**Registro corporativo**|
|enrollmentProfiles|[coleção enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Os perfis de registro.|
|importedAppleDeviceIdentities|[Coleção importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|As identidades de dispositivo apple importadas.|
|importedDeviceIdentities|[coleção importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|As identidades de dispositivo importadas.|
|**Configuração do dispositivo**|
|advancedThreatProtectionOnboardingStateSummary|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|O estado de resumo do estado de integração do ATP para essa conta.|
|cartToClassAssociations|[coleção cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|O carrinho para associações de classe.|
|deviceCompliancePolicies|Coleção [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|As políticas de conformidade do dispositivo.|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|O resumo do estado de conformidade dos dispositivos para esta conta.|
|deviceCompliancePolicySettingStateSummaries|Coleção [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|Os estados resumidos das configurações da política de conformidade para esta conta.|
|deviceConfigurationConflictSummary|[Coleção deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Resumo das políticas em estado de conflito para essa conta.|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|O resumo do estado de configuração de dispositivos para esta conta.|
|deviceConfigurationRestrictedAppsViolations|[Coleção restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Violações de aplicativos restritos para essa conta.|
|deviceConfigurations|Coleção [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|As configurações de dispositivos.|
|deviceConfigurationUserStateSummaries|[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)|O resumo do estado do usuário de configuração do dispositivo para essa conta.|
|iosUpdateStatuses|Coleção [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)|Os status de instalação de atualizações de software do iOS para esta conta.|
|ndesConnectors|[Coleção ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|A coleção de conectores do Ndes para essa conta.|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|O resumo do status de atualização do software.|
|**Intenção do dispositivo**|
|intenções|[Coleção deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|As intenções de gerenciamento de dispositivo|
|settingDefinitions|[Coleção deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|As definições de configuração de intenção de gerenciamento de dispositivo|
|Modelos|[Coleção deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|Os modelos disponíveis|
|categories|[Coleção deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|As categorias disponíveis|
|**Gerenciamento de dispositivo**|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Certificado de notificação por push da Apple.|
|dataSharingConsents|[Coleção dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Consentimentos de compartilhamento de dados.|
|detectedApps|Conjunto [detectedApp](../resources/intune-devices-detectedapp.md)|A lista de aplicativos detectados associados a um dispositivo.|
|deviceManagementScripts|[Coleção deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|A lista de scripts de gerenciamento de dispositivos associados ao locatário.|
|deviceShellScripts|[coleção deviceShellScript](../resources/intune-devices-deviceshellscript.md)|A lista de scripts de shell de dispositivo associados ao locatário.|
|deviceHealthScripts|[Coleção deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|A lista de scripts de integridade do dispositivo associados ao locatário.|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|Visão geral do dispositivo|
|managedDevices|Conjunto [managedDevice](../resources/intune-devices-manageddevice.md)|A lista de dispositivos gerenciados.|
|remoteActionAudits|[Coleção remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|A lista de auditorias de ação remota do dispositivo com o locatário.|
|windowsMalwareInformation|[coleção windowsMalwareInformation](../resources/intune-devices-windowsmalwareinformation.md)|A lista de malwares afetados no locatário.|
|mobileAppTroubleshootingEvents|[coleção mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|A propriedade de coleção de MobileAppTroubleshootingEvent.|
|userExperienceAnalyticsOverview|[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)|Visão geral da análise da experiência do usuário|
|userExperienceAnalyticsBaselines|[coleção userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|Linhas de base de análise da experiência do usuário|
|userExperienceAnalyticsCategories|[coleção userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|Categorias de análise da experiência do usuário|
|userExperienceAnalyticsDevicePerformance|[coleção userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|Desempenho do dispositivo de análise da experiência do usuário|
|userExperienceAnalyticsRegressionSummary|[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)|Resumo da regressão de análise da experiência do usuário|
|userExperienceAnalyticsDeviceStartupHistory|[coleção userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|Histórico de inicialização do dispositivo de análise da experiência do usuário|
|userExperienceAnalyticsDeviceStartupProcesses|[coleção userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|Processos de inicialização do dispositivo de análise da experiência do usuário|
|userExperienceAnalyticsDeviceStartupProcessPerformance|[coleção userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)|Desempenho do processo de inicialização do dispositivo de análise da experiência do usuário|
|userExperienceAnalyticsScoreHistory|[coleção userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|Histórico de pontuação do dispositivo de análise da experiência do usuário|
|**Registro**|
|depOnboardingSettings|[Coleção depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Essas coleções de vários tokens DEP por locatário.|
|importedDeviceIdentities|[coleção importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|As identidades de dispositivo importadas.|
|importedWindowsAutopilotDeviceIdentities|Coleção [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|Coleção de dispositivos do Windows AutoPilot importados.|
|windowsAutopilotDeploymentProfiles|[coleção windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|Windows de implantação piloto automático|
|windowsAutopilotDeviceIdentities|[coleção windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|As Windows de dispositivo do autopilot continham a coleção.|
|windowsAutopilotSettings|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|As configurações Windows conta do autopilot.|
|**SIM inserido**|
|embeddedSIMActivationCodePools|[Coleção embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Os pools de códigos de ativação do SIM inseridos criados por essa conta.|
|**Esgrima**|
|managementConditions|[coleção managementCondition](../resources/intune-fencing-managementcondition.md)|As condições de gerenciamento associadas ao gerenciamento de dispositivos da empresa.|
|managementConditionStatements|[coleção managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|As instruções de condição de gerenciamento associadas ao gerenciamento de dispositivos da empresa.|
|**Política de Grupo Analytics**|
|groupPolicyMigrationReports|[Coleção groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|Uma lista de relatórios Política de Grupo migração.|
|**MicrosoftTunnel**|
|microsoftTunnelConfigurations|[coleção microsoftTunnelConfiguration](../resources/intune-mstunnel-microsoftTunnelConfiguration.md)|Coleção de configurações de MicrosoftTunnelConfiguration associadas à conta.|
|microsoftTunnelSites|[coleção microsoftTunnelSite](../resources/intune-mstunnel-microsoftTunnelSite.md)|Coleção de configurações do MicrosoftTunnelSite associadas à conta.|
|**Notificações**|
|notificationMessageTemplates|Conjunto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Os modelos de mensagens de notificação.|
|**Integração**|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|As configurações de acesso condicional do Exchange no local. O acesso condicional no local exigirá que os dispositivos sejam registrados e estejam em conformidade para o acesso ao email|
|deviceCategories|Coleção [deviceCategory](../resources/intune-shared-devicecategory.md)|A lista de categorias de dispositivo com o locatário.|
|deviceEnrollmentConfigurations|Coleção [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|A lista de configurações de registro de dispositivos|
|deviceManagementPartners|Coleção [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|A lista de Parceiros de gerenciamento de dispositivos configurados pelo locatário.|
|exchangeConnectors|Coleção [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|A lista dos Conectores do Exchange configurados pelo locatário.|
|exchangeOnPremisesPolicies|[Coleção deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|A lista de Exchange no Premisis configuradas pelo locatário.|
|exchangeOnPremisesPolicy|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|A política que controla o acesso de dispositivo móvel Exchange local|
|mobileThreatDefenseConnectors|Coleção [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|A lista dos conectores de defesa contra ameaças móveis configurados pelo locatário.|
|**Conjunto de Políticas**|
|deviceManagementScripts|[Coleção deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|A lista de scripts de gerenciamento de dispositivos associados ao locatário.|
|deviceConfigurations|Coleção [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|A lista de configurações de dispositivo associadas ao locatário.|
|deviceCompliancePolicies|Coleção [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|A lista de políticas de conformidade do dispositivo associadas ao locatário.|
|windowsAutopilotDeploymentProfiles|[coleção windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|Windows de implantação piloto automático|
|deviceEnrollmentConfigurations|Coleção [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|A lista de configurações de registro de dispositivos|
|**Política de Acesso a Recursos**|
|derivedCredentials|[Coleção deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|Coleção de configurações de credenciais derivadas associadas à conta.|
|**Acesso remoto**|
|userPfxCertificates|[coleção userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Coleção de certificados PFX associados a um usuário.|
|**Assistência remota**|
|remoteAssistancePartners|Conjunto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Os parceiros de assistência remota.|
|**RBAC (controle de acesso baseado em função)**|
|resourceOperations|Conjunto [resourceOperation](../resources/intune-rbac-resourceoperation.md)|As operações de recurso.|
|roleAssignments|Conjunto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|As atribuições da função|
|roleDefinitions|Conjunto [roleDefinition](../resources/intune-rbac-roledefinition.md)|As definições da função.|
|roleScopeTags|[Coleção roleScopeTag](../resources/intune-rbac-rolescopetag.md)|As marcas de escopo da função.|
|**Relatórios**|
|Relatórios|[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)|Singleton de relatórios|
|**Atualização de Software**|
|windowsFeatureUpdateProfiles|[coleção windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|Uma coleção de perfis de atualização de recursos do Windows|
|**TEM (Gerenciamento de Despesas de Telecomunicações)**|
|telecomExpenseManagementPartners|Conjunto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|Os parceiros de gerenciamento de despesas de telecomunicações.|
|**Solução de Problemas**|
|troubleshootingEvents|Conjunto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|A lista de eventos de solução de problemas para o locatário.|
|**Proteção de Informações do Windows**|
|intuneBrandingProfiles|[Coleção intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Intune perfis de identidade visual direcionados a grupos do AAD|
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



