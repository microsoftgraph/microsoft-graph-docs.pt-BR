---
title: tipo de recurso deviceManagementAutopilotEvent
description: Representa um evento de fluxo do piloto automático.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e9a386785163e9870c0075eb2c6676abb23a8b71
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087688"
---
# <a name="devicemanagementautopilotevent-resource-type"></a>tipo de recurso deviceManagementAutopilotEvent

Namespace: microsoft.graph

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
|id|Cadeia de caracteres|O UUID do objeto.|
|deviceId|Cadeia de caracteres|ID de dispositivo associada ao objeto|
|eventDateTime|DateTimeOffset|A hora em que o evento ocorreu.|
|deviceRegisteredDateTime|DateTimeOffset|Data de registro do dispositivo.|
|enrollmentStartDateTime|DateTimeOffset|Data de início do registro do dispositivo.|
|enrollmentType|[windowsAutopilotEnrollmentType](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|Tipo de registro. Os valores possíveis são: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.|
|deviceSerialNumber|Cadeia de caracteres|Número de série do dispositivo.|
|managedDeviceName|String|Nome do dispositivo gerenciado.|
|userPrincipalName|Cadeia de caracteres|Nome principal do usuário usado para registrar o dispositivo.|
|windowsAutopilotDeploymentProfileDisplayName|Cadeia de caracteres|Nome do perfil do AutoPilot.|
|enrollmentid|[enrollmentid](../resources/intune-shared-enrollmentstate.md)|Estado de registro como cadastrado, falhou. Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|windows10EnrollmentCompletionPageConfigurationDisplayName|Cadeia de caracteres|Nome do perfil da página de status do registro|
|DeploymentState|[windowsAutopilotDeploymentState](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|Estado de implantação como êxito, falha, InProgress, SuccessWithTimeout. Os valores possíveis são: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.|
|osVersion|String|Versão do sistema operacional do dispositivo.|
|deploymentDuration|Duração|Duração da implantação do piloto automático, incluindo registro.|
|deploymentTotalDuration|Duração|Duração total da implantação na tela de registro na área de trabalho.|
|devicePreparationDuration|Duração|Tempo gasto no registro do dispositivo.|
|deviceSetupDuration|Duração|Tempo gasto em ESP de dispositivo.|
|accountSetupDuration|Duração|Tempo gasto na ESP do usuário.|
|deploymentStartDateTime|DateTimeOffset|Hora de início da implantação.|
|deploymentEndDateTime|DateTimeOffset|Hora de término da implantação.|
|targetedAppCount|Int32|Contagem de aplicativos direcionados.|
|targetedPolicyCount|Int32|Contagem de políticas direcionadas.|
|enrollmentFailureDetails|Cadeia de caracteres|Detalhes da falha de inscrição.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|policyStatusDetails|coleção [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)|Detalhes de status do aplicativo e da política para este dispositivo.|

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






