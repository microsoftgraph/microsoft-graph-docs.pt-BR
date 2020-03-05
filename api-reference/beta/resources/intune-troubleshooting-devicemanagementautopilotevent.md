---
title: tipo de recurso deviceManagementAutopilotEvent
description: Representa um evento de fluxo do piloto automático.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 361506e7fb04aaa06eac708ab3a13b1f08f6e163
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523391"
---
# <a name="devicemanagementautopilotevent-resource-type"></a>tipo de recurso deviceManagementAutopilotEvent

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um evento de fluxo do piloto automático.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementAutopilotEvents](../api/intune-troubleshooting-devicemanagementautopilotevent-list.md)|coleção [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|Listar Propriedades e relações dos objetos [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .|
|[Obter deviceManagementAutopilotEvent](../api/intune-troubleshooting-devicemanagementautopilotevent-get.md)|[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|Leia as propriedades e as relações do objeto [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .|
|[Criar deviceManagementAutopilotEvent](../api/intune-troubleshooting-devicemanagementautopilotevent-create.md)|[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|Criar um novo objeto [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .|
|[Excluir deviceManagementAutopilotEvent](../api/intune-troubleshooting-devicemanagementautopilotevent-delete.md)|Nenhum|Exclui [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md).|
|[Atualizar deviceManagementAutopilotEvent](../api/intune-troubleshooting-devicemanagementautopilotevent-update.md)|[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|Atualiza as propriedades de um objeto [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O UUID do objeto.|
|eventDateTime|DateTimeOffset|A hora em que o evento ocorreu.|
|deviceRegisteredDateTime|DateTimeOffset|Data de registro do dispositivo.|
|enrollmentStartDateTime|DateTimeOffset|Data de início do registro do dispositivo.|
|enrollmentType|[windowsAutopilotEnrollmentType](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|Tipo de registro. Os valores possíveis são: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.|
|deviceSerialNumber|String|Número de série do dispositivo.|
|managedDeviceName|String|Nome do dispositivo gerenciado.|
|userPrincipalName|String|Nome principal do usuário usado para registrar o dispositivo.|
|windowsAutopilotDeploymentProfileDisplayName|String|Nome do perfil do AutoPilot.|
|enrollmentid|[enrollmentid](../resources/intune-shared-enrollmentstate.md)|Estado de registro como cadastrado, falhou. Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|windows10EnrollmentCompletionPageConfigurationDisplayName|String|Nome do perfil da página de status do registro|
|DeploymentState|[windowsAutopilotDeploymentState](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|Estado de implantação como êxito, falha, InProgress, SuccessWithTimeout. Os valores possíveis são: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.|
|osVersion|Cadeia de caracteres|Versão do sistema operacional do dispositivo.|
|deploymentDuration|Duração|Duração da implantação do piloto automático, incluindo registro.|
|deploymentTotalDuration|Duração|Duração total da implantação na tela de registro na área de trabalho.|
|devicePreparationDuration|Duração|Tempo gasto no registro do dispositivo.|
|deviceSetupDuration|Duração|Tempo gasto em ESP de dispositivo.|
|accountSetupDuration|Duração|Tempo gasto na ESP do usuário.|
|deploymentStartDateTime|DateTimeOffset|Hora de início da implantação.|
|deploymentEndDateTime|DateTimeOffset|Hora de término da implantação.|
|targetedAppCount|Int32|Contagem de aplicativos direcionados.|
|targetedPolicyCount|Int32|Contagem de políticas direcionadas.|
|enrollmentFailureDetails|String|Detalhes da falha de inscrição.|

## <a name="relationships"></a>Relações
Nenhum

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
  "deploymentState": "String",
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



