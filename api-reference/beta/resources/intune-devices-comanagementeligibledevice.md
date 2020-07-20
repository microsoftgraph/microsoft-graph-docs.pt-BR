---
title: tipo de recurso comanagementEligibleDevice
description: Estado de qualificação para gerenciamento de dispositivos
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 58d6714c2d9e0214286ef9f26c9634b4f16a78f5
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793455"
---
# <a name="comanagementeligibledevice-resource-type"></a>tipo de recurso comanagementEligibleDevice

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado de qualificação para gerenciamento de dispositivos

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar comanagementEligibleDevices](../api/intune-devices-comanagementeligibledevice-list.md)|coleção [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md)|Listar Propriedades e relações dos objetos [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) .|
|[Obter comanagementEligibleDevice](../api/intune-devices-comanagementeligibledevice-get.md)|[comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md)|Leia as propriedades e as relações do objeto [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) .|
|[Criar comanagementEligibleDevice](../api/intune-devices-comanagementeligibledevice-create.md)|[comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md)|Criar um novo objeto [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) .|
|[Excluir comanagementEligibleDevice](../api/intune-devices-comanagementeligibledevice-delete.md)|Nenhuma|Exclui [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md).|
|[Atualizar comanagementEligibleDevice](../api/intune-devices-comanagementeligibledevice-update.md)|[comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md)|Atualiza as propriedades de um objeto [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|ID exclusiva do dispositivo|
|deviceName|String|DeviceName|
|deviceType|[deviceType](../resources/intune-shared-devicetype.md)|DeviceType. Os valores possíveis são:,,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` , `macMDM` , `holoLens` , `surfaceHub` , `androidForWork` , `androidEnterprise` , `windows10x` `androidnGMS` `blackberry` `palm` `unknown` ,,,,,,,,,,,,,.|
|clientRegistrationStatus|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|ClientRegistrationStatus. Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|ownerType|[ownerType](../resources/intune-shared-ownertype.md)|OwnerType. Os valores possíveis são: `unknown`, `company`, `personal`.|
|managementAgents|[managementAgentType](../resources/intune-shared-managementagenttype.md)|ManagementAgents. Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm` e `windowsManagementCloudApi`.|
|ManagementState|[ManagementState](../resources/intune-devices-managementstate.md)|ManagementState. Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.|
|referenceId|String|ReferenceId|
|mdmStatus|String|MDMStatus|
|osVersion|String|OSVersion|
|serialNumber|String|SerialNumber|
|fabricante|String|Fabricantes|
|modelo|String|Modelo|
|osDescription|String|OSDescription|
|EntityName|Int32|EntityName|
|userId|Cadeia de caracteres|UserId|
|UPN|String|UPN|
|userEmail|Cadeia de caracteres|UserEmail|
|userName|String|UserName|
|status|[comanagementEligibleType](../resources/intune-devices-comanagementeligibletype.md)|ComanagementEligibleStatus. Os valores possíveis são: `comanaged`, `eligible`, `eligibleButNotAzureAdJoined`, `needsOsUpdate`, `ineligible`.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.comanagementEligibleDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagementEligibleDevice",
  "id": "String (identifier)",
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
  "status": "String"
}
```



