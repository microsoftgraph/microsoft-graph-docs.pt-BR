---
title: Tipo de recurso deviceManagementAutopilotEvent
description: Representa um evento de fluxo do Autopilot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d438723ab14cb9fd47828bbaba3b45ccbf5f7f13
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266797"
---
# <a name="devicemanagementautopilotevent-resource-type"></a>Tipo de recurso deviceManagementAutopilotEvent

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um evento de fluxo do Autopilot.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementAutopilotEvents](../api/intune-troubleshooting-devicemanagementautopilotevent-list.md)|[Coleção deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|Listar propriedades e relações dos [objetos deviceManagementAutopilotEvent.](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|
|[Obter deviceManagementAutopilotEvent](../api/intune-troubleshooting-devicemanagementautopilotevent-get.md)|[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|Leia propriedades e relações do [objeto deviceManagementAutopilotEvent.](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|
|[Criar deviceManagementAutopilotEvent](../api/intune-troubleshooting-devicemanagementautopilotevent-create.md)|[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|Crie um novo [objeto deviceManagementAutopilotEvent.](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|
|[Excluir deviceManagementAutopilotEvent](../api/intune-troubleshooting-devicemanagementautopilotevent-delete.md)|Nenhum|Exclui um [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md).|
|[Atualizar deviceManagementAutopilotEvent](../api/intune-troubleshooting-devicemanagementautopilotevent-update.md)|[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|Atualize as propriedades de [um objeto deviceManagementAutopilotEvent.](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O UUID do objeto.|
|deviceId|Cadeia de caracteres|ID do dispositivo associada ao objeto|
|eventDateTime|DateTimeOffset|A hora em que o evento ocorreu.|
|deviceRegisteredDateTime|DateTimeOffset|Data do registro do dispositivo.|
|enrollmentStartDateTime|DateTimeOffset|Data de início do registro do dispositivo.|
|enrollmentType|[windowsAutopilotEnrollmentType](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|Tipo de registro. Os valores possíveis são: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.|
|deviceSerialNumber|Cadeia de caracteres|Número de série do dispositivo.|
|managedDeviceName|String|Nome do dispositivo gerenciado.|
|userPrincipalName|Cadeia de caracteres|Nome principal do usuário usado para registrar o dispositivo.|
|windowsAutopilotDeploymentProfileDisplayName|Cadeia de caracteres|Nome do perfil do piloto automático.|
|enrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Estado de registro como Inscrito, Falha. Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|windows10EnrollmentCompletionPageConfigurationDisplayName|Cadeia de caracteres|Nome do perfil da Página de Status do Registro|
|windows10EnrollmentCompletionPageConfigurationId|Cadeia de caracteres|ID do perfil da página de status de registro|
|deploymentState|[windowsAutopilotDeploymentState](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|Estado de implantação como Sucesso, Falha, InProgress, SuccessWithTimeout. Os valores possíveis são: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.|
|deviceSetupStatus|[windowsAutopilotDeploymentState](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|Status de implantação para a fase de configuração do dispositivo de página de status de registro. Os valores possíveis são: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.|
|accountSetupStatus|[windowsAutopilotDeploymentState](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|Status de implantação para a fase de configuração da conta de página de status de registro. Os valores possíveis são: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.|
|osVersion|String|Versão do sistema operacional do dispositivo.|
|deploymentDuration|Duration|Duração da implantação do piloto automático, incluindo o registro.|
|deploymentTotalDuration|Duration|Duração total da implantação do registro na tela da Área de Trabalho.|
|devicePreparationDuration|Duration|Tempo gasto no registro do dispositivo.|
|deviceSetupDuration|Duration|Tempo gasto no ESP do dispositivo.|
|accountSetupDuration|Duration|Tempo gasto no ESP do usuário.|
|deploymentStartDateTime|DateTimeOffset|Hora de início da implantação.|
|deploymentEndDateTime|DateTimeOffset|Hora de término da implantação.|
|targetedAppCount|Int32|Contagem de aplicativos direcionados.|
|targetedPolicyCount|Int32|Contagem de políticas direcionadas.|
|enrollmentFailureDetails|Cadeia de caracteres|Detalhes de falha de registro.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|policyStatusDetails|[Coleção deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)|Detalhes de política e status do aplicativo para este dispositivo.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementAutopilotEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "id": "String (identifier)",
  "deviceId": "String",
  "eventDateTime": "String (timestamp)",
  "deviceRegisteredDateTime": "String (timestamp)",
  "enrollmentStartDateTime": "String (timestamp)",
  "enrollmentType": "String",
  "deviceSerialNumber": "String",
  "managedDeviceName": "String",
  "userPrincipalName": "String",
  "windowsAutopilotDeploymentProfileDisplayName": "String",
  "enrollmentState": "String",
  "windows10EnrollmentCompletionPageConfigurationDisplayName": "String",
  "windows10EnrollmentCompletionPageConfigurationId": "String",
  "deploymentState": "String",
  "deviceSetupStatus": "String",
  "accountSetupStatus": "String",
  "osVersion": "String",
  "deploymentDuration": "String (duration)",
  "deploymentTotalDuration": "String (duration)",
  "devicePreparationDuration": "String (duration)",
  "deviceSetupDuration": "String (duration)",
  "accountSetupDuration": "String (duration)",
  "deploymentStartDateTime": "String (timestamp)",
  "deploymentEndDateTime": "String (timestamp)",
  "targetedAppCount": 1024,
  "targetedPolicyCount": 1024,
  "enrollmentFailureDetails": "String"
}
```




