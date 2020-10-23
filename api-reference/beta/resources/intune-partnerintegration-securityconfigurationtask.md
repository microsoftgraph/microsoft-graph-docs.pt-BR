---
title: tipo de recurso securityConfigurationTask
description: Uma tarefa de configuração de segurança.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 37d6d4a3c42dafaf03bd5879fc2e0fd4905b14cd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709871"
---
# <a name="securityconfigurationtask-resource-type"></a>tipo de recurso securityConfigurationTask

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma tarefa de configuração de segurança.


Herda de [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar securityConfigurationTasks](../api/intune-partnerintegration-securityconfigurationtask-list.md)|coleção [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md)|Listar Propriedades e relações dos objetos [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) .|
|[Obter securityConfigurationTask](../api/intune-partnerintegration-securityconfigurationtask-get.md)|[securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md)|Leia as propriedades e as relações do objeto [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) .|
|[Criar securityConfigurationTask](../api/intune-partnerintegration-securityconfigurationtask-create.md)|[securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md)|Criar um novo objeto [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) .|
|[Excluir securityConfigurationTask](../api/intune-partnerintegration-securityconfigurationtask-delete.md)|Nenhum|Exclui [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md).|
|[Atualizar securityConfigurationTask](../api/intune-partnerintegration-securityconfigurationtask-update.md)|[securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md)|Atualiza as propriedades de um objeto [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A chave da entidade. Herdado de [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|displayName|String|O nome. Herdado de [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|description|String|A descrição. Herdado de [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|createdDateTime|DateTimeOffset|A data de criação. Herdado de [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|dueDateTime|DateTimeOffset|A data de conclusão. Herdado de [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|category|[deviceAppManagementTaskCategory](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|A categoria. Herdado de [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md). Os valores possíveis são: `unknown` e `advancedThreatProtection`.|
|prioridade|[deviceAppManagementTaskPriority](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|A prioridade. Herdado de [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md). Os valores possíveis são: `none`, `high`, `low`.|
|criador|String|O endereço de email do criador. Herdado de [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|creatorNotes|String|Observações do criador. Herdado de [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|assignedTo|String|O nome ou email do administrador ao qual esta tarefa é atribuída. Herdado de [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|status|[deviceAppManagementTaskStatus](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|O status. Herdado de [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md). Os valores possíveis são: `unknown`, `pending`, `active`, `completed`, `rejected`.|
|endpointSecurityPolicy|[endpointSecurityConfigurationType](../resources/intune-partnerintegration-endpointsecurityconfigurationtype.md)|O tipo de política de segurança do ponto de extremidade. Os valores possíveis são: `unknown`, `antivirus`, `diskEncryption`, `firewall`, `endpointDetectionAndResponse`, `attackSurfaceReduction`, `accountProtection`.|
|applicablePlatform|[endpointSecurityConfigurationApplicablePlatform](../resources/intune-partnerintegration-endpointsecurityconfigurationapplicableplatform.md)|A plataforma aplicável. Os valores possíveis são: `unknown`, `macOS`, `windows10AndLater`, `windows10AndWindowsServer`.|
|endpointSecurityPolicyProfile|[endpointSecurityConfigurationProfileType](../resources/intune-partnerintegration-endpointsecurityconfigurationprofiletype.md)|O perfil da política de segurança do ponto de extremidade. Os valores possíveis são:, `unknown` `antivirus` , `windowsSecurity` , `bitLocker` , `fileVault` , `firewall` , `firewallRules` , `endpointDetectionAndResponse` , `deviceControl` , `appAndBrowserIsolation` , `exploitProtection` , `webProtection` ,, `applicationControl` `attackSurfaceReductionRules` `accountProtection` .|
|insights|String|Informações sobre a mitigação.|
|managedDeviceCount|Int32|O número de dispositivos vulneráveis.|
|intendedSettings|Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)|As configurações pretendidas e seus valores.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|managedDevices|coleção [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|Os dispositivos gerenciados vulneráveis.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityConfigurationTask"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityConfigurationTask",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "dueDateTime": "String (timestamp)",
  "category": "String",
  "priority": "String",
  "creator": "String",
  "creatorNotes": "String",
  "assignedTo": "String",
  "status": "String",
  "endpointSecurityPolicy": "String",
  "applicablePlatform": "String",
  "endpointSecurityPolicyProfile": "String",
  "insights": "String",
  "managedDeviceCount": 1024,
  "intendedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```





