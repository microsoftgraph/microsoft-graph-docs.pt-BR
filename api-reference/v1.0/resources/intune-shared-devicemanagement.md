---
title: Tipo de recurso deviceManagement
description: 'O recurso deviceManagement representa um contêiner cujo conteúdo varia de acordo com o fluxo de trabalho, incluindo:  '
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 83d3f3cda24c5961a34cb5c38de3ee43d6f5fe44
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475769"
---
# <a name="devicemanagement-resource-type"></a>Tipo de recurso deviceManagement

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso deviceManagement representa um contêiner cujo conteúdo varia de acordo com o fluxo de trabalho, incluindo:  

- Eventos de auditoria  
- Termos e condições corporativos   
- Configurações de dispositivo  
- Gerenciamento de dispositivo  
- Proteção de pontos de extremidade  
- Perfis de registro  
- Notificações  
- Políticas, configurações e detalhes de integração  
- Políticas de controle de acesso baseado em função (RBAC)  
- Parceiros de assistência remota  
- Parceiros de gerenciamento de expansão de telecomunicações  
- Solução de problemas de eventos  
- Resumos da Proteção de Informações do Windows  

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagement](../api/intune-shared-devicemanagement-get.md)|[deviceManagement](../resources/intune-shared-devicemanagement.md)|Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).|
|[Atualizar deviceManagement](../api/intune-shared-devicemanagement-update.md)|[deviceManagement](../resources/intune-shared-devicemanagement.md)|Atualizar as propriedades de um objeto de [deviceManagement](../resources/intune-shared-devicemanagement.md).|
|**Integração**|
|[Função verifyWindowsEnrollmentAutoDiscovery](../api/intune-shared-devicemanagement-verifywindowsenrollmentautodiscovery.md)|Booliano|Ainda não documentado|
|**RBAC**|
|[Função getEffectivePermissions](../api/intune-shared-devicemanagement-geteffectivepermissions.md)|[Coleção rolePermission](../resources/intune-rbac-rolepermission.md) ou coleção de cadeias de caracteres|Recupera permissões efetivas de usuário autenticado no momento|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do dispositivo|
|**Configuração do dispositivo**|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|Configurações de nível da conta.|
|**Gerenciamento de dispositivos**|
|subscriptionState|Cadeia de caracteres|Estado de assinatura de gerenciamento de dispositivo móvel do locatário. Os valores possíveis são `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|
|**Integração**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|**Termos e condições corporativos**|
|termsAndConditions|Conjunto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Os termos e condições associados ao gerenciamento do dispositivo da empresa.|
|**Configuração do dispositivo**|
|intuneAccountId|Guid|ID da conta do Intune para determinado locatário.|
|deviceCompliancePolicies|Coleção [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|As políticas de conformidade do dispositivo.|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|O resumo do estado de conformidade dos dispositivos para esta conta.|
|deviceCompliancePolicySettingStateSummaries|Coleção [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|Os estados resumidos das configurações da política de conformidade para esta conta.|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|O resumo do estado de configuração de dispositivos para esta conta.|
|deviceConfigurations|Coleção [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|As configurações de dispositivos.|
|iosUpdateStatuses|Coleção [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)|Os status de instalação de atualizações de software do iOS para esta conta.|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|O resumo do status de atualização do software.|
|**Gerenciamento de dispositivos**|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Certificado de notificação por push da Apple.|
|detectedApps|Conjunto [detectedApp](../resources/intune-devices-detectedapp.md)|A lista de aplicativos detectados associados a um dispositivo.|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|Visão geral do dispositivo|
|managedDevices|Conjunto [managedDevice](../resources/intune-devices-manageddevice.md)|A lista de dispositivos gerenciados.|
|**Notificações**|
|notificationMessageTemplates|Conjunto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Os modelos de mensagens de notificação.|
|**Integração**|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|As configurações de acesso condicional do Exchange no local. O acesso condicional no local exigirá que os dispositivos sejam registrados e estejam em conformidade para o acesso ao email|
|deviceCategories|Coleção [deviceCategory](../resources/intune-shared-devicecategory.md)|A lista de categorias de dispositivo com o locatário.|
|deviceEnrollmentConfigurations|Coleção [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|A lista de configurações de registro de dispositivos|
|deviceManagementPartners|Coleção [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|A lista de Parceiros de gerenciamento de dispositivos configurados pelo locatário.|
|complianceManagementPartners|[coleção complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)|A lista de Parceiros de Gerenciamento de Conformidade configurados pelo locatário.|
|exchangeConnectors|Coleção [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|A lista dos Conectores do Exchange configurados pelo locatário.|
|mobileThreatDefenseConnectors|Coleção [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|A lista dos conectores de defesa contra ameaças móveis configurados pelo locatário.|
|**RBAC**|
|resourceOperations|Conjunto [resourceOperation](../resources/intune-rbac-resourceoperation.md)|As operações de recurso.|
|roleAssignments|Conjunto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|As atribuições da função|
|roleDefinitions|Conjunto [roleDefinition](../resources/intune-rbac-roledefinition.md)|As definições da função.|
|**Assistência remota**|
|remoteAssistancePartners|Conjunto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Os parceiros de assistência remota.|
|**Gerenciamento de despesas de telecomunicações**|
|telecomExpenseManagementPartners|Conjunto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|Os parceiros de gerenciamento de despesas de telecomunicações.|
|**Solução de Problemas**|
|troubleshootingEvents|Conjunto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|A lista de eventos de solução de problemas para o locatário.|
|**Proteção de Informações do Windows**|
|windowsInformationProtectionAppLearningSummaries|Conjunto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)|Os resumos de aprendizagem de aplicativos da proteção de informações do Windows.|
|windowsInformationProtectionNetworkLearningSummaries|Conjunto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)|Os resumos de aprendizagem de redes da proteção de informações do Windows.|


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









