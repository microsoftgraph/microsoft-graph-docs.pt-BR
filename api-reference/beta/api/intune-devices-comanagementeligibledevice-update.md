---
title: Atualizar comanagementEligibleDevice
description: Atualize as propriedades de um objeto comanagementEligibleDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: af06ad6eb1ade4ae1a994cf60dad9626dfc06344
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671259"
---
# <a name="update-comanagementeligibledevice"></a>Atualizar comanagementEligibleDevice

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/comanagementEligibleDevices/{comanagementEligibleDeviceId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do [objeto comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [o comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID exclusiva do dispositivo|
|deviceName|String|DeviceName|
|deviceType|[Devicetype](../resources/intune-devices-devicetype.md)|Devicetype. Os valores possíveis são: , , , , , , , `winCE`, `iPod``cloudPC``palm``macMDM``blackberry``unix``linux``iSocConsumer``unknown``windows10x``androidnGMS``iPad``chromeOS``androidEnterprise``androidForWork``surfaceHub``holoLens``android``iPhone``winEmbedded`. `windowsPhone``mac``nokia``winMO6``windowsRT``desktop`|
|clientRegistrationStatus|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|ClientRegistrationStatus. Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|Ownertype|[Ownertype](../resources/intune-shared-ownertype.md)|Ownertype. Os valores possíveis são: `unknown`, `company`, `personal`.|
|managementAgents|[managementAgentType](../resources/intune-shared-managementagenttype.md)|ManagementAgents. Os valores possíveis são: , , , , , , , `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, , `googleCloudDevicePolicyController`, `msSense``microsoft365ManagedMdm`, . `intuneAosp``configurationManagerClient``easIntuneClient``intuneClient``easMdm``mdm``eas`|
|managementState|[managementState](../resources/intune-devices-managementstate.md)|ManagementState. Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.|
|referenceId|Cadeia de Caracteres|ReferenceId|
|mdmStatus|String|MDMStatus|
|osVersion|String|OSVersion|
|serialNumber|String|SerialNumber|
|fabricante|String|Fabricante|
|modelo|String|Modelo|
|osDescription|Cadeia de caracteres|OSDescription|
|entitySource|Int32|EntitySource|
|userId|Cadeia de caracteres|UserId|
|Upn|String|UPN|
|userEmail|Cadeia de caracteres|UserEmail|
|userName|Cadeia de caracteres|UserName|
|status|[comanagementEligibleType](../resources/intune-devices-comanagementeligibletype.md)|ComanagementEligibleStatus. Os valores possíveis são: `comanaged`, `eligible`, `eligibleButNotAzureAdJoined`, `needsOsUpdate`, `ineligible`.|



## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna `200 OK` um código de resposta e um objeto [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/comanagementEligibleDevices/{comanagementEligibleDeviceId}
Content-type: application/json
Content-length: 714

{
  "@odata.type": "#microsoft.graph.comanagementEligibleDevice",
  "deviceName": "Device Name value",
  "deviceType": "windowsRT",
  "clientRegistrationStatus": "registered",
  "ownerType": "company",
  "managementAgents": "mdm",
  "managementState": "retirePending",
  "referenceId": "Reference Id value",
  "mdmStatus": "Mdm Status value",
  "osVersion": "Os Version value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "osDescription": "Os Description value",
  "entitySource": 12,
  "userId": "User Id value",
  "upn": "Upn value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "status": "eligible"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 763

{
  "@odata.type": "#microsoft.graph.comanagementEligibleDevice",
  "id": "ac20683b-683b-ac20-3b68-20ac3b6820ac",
  "deviceName": "Device Name value",
  "deviceType": "windowsRT",
  "clientRegistrationStatus": "registered",
  "ownerType": "company",
  "managementAgents": "mdm",
  "managementState": "retirePending",
  "referenceId": "Reference Id value",
  "mdmStatus": "Mdm Status value",
  "osVersion": "Os Version value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "osDescription": "Os Description value",
  "entitySource": 12,
  "userId": "User Id value",
  "upn": "Upn value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "status": "eligible"
}
```




