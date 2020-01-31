---
title: tipo de recurso comanagementEligibleDeviceEntity
description: tipo de recurso comanagementEligibleDeviceEntity
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e5ad068a348eabaceafd9ca736f27cf6fda3218e
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636550"
---
# <a name="comanagementeligibledeviceentity-resource-type"></a>tipo de recurso comanagementEligibleDeviceEntity

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado da configuração do aplicativo móvel do dispositivo gerenciado para um determinado dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar comanagementEligibleDeviceEntity](../api/intune-device-comanagementEligibleDeviceEntity-list.md)|coleção [comanagementEligibleDeviceEntity](../resources/intune-device-comanagementEligibleDeviceEntity.md)|Listar Propriedades e relações dos objetos [comanagementEligibleDeviceEntity](../resources/intune-device-comanagementEligibleDeviceEntity.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|ID exclusiva do EligibleDeviceEntity|
|deviceId|Cadeia de caracteres|DeviceId|
|deviceName|Cadeia de caracteres|DeviceName|
|deviceType|String|DeviceType|
|clientRegistrationStatus|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|ClientRegistrationStatus. Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|ownerType|[ownerType](../resources/intune-shared-ownertype.md)|OwnerType. Os valores possíveis são: `unknown`, `company`, `personal`.|
|managementAgents|[managementAgentType](../resources/intune-shared-managementagenttype.md)|ManagementAgentType. Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.|
|ManagementState|[ManagementState](../resources/intune-devices-managementstate.md)|ManagementState. Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.|
|referenceId|Cadeia de caracteres|ReferenceId|
|mdmStatus|Cadeia de caracteres|MDMStatus|
|osVersion|Cadeia de caracteres|OSVersion|
|serialNumber|String|SerialNumber|
|fabricante|Cadeia de caracteres|Fabricantes|
|modelo|Cadeia de caracteres|Modelo|
|osDescription|Cadeia de caracteres|OSDescription|
|EntityName|Int32|EntityName|
|userId|Cadeia de caracteres|UserId|
|UPN|Cadeia de caracteres|UPN|
|userEmail|Cadeia de caracteres|UserEmail|
|userName|Cadeia de caracteres|UserName|
|coManageEligibleStatus|[coManagementEligibleType](../resources/intune-devices-comanagementeligibletype.md)|CoManagementEligibleType. Os valores possíveis são: `coManaged`, `eligible`, `eligibleButNotAadJoined`, `needsOSUpdate`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.comanagementEligibleDeviceEntity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagementEligibleDeviceEntity",
  "id": "String (identifier)",
  "deviceId": "String",
  "deviceName": "String",
  "deviceType": "String",
  "clientRegistrationStatus": "String",
  "ownerType": "String",
  "managementAgents": "String",
  "managementState": "String",
  "referenceId": "String",
  "mdmStatus": "String",
  "osVersion": "String",
  "serialNumber": "String",
  "manufacturer": "String",
  "model": "String",
  "osDescription": "String",
  "entitySource": 1024,
  "userId": "String",
  "upn": "String",
  "userEmail": "String",
  "userName": "String",
  "coManageEligibleStatus": "String"
}
```

