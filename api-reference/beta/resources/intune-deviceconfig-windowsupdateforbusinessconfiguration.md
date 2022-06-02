---
title: Tipo de recurso windowsUpdateForBusinessConfiguration
description: Configuração do Windows Update para Empresas.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 147b12450cb53787e1ebb0156a8d595703522078
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2022
ms.locfileid: "65857831"
---
# <a name="windowsupdateforbusinessconfiguration-resource-type"></a>Tipo de recurso windowsUpdateForBusinessConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Configuração do Windows Update para Empresas.


Herda de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsUpdateForBusinessConfigurations](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-list.md)|Coleção [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md)|Lista propriedades e relações dos objetos [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).|
|[Obter windowsUpdateForBusinessConfiguration](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-get.md)|[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md)|Propriedades de leitura e relações do objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).|
|[Criar windowsUpdateForBusinessConfiguration](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-create.md)|[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md)|Cria um novo objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).|
|[Excluir windowsUpdateForBusinessConfiguration](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-delete.md)|Nenhum|Exclui um [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).|
|[Atualizar windowsUpdateForBusinessConfiguration](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-update.md)|[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md)|Atualiza as propriedades de um objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).|
|[ação extendFeatureUpdatesPause](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-extendfeatureupdatespause.md)|Nenhum|Estender a pausa de atualizações de recursos para um anel Windows Update para Empresas.|
|[ação extendQualityUpdatesPause](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-extendqualityupdatespause.md)|Nenhum|Estender a pausa de atualizações de qualidade para um Windows Update para empresas.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Booliano|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|description|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deliveryOptimizationMode|[windowsDeliveryOptimizationMode](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|Modo de Otimização de Entrega. Os valores possíveis são: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.|
|prereleaseFeatures|[prereleaseFeatures](../resources/intune-deviceconfig-prereleasefeatures.md)|Os recursos de pré-lançamento. Os valores possíveis são: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.|
|automaticUpdateMode|[automaticUpdateMode](../resources/intune-deviceconfig-automaticupdatemode.md)|Modo de atualização automática. Os valores possíveis são: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.|
|microsoftUpdateServiceAllowed|Boolean|Permitir serviço Microsoft Update|
|driversExcluded|Boolean|Excluir drivers de atualização do Windows|
|installationSchedule|[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|Cronograma de instalação|
|qualityUpdatesDeferralPeriodInDays|Int32|Aditar atualizações de qualidade por este número de dias|
|featureUpdatesDeferralPeriodInDays|Int32|Aditar atualizações de recursos por este número de dias|
|qualityUpdatesPaused|Boolean|Pausar atualizações de qualidade|
|featureUpdatesPaused|Boolean|Pausar atualizações de recursos|
|qualityUpdatesPauseExpiryDateTime|DateTimeOffset|Data e hora de expiração da pausa de atualizações de qualidade|
|featureUpdatesPauseExpiryDateTime|DateTimeOffset|Data e hora de expiração da pausa de atualizações de recursos|
|businessReadyUpdatesOnly|[windowsUpdateType](../resources/intune-deviceconfig-windowsupdatetype.md)|Determina de quais dispositivos de branch receberão suas atualizações. Os possíveis valores são: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.|
|skipChecksBeforeRestart|Booliano|Defina para ignorar todas as verificações antes da reinicialização: Nível da bateria = 40%, Presença do usuário, Exibição Necessária, Modo de Apresentação, Modo de tela inteira, estado da chamada telefônica, modo de jogo etc. |
|updateWeeks|[windowsUpdateForBusinessUpdateWeeks](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|Agendou a instalação da atualização nas semanas do mês. Os possíveis valores são: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.|
|qualityUpdatesPauseStartDate|Data|Data de início da pausa das Atualizações de Qualidade. Essa propriedade é somente leitura.|
|featureUpdatesPauseStartDate|Data|Data de início da pausa das Atualizações de Recursos. Essa propriedade é somente leitura.|
|featureUpdatesRollbackWindowInDays|Int32|O número de dias após uma Atualização de Recursos para a qual uma reversão é válida|
|qualityUpdatesWillBeRolledBack|Booliano|Especifica se as Atualizações de Qualidade devem ser revertidas no próximo check-in do dispositivo|
|featureUpdatesWillBeRolledBack|Booliano|Especifica se as Atualizações de Recursos devem ser revertidas no próximo check-in do dispositivo|
|qualityUpdatesRollbackStartDateTime|DateTimeOffset|Data e hora de início da reversão de atualizações de qualidade|
|featureUpdatesRollbackStartDateTime|DateTimeOffset|Data e hora de início da reversão de atualizações de recursos|
|engagedRestartDeadlineInDays|Int32|Prazo em dias antes de agendar e executar automaticamente uma reinicialização pendente fora do horário ativo, com intervalo válido de 2 a 30 dias|
|engagedRestartSnoozeScheduleInDays|Int32|Número de dias em que um usuário pode adiar notificações de lembrete de Reinicialização Ativada com intervalo válido de 1 a 3 dias|
|engagedRestartTransitionScheduleInDays|Int32|Número de dias antes da transição das Reinicializações Automáticas agendadas fora do horário ativo para a Reinicialização Ativada, o que exige que o usuário agende, com intervalo válido de 0 a 30 dias|
|deadlineForFeatureUpdatesInDays|Int32|Número de dias antes que as atualizações de recursos sejam instaladas automaticamente com um intervalo válido de 0 a 30 dias|
|deadlineForQualityUpdatesInDays|Int32|Número de dias antes que as atualizações de qualidade sejam instaladas automaticamente com intervalo válido de 0 a 30 dias|
|deadlineGracePeriodInDays|Int32|Número de dias após o prazo até que as reinicializações ocorram automaticamente com intervalo válido de 0 a 7 dias|
|postponeRebootUntilAfterDeadline|Booliano|Especifica se o dispositivo deve aguardar até o prazo para reinicializar fora do horário ativo|
|autoRestartNotificationDismissal|[autoRestartNotificationDismissalMethod](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|Especifique o método pelo qual a notificação de reinicialização automática necessária é ignorada. Os valores possíveis são: `notConfigured`, `automatic`, `user`.|
|scheduleRestartWarningInHours|Int32|Especifique o período para notificações de lembrete de aviso de reinicialização automática. Valores com suporte: 2, 4, 8, 12 ou 24 (horas).|
|scheduleImminentRestartWarningInMinutes|Int32|Especifique o período para notificações de aviso iminentes de reinicialização automática. Valores com suporte: 15, 30 ou 60 (minutos).|
|userPauseAccess|[Capacitação](../resources/intune-shared-enablement.md)|Especifica se o acesso do usuário final deve ser habilitado para pausar atualizações de software. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|userWindowsUpdateScanAccess|[Capacitação](../resources/intune-shared-enablement.md)|Especifica se o acesso do usuário deve ser desabilitado para verificar Windows Update. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|updateNotificationLevel|[windowsUpdateNotificationDisplayOption](../resources/intune-deviceconfig-windowsupdatenotificationdisplayoption.md)|Especifica o que Windows Update notificações que os usuários veem. Os valores possíveis são: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.|
|allowWindows11Upgrade|Booliano|Permitir que dispositivos Windows 10 qualificados atualizem para a versão mais recente do Windows 11.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|[Coleção deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status da instalação da configuração de dispositivo por dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status de instalação da configuração do dispositivo por usuário. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status de dispositivos para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status de usuários para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Visão geral de dispositivos de configuração para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceUpdateStates|[coleção windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|Windows atualização para estados do dispositivo de configuração de negócios. Esta coleção pode conter um máximo de 500 elementos.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdateForBusinessConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "deliveryOptimizationMode": "String",
  "prereleaseFeatures": "String",
  "automaticUpdateMode": "String",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "String",
    "scheduledInstallTime": "String (time of day)"
  },
  "qualityUpdatesDeferralPeriodInDays": 1024,
  "featureUpdatesDeferralPeriodInDays": 1024,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "String (timestamp)",
  "featureUpdatesPauseExpiryDateTime": "String (timestamp)",
  "businessReadyUpdatesOnly": "String",
  "skipChecksBeforeRestart": true,
  "updateWeeks": "String",
  "qualityUpdatesPauseStartDate": "String (Date)",
  "featureUpdatesPauseStartDate": "String (Date)",
  "featureUpdatesRollbackWindowInDays": 1024,
  "qualityUpdatesWillBeRolledBack": true,
  "featureUpdatesWillBeRolledBack": true,
  "qualityUpdatesRollbackStartDateTime": "String (timestamp)",
  "featureUpdatesRollbackStartDateTime": "String (timestamp)",
  "engagedRestartDeadlineInDays": 1024,
  "engagedRestartSnoozeScheduleInDays": 1024,
  "engagedRestartTransitionScheduleInDays": 1024,
  "deadlineForFeatureUpdatesInDays": 1024,
  "deadlineForQualityUpdatesInDays": 1024,
  "deadlineGracePeriodInDays": 1024,
  "postponeRebootUntilAfterDeadline": true,
  "autoRestartNotificationDismissal": "String",
  "scheduleRestartWarningInHours": 1024,
  "scheduleImminentRestartWarningInMinutes": 1024,
  "userPauseAccess": "String",
  "userWindowsUpdateScanAccess": "String",
  "updateNotificationLevel": "String",
  "allowWindows11Upgrade": true
}
```




