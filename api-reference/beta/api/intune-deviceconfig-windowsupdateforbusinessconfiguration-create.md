---
title: Criar windowsUpdateForBusinessConfiguration
description: Cria um novo objeto windowsUpdateForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f5a1e2ef29eceb852cdcecaff3516ee96a05662e
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858447"
---
# <a name="create-windowsupdateforbusinessconfiguration"></a>Criar windowsUpdateForBusinessConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Cria um novo objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto windowsUpdateForBusinessConfiguration.

A tabela a seguir mostra as propriedades que são necessárias ao criar windowsUpdateForBusinessConfiguration.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|Coleção String|Lista de marcas de escopo para esta instância de entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
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



## <a name="response"></a>Resposta
Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2828

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly",
  "prereleaseFeatures": "settingsOnly",
  "automaticUpdateMode": "notifyDownload",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "everyday",
    "scheduledInstallTime": "11:59:31.3170000"
  },
  "qualityUpdatesDeferralPeriodInDays": 2,
  "featureUpdatesDeferralPeriodInDays": 2,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
  "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
  "businessReadyUpdatesOnly": "all",
  "skipChecksBeforeRestart": true,
  "updateWeeks": "firstWeek",
  "qualityUpdatesPauseStartDate": "2016-12-31",
  "featureUpdatesPauseStartDate": "2016-12-31",
  "featureUpdatesRollbackWindowInDays": 2,
  "qualityUpdatesWillBeRolledBack": true,
  "featureUpdatesWillBeRolledBack": true,
  "qualityUpdatesRollbackStartDateTime": "2016-12-31T23:57:01.05526-08:00",
  "featureUpdatesRollbackStartDateTime": "2017-01-01T00:03:21.6080517-08:00",
  "engagedRestartDeadlineInDays": 12,
  "engagedRestartSnoozeScheduleInDays": 2,
  "engagedRestartTransitionScheduleInDays": 6,
  "deadlineForFeatureUpdatesInDays": 15,
  "deadlineForQualityUpdatesInDays": 15,
  "deadlineGracePeriodInDays": 9,
  "postponeRebootUntilAfterDeadline": true,
  "autoRestartNotificationDismissal": "automatic",
  "scheduleRestartWarningInHours": 13,
  "scheduleImminentRestartWarningInMinutes": 7,
  "userPauseAccess": "enabled",
  "userWindowsUpdateScanAccess": "enabled",
  "updateNotificationLevel": "defaultNotifications",
  "allowWindows11Upgrade": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3000

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "id": "4928dd6a-dd6a-4928-6add-28496add2849",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly",
  "prereleaseFeatures": "settingsOnly",
  "automaticUpdateMode": "notifyDownload",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "everyday",
    "scheduledInstallTime": "11:59:31.3170000"
  },
  "qualityUpdatesDeferralPeriodInDays": 2,
  "featureUpdatesDeferralPeriodInDays": 2,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
  "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
  "businessReadyUpdatesOnly": "all",
  "skipChecksBeforeRestart": true,
  "updateWeeks": "firstWeek",
  "qualityUpdatesPauseStartDate": "2016-12-31",
  "featureUpdatesPauseStartDate": "2016-12-31",
  "featureUpdatesRollbackWindowInDays": 2,
  "qualityUpdatesWillBeRolledBack": true,
  "featureUpdatesWillBeRolledBack": true,
  "qualityUpdatesRollbackStartDateTime": "2016-12-31T23:57:01.05526-08:00",
  "featureUpdatesRollbackStartDateTime": "2017-01-01T00:03:21.6080517-08:00",
  "engagedRestartDeadlineInDays": 12,
  "engagedRestartSnoozeScheduleInDays": 2,
  "engagedRestartTransitionScheduleInDays": 6,
  "deadlineForFeatureUpdatesInDays": 15,
  "deadlineForQualityUpdatesInDays": 15,
  "deadlineGracePeriodInDays": 9,
  "postponeRebootUntilAfterDeadline": true,
  "autoRestartNotificationDismissal": "automatic",
  "scheduleRestartWarningInHours": 13,
  "scheduleImminentRestartWarningInMinutes": 7,
  "userPauseAccess": "enabled",
  "userWindowsUpdateScanAccess": "enabled",
  "updateNotificationLevel": "defaultNotifications",
  "allowWindows11Upgrade": true
}
```




