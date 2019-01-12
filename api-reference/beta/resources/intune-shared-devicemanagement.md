---
title: Tipo de recurso deviceManagement
description: 'O recurso de deviceManagement representa um contêiner cujo conteúdo varia de acordo com o fluxo de trabalho, incluindo:  '
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: a2f4348da007a3d69d1618151718789d1b72e3e1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961334"
---
# <a name="devicemanagement-resource-type"></a>Tipo de recurso deviceManagement

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

O recurso de deviceManagement representa um contêiner cujo conteúdo varia de acordo com o fluxo de trabalho, incluindo:  

- Configurações do Android for Work
- Eventos de auditoria
- Termos e condições corporativas 
- Perfis de inscrição corporativo
- Definições de configuração de dispositivo
- Gerenciamento de dispositivo
- SIM eletrônico (ESIM)
- Instalação da cerca
- Notificações
- Detalhes, configurações e políticas de inclusão
- Acesso remoto
- Parceiros de assistência remota
- Políticas de RBAC (controle) de acesso baseado em função
- Parceiros de gerenciamento de extensão de telecomunicações
- Solução de problemas de eventos
- Resumos de proteção de informações do Windows

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagement](../api/intune-shared-devicemanagement-get.md)|Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).|
|[Atualizar deviceManagement](../api/intune-shared-devicemanagement-update.md)|Atualizar as propriedades de um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).|
|**Configuração do dispositivo**|
|[ação de enableLegacyPcManagement](../api/intune-shared-devicemanagement-enablelegacypcmanagement.md)|Nenhum|Ainda não documentado|
|**Gerenciamento de dispositivos**|
|[ação de sendCustomNotificationToCompanyPortal](../api/intune-shared-devicemanagement-sendcustomnotificationtocompanyportal.md)|Nenhum|Ainda não documentado|
|**Inclusão**|
|[Função verifyWindowsEnrollmentAutoDiscovery](../api/intune-shared-devicemanagement-verifywindowsenrollmentautodiscovery.md)|Booliano|Ainda não documentado|
|**Controle de acesso baseado em função (RBAC)**|
|[Função getEffectivePermissions](../api/intune-shared-devicemanagement-geteffectivepermissions.md)|Conjunto [rolePermission](../resources/intune-rbac-rolepermission.md)|Recupera permissões efetivas de usuário autenticado no momento|
|[função getRoleScopeTagsByIds](../api/intune-shared-devicemanagement-getrolescopetagsbyids.md)|coleção [roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Ainda não documentado|
|[função getRoleScopeTagsByResource](../api/intune-shared-devicemanagement-getrolescopetagsbyresource.md)|coleção [roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Ainda não documentado|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo associado ao dispositivo.|
|**Configuração do dispositivo**|
|intuneAccountId|Guid|ID da conta Intune para dado locatário|
|legacyPcManangementEnabled|Booliano|A propriedade habilitem Non-MDM gerenciados herdado gerenciamento de PC para essa conta. Esta propriedade é somente leitura.|
|maximumDepTokens|Int32|Número máximo de tokens DEP permitido por locatário.|
|configurações|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|Configurações de nível da conta.|
|**Gerenciamento de dispositivos**|
|accountMoveCompletionDateTime|DateTimeOffset|A data e a hora quando os dados de inquilinos movidos entre scaleunits.|
|adminConsent|[adminConsent](../resources/intune-devices-adminconsent.md)|Informações de consentimento do administrador.|
|deviceProtectionOverview|[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)|Visão geral de proteção do dispositivo.|
|managedDeviceCleanupSettings|[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)|Regra de limpeza do dispositivo|
|subscriptionState|[deviceManagementSubscriptionState](../resources/intune-devices-devicemanagementsubscriptionstate.md)|Estado de assinatura de gerenciamento de dispositivo móvel do locatário. Os valores possíveis são: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|
|assinaturas|[deviceManagementSubscriptions](../resources/intune-devices-devicemanagementsubscriptions.md)|Assinatura de locatário. Os possíveis valores são: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/intune-devices-windowsmalwareoverview.md)|Visão geral de malware para dispositivos do windows.|
|**Inclusão**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|
|:---|:---|:---|
|**Android para o trabalho**|
|androidDeviceOwnerEnrollmentProfiles|coleção [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|Entidades de perfil de inscrição do dispositivo Android proprietário.|
|androidForWorkAppConfigurationSchemas|Coleção [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)|Entidades do esquema de configuração do aplicativo Android for Work.|
|androidForWorkEnrollmentProfiles|Coleção [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|Entidades do perfil de registro do Android for Work.|
|androidForWorkSettings|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|A entidade singleton de configurações do Android for Work.|
|androidManagedStoreAccountEnterpriseSettings|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)|O único Android gerenciado armazenar entidade de configurações de empresa de conta.|
|androidManagedStoreAppConfigurationSchemas|coleção [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|Entidades dos esquemas de configuração de aplicativo do Android Enterprise.|
|**Auditoria**|
|auditEvents|Conjunto [auditEvent](../resources/intune-auditing-auditevent.md)|Eventos de auditoria|
|**Termos de empresa**|
|termsAndConditions|Conjunto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Os termos e condições associados ao gerenciamento do dispositivo da empresa.|
|**Inscrição corporativa**|
|enrollmentProfiles|coleção [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Os perfis de inscrição.|
|importedAppleDeviceIdentities|coleção [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|As identidades de dispositivo Apple importadas.|
|importedDeviceIdentities|coleção [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|As identidades de dispositivo importada.|
|**Configuração do dispositivo**|
|advancedThreatProtectionOnboardingStateSummary|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|O estado de resumo do estado de inclusão de ATP para essa conta.|
|cartToClassAssociations|coleção [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Carrinho de associações de classe.|
|deviceCompliancePolicies|Coleção [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|As políticas de conformidade do dispositivo.|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|O resumo do estado de conformidade dos dispositivos para esta conta.|
|deviceCompliancePolicySettingStateSummaries|Coleção [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|Os estados resumidos das configurações da política de conformidade para esta conta.|
|deviceConfigurationConflictSummary|coleção [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Resumo das políticas em estado de conflito para essa conta.|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|O resumo do estado de configuração de dispositivos para esta conta.|
|deviceConfigurationRestrictedAppsViolations|coleção [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Restrito violações de aplicativos para essa conta.|
|deviceConfigurations|Coleção [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|As configurações de dispositivos.|
|deviceConfigurationUserStateSummaries|[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)|Estado do dispositivo configuração usuário resumo para essa conta.|
|iosUpdateStatuses|Coleção [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)|Os status de instalação de atualizações de software do iOS para esta conta.|
|ndesConnectors|coleção [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|A coleção de conectores Ndes para essa conta.|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|O resumo do status de atualização do software.|
|**Gerenciamento de dispositivos**|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Certificado de notificação por push da Apple.|
|dataSharingConsents|coleção [dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Compartilhamento de dados consentir.|
|detectedApps|Conjunto [detectedApp](../resources/intune-devices-detectedapp.md)|A lista de aplicativos detectados associados a um dispositivo.|
|deviceManagementScripts|coleção [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|A lista de scripts de gerenciamento de dispositivo associado ao inquilino.|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|Visão geral do dispositivo|
|managedDevices|Conjunto [managedDevice](../resources/intune-devices-manageddevice.md)|A lista de dispositivos gerenciados.|
|remoteActionAudits|coleção [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|A lista de ação de dispositivo remoto auditorias com o inquilino.|
|windowsMalwareInformation|coleção [windowsMalwareInformation](../resources/intune-devices-windowsmalwareinformation.md)|A lista de malware afetado no inquilino.|
|**Registro**|
|depOnboardingSettings|coleção [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Este coleções de vários DEP tokens por locatário.|
|importedDeviceIdentities|coleção [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|As identidades de dispositivo importada.|
|importedWindowsAutopilotDeviceIdentities|Coleção [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|Coleção de dispositivos do Windows AutoPilot importados.|
|importedWindowsAutopilotDeviceIdentityUploads|coleção [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)|Coleção de piloto automático do Windows carregar de dispositivos.|
|windowsAutopilotDeploymentProfiles|coleção [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|Perfis de implantação piloto do Windows automático|
|windowsAutopilotDeviceIdentities|coleção [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|As identidades de dispositivo do Windows piloto automático continham a coleção.|
|windowsAutopilotSettings|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|As configurações de conta do Windows piloto automático.|
|**SIM incorporado**|
|embeddedSIMActivationCodePools|coleção [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Os incorporado SIM ativação código pools criados por essa conta.|
|**Instalação da cerca**|
|managementConditions|coleção [managementCondition](../resources/intune-fencing-managementcondition.md)|As condições de gerenciamento associadas ao gerenciamento de dispositivo da empresa.|
|managementConditionStatements|coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|As instruções de condição de gerenciamento associadas ao gerenciamento de dispositivo da empresa.|
|**Notificações**|
|notificationMessageTemplates|Conjunto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Os modelos de mensagens de notificação.|
|**Inclusão**|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|As configurações de acesso condicional do Exchange no local. O acesso condicional no local exigirá que os dispositivos sejam registrados e estejam em conformidade para o acesso ao email|
|deviceCategories|Coleção [deviceCategory](../resources/intune-shared-devicecategory.md)|A lista de categorias de dispositivo com o locatário.|
|deviceEnrollmentConfigurations|Coleção [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|A lista de configurações de registro de dispositivos|
|deviceManagementPartners|Coleção [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|A lista de Parceiros de gerenciamento de dispositivos configurados pelo locatário.|
|exchangeConnectors|Coleção [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|A lista dos Conectores do Exchange configurados pelo locatário.|
|exchangeOnPremisesPolicies|coleção [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|Lista de políticas do Exchange em Premisis configurada por locatário.|
|exchangeOnPremisesPolicy|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|A política que controla o acesso de dispositivo móvel para o Exchange no local|
|mobileThreatDefenseConnectors|Coleção [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|A lista dos conectores de defesa contra ameaças móveis configurados pelo locatário.|
|**Acesso remoto**|
|userPfxCertificates|coleção [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Coleção de certificados PFX associados a um usuário.|
|**Assistência remota**|
|remoteAssistancePartners|Conjunto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Os parceiros de assistência remota.|
|**Controle de acesso baseado em função (RBAC)**|
|resourceOperations|Conjunto [resourceOperation](../resources/intune-rbac-resourceoperation.md)|As operações de recurso.|
|roleAssignments|Conjunto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|As atribuições da função|
|roleDefinitions|Conjunto [roleDefinition](../resources/intune-rbac-roledefinition.md)|As definições da função.|
|roleScopeTags|coleção [roleScopeTag](../resources/intune-rbac-rolescopetag.md)|As marcas de escopo de função.|
|**Gerenciamento de despesas de telecomunicações (Temperatura)**|
|telecomExpenseManagementPartners|Conjunto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|Os parceiros de gerenciamento de despesas de telecomunicações.|
|**Solução de problemas**|
|troubleshootingEvents|Conjunto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|A lista de eventos de solução de problemas para o locatário.|
|**Proteção de informações do Windows**|
|intuneBrandingProfiles|coleção [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Intune branding perfis voltados para grupos AAD|
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



