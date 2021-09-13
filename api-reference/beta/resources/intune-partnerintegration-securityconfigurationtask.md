---
title: Tipo de recurso securityConfigurationTask
description: Uma tarefa de configuração de segurança.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4d9922bbad0328171c97b216c4f438f95ceacfce
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59100985"
---
# <a name="securityconfigurationtask-resource-type"></a>Tipo de recurso securityConfigurationTask

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma tarefa de configuração de segurança.


Herda de [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar securityConfigurationTasks](../api/intune-partnerintegration-securityconfigurationtask-list.md)|[Coleção securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md)|Listar propriedades e relações dos objetos [securityConfigurationTask.](../resources/intune-partnerintegration-securityconfigurationtask.md)|
|[Obter securityConfigurationTask](../api/intune-partnerintegration-securityconfigurationtask-get.md)|[securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md)|Leia propriedades e relações do [objeto securityConfigurationTask.](../resources/intune-partnerintegration-securityconfigurationtask.md)|
|[Criar securityConfigurationTask](../api/intune-partnerintegration-securityconfigurationtask-create.md)|[securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md)|Crie um novo [objeto securityConfigurationTask.](../resources/intune-partnerintegration-securityconfigurationtask.md)|
|[Excluir securityConfigurationTask](../api/intune-partnerintegration-securityconfigurationtask-delete.md)|Nenhum|Exclui um [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md).|
|[Atualizar securityConfigurationTask](../api/intune-partnerintegration-securityconfigurationtask-update.md)|[securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md)|Atualize as propriedades de [um objeto securityConfigurationTask.](../resources/intune-partnerintegration-securityconfigurationtask.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A chave da entidade. Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|displayName|Cadeia de caracteres|O nome. Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|description|Cadeia de caracteres|A descrição. Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|createdDateTime|DateTimeOffset|A data criada. Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|dueDateTime|DateTimeOffset|A data de vencimento. Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|category|[deviceAppManagementTaskCategory](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|A categoria. Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md). Os valores possíveis são: `unknown` e `advancedThreatProtection`.|
|prioridade|[deviceAppManagementTaskPriority](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|A prioridade. Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md). Os valores possíveis são: `none`, `high`, `low`.|
|criador|Cadeia de Caracteres|O endereço de email do criador. Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|creatorNotes|Cadeia de Caracteres|Observações do criador. Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|assignedTo|Cadeia de caracteres|O nome ou o email do administrador ao que essa tarefa é atribuída. Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|status|[deviceAppManagementTaskStatus](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|O status. Herdado [de deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md). Os valores possíveis são: `unknown`, `pending`, `active`, `completed`, `rejected`.|
|endpointSecurityPolicy|[endpointSecurityConfigurationType](../resources/intune-partnerintegration-endpointsecurityconfigurationtype.md)|O tipo de política de segurança do ponto de extremidade. Os valores possíveis são: `unknown`, `antivirus`, `diskEncryption`, `firewall`, `endpointDetectionAndResponse`, `attackSurfaceReduction`, `accountProtection`.|
|applicablePlatform|[endpointSecurityConfigurationApplicablePlatform](../resources/intune-partnerintegration-endpointsecurityconfigurationapplicableplatform.md)|A plataforma aplicável. Os valores possíveis são: `unknown`, `macOS`, `windows10AndLater`, `windows10AndWindowsServer`.|
|endpointSecurityPolicyProfile|[endpointSecurityConfigurationProfileType](../resources/intune-partnerintegration-endpointsecurityconfigurationprofiletype.md)|O perfil da política de segurança do ponto de extremidade. Os valores possíveis são: `unknown` , , , , , , , , , `antivirus` , , `windowsSecurity` , , , `bitLocker` `fileVault` `firewall` , `firewallRules` `endpointDetectionAndResponse` `deviceControl` `appAndBrowserIsolation` `exploitProtection` `webProtection` `applicationControl` `attackSurfaceReductionRules` `accountProtection` .|
|insights|Cadeia de Caracteres|Informações sobre a mitigação.|
|managedDeviceCount|Int32|O número de dispositivos vulneráveis.|
|intendedSettings|Coleção [keyValuePair](../resources/intune-partnerintegration-keyvaluepair.md)|As configurações pretenddas e seus valores.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|managedDevices|[coleção vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|Os dispositivos gerenciados vulneráveis.|

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



