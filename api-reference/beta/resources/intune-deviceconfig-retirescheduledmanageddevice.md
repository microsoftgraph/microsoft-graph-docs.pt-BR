---
title: Tipo de recurso retireScheduledManagedDevice
description: ManagedDevices que estão agendados para a reforma
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2ae915cf471217c7b053428b376f485e3c04aa1f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017419"
---
# <a name="retirescheduledmanageddevice-resource-type"></a>Tipo de recurso retireScheduledManagedDevice

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

ManagedDevices que estão agendados para a reforma

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|managedDeviceId|Cadeia de caracteres|DeviceId gerenciado|
|managedDeviceName|String|Nome do dispositivo gerenciado|
|deviceType|[deviceType](../resources/intune-deviceconfig-devicetype.md)|Tipo de dispositivo gerenciado. Os valores possíveis são: `desktop` , , , , , , , , `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` , `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `cloudPC` `blackberry` `palm` `unknown` .|
|complianceState|[complianceStatus](../resources/intune-shared-compliancestatus.md)|Managed Device ComplianceStatus. Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|retireAfterDateTime|DateTimeOffset|Dispositivo gerenciado se aposentar após DateTime|
|managementAgent|[managementAgentType](../resources/intune-deviceconfig-managementagenttype.md)|Managed Device ManagementAgentType. Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm` e `windowsManagementCloudApi`.|
|ownerType|[managedDeviceOwnerType](../resources/intune-shared-manageddeviceownertype.md)|Managed Device ManagedDeviceOwnerType. Os valores possíveis são: `unknown`, `company`, `personal`.|
|deviceCompliancePolicyName|Cadeia de caracteres|Nome da política de conformidade do dispositivo|
|deviceCompliancePolicyId|Cadeia de caracteres|Device Compliance PolicyId|
|roleScopeTagIds|Coleção String|Lista de marcas de escopo para esta instância entity.|

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
  "deviceCompliancePolicyId": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```



