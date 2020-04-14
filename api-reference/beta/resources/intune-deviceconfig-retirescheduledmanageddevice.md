---
title: tipo de recurso retireScheduledManagedDevice
description: ManagedDevices que estão agendados para desativação
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 326961826e76350cf63a886b946d23eb7444bab1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444885"
---
# <a name="retirescheduledmanageddevice-resource-type"></a>tipo de recurso retireScheduledManagedDevice

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

ManagedDevices que estão agendados para desativação

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|managedDeviceId|String|DeviceID gerenciado|
|managedDeviceName|String|Nome do dispositivo gerenciado|
|deviceType|[deviceType](../resources/intune-shared-devicetype.md)|Tipo de dispositivo de dispositivo gerenciado. Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone` `mac` `winCE`,,, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` `windows10x` `blackberry` `palm`,,,, `unknown`,,,,,,,,,.|
|complianceState|[complianceStatus](../resources/intune-shared-compliancestatus.md)|ComplianceStatus de dispositivo gerenciado. Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|retireAfterDateTime|DateTimeOffset|Desativação de dispositivo gerenciado após DateTime|
|managementAgent|[managementAgentType](../resources/intune-shared-managementagenttype.md)|ManagementAgentType de dispositivo gerenciado. Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm` e `windowsManagementCloudApi`.|
|ownerType|[managedDeviceOwnerType](../resources/intune-shared-manageddeviceownertype.md)|ManagedDeviceOwnerType de dispositivo gerenciado. Os valores possíveis são: `unknown`, `company`, `personal`.|
|deviceCompliancePolicyName|String|Nome da política de conformidade do dispositivo|
|deviceCompliancePolicyId|String|Política de conformidade do dispositivo|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.retireScheduledManagedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.retireScheduledManagedDevice",
  "id": "String (identifier)",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "deviceType": "String",
  "complianceState": "String",
  "retireAfterDateTime": "String (timestamp)",
  "managementAgent": "String",
  "ownerType": "String",
  "deviceCompliancePolicyName": "String",
  "deviceCompliancePolicyId": "String"
}
```



