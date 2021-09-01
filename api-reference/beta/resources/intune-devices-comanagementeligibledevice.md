---
title: Tipo de recurso comanagementEligibleDevice
description: Estado Co-Management de qualificação do dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 647554e93a790787d7acc4eb05a6e0bca5afe6d2
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58806632"
---
# <a name="comanagementeligibledevice-resource-type"></a>Tipo de recurso comanagementEligibleDevice

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado Co-Management de qualificação do dispositivo

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar comanagementEligibleDevices](../api/intune-devices-comanagementeligibledevice-list.md)|[Coleção comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md)|Listar propriedades e relações dos [objetos comanagementEligibleDevice.](../resources/intune-devices-comanagementeligibledevice.md)|
|[Obter comanagementEligibleDevice](../api/intune-devices-comanagementeligibledevice-get.md)|[comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md)|Leia propriedades e relações do [objeto comanagementEligibleDevice.](../resources/intune-devices-comanagementeligibledevice.md)|
|[Criar comanagementEligibleDevice](../api/intune-devices-comanagementeligibledevice-create.md)|[comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md)|Crie um [novo objeto comanagementEligibleDevice.](../resources/intune-devices-comanagementeligibledevice.md)|
|[Excluir comanagementEligibleDevice](../api/intune-devices-comanagementeligibledevice-delete.md)|Nenhum(a)|Exclui um [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md).|
|[Atualizar comanagementEligibleDevice](../api/intune-devices-comanagementeligibledevice-update.md)|[comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md)|Atualize as propriedades de [um objeto comanagementEligibleDevice.](../resources/intune-devices-comanagementeligibledevice.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID exclusiva do dispositivo|
|deviceName|String|DeviceName|
|deviceType|[deviceType](../resources/intune-devices-devicetype.md)|DeviceType. Os valores possíveis são: `desktop` , , , , , , , `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` , `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `chromeOS` `linux` `blackberry` `palm` `unknown` `cloudPC`|
|clientRegistrationStatus|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|ClientRegistrationStatus. Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|ownerType|[ownerType](../resources/intune-shared-ownertype.md)|OwnerType. Os valores possíveis são: `unknown`, `company`, `personal`.|
|managementAgents|[managementAgentType](../resources/intune-devices-managementagenttype.md)|ManagementAgents. Os valores possíveis são: `eas` , , , , , , , , , `mdm` , , `easMdm` , , , `intuneClient` , `easIntuneClient` `configurationManagerClient` `configurationManagerClientMdm` `configurationManagerClientMdmEas` `unknown` `jamf` `googleCloudDevicePolicyController` `microsoft365ManagedMdm` `msSense` `intuneAosp` .|
|managementState|[managementState](../resources/intune-devices-managementstate.md)|ManagementState. Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.|
|referenceId|Cadeia de caracteres|ReferenceId|
|mdmStatus|Cadeia de caracteres|MDMStatus|
|osVersion|String|OSVersion|
|serialNumber|String|SerialNumber|
|fabricante|String|Fabricante|
|modelo|String|Modelo|
|osDescription|Cadeia de caracteres|OSDescription|
|entitySource|Int32|EntitySource|
|userId|Cadeia de caracteres|UserId|
|upn|Cadeia de caracteres|UPN|
|userEmail|Cadeia de caracteres|UserEmail|
|userName|Cadeia de caracteres|UserName|
|status|[comanagementEligibleType](../resources/intune-devices-comanagementeligibletype.md)|ComanagementEligibleStatus. Os valores possíveis são: `comanaged`, `eligible`, `eligibleButNotAzureAdJoined`, `needsOsUpdate`, `ineligible`.|

## <a name="relationships"></a>Relações
Nenhum

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



