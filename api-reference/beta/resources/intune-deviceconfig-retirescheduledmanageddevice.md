---
title: Tipo de recurso retireScheduledManagedDevice
description: ManagedDevices que estão agendados para desativação
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fdc0d2e97c417d0189805006fc6636aaae4b154b
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66667632"
---
# <a name="retirescheduledmanageddevice-resource-type"></a>Tipo de recurso retireScheduledManagedDevice

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

ManagedDevices que estão agendados para desativação

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|managedDeviceId|Cadeia de caracteres|DeviceId gerenciado|
|managedDeviceName|String|Nome do Dispositivo Gerenciado|
|deviceType|[Devicetype](../resources/intune-deviceconfig-devicetype.md)|Tipo de dispositivo gerenciado. Os valores possíveis são: , , , , , , , `winCE`, `iPod``cloudPC``palm``macMDM``blackberry``unix``linux``iSocConsumer``unknown``windows10x``androidnGMS``iPad``chromeOS``androidEnterprise``androidForWork``surfaceHub``holoLens``android``iPhone``winEmbedded`. `windowsPhone``mac``nokia``winMO6``windowsRT``desktop`|
|complianceState|[complianceStatus](../resources/intune-shared-compliancestatus.md)|Managed Device ComplianceStatus. Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|retireAfterDateTime|DateTimeOffset|Desativação de dispositivo gerenciado após DateTime|
|managementAgent|[managementAgentType](../resources/intune-shared-managementagenttype.md)|Managed Device ManagementAgentType. Os valores possíveis são: , , , , , , , `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, , `googleCloudDevicePolicyController`, `msSense``microsoft365ManagedMdm`, . `intuneAosp``configurationManagerClient``easIntuneClient``intuneClient``easMdm``mdm``eas`|
|Ownertype|[managedDeviceOwnerType](../resources/intune-shared-manageddeviceownertype.md)|ManagedDeviceOwnerType de dispositivo gerenciado. Os valores possíveis são: `unknown`, `company`, `personal`.|
|deviceCompliancePolicyName|Cadeia de caracteres|Nome da Política de Conformidade do Dispositivo|
|deviceCompliancePolicyId|Cadeia de caracteres|PolicyId de Conformidade do Dispositivo|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade.|

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




