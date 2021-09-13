---
title: Criar windowsAutopilotDeviceIdentity
description: Crie um novo objeto windowsAutopilotDeviceIdentity.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b6e7ea79b5f487963ea495b0125973fa7767ccc3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59076954"
---
# <a name="create-windowsautopilotdeviceidentity"></a>Criar windowsAutopilotDeviceIdentity

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto windowsAutopilotDeviceIdentity.](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto windowsAutopilotDeviceIdentity.

A tabela a seguir mostra as propriedades necessárias ao criar o windowsAutopilotDeviceIdentity.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O GUID do objeto.|
|deploymentProfileAssignmentStatus|[windowsAutopilotProfileAssignmentStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|Status de atribuição de perfil do dispositivo Windows piloto automático. Os valores possíveis são: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.|
|deploymentProfileAssignmentDetailedStatus|[windowsAutopilotProfileAssignmentDetailedStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|Status detalhado da atribuição de perfil do dispositivo Windows piloto automático. Os valores possíveis são: `none`, `hardwareRequirementsNotMet`, `surfaceHubProfileNotSupported`, `holoLensProfileNotSupported`, `windowsPcProfileNotSupported`.|
|deploymentProfileAssignedDateTime|DateTimeOffset|Hora do conjunto de perfis do dispositivo Windows piloto automático.|
|groupTag|String|Marca de grupo do dispositivo Windows piloto automático.|
|purchaseOrderIdentifier|Cadeia de Caracteres|Purchase Order Identifier of the Windows autopilot device.|
|serialNumber|Cadeia de caracteres|Número de série do dispositivo do Windows AutoPilot.|
|productKey|Cadeia de caracteres|Chave do produto (Product Key) do dispositivo do Windows AutoPilot.|
|fabricante|String|Fabricante Oem do dispositivo Windows piloto automático.|
|modelo|String|Nome do modelo do dispositivo Windows piloto automático.|
|enrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Estado de registro do intune do dispositivo Windows piloto automático. Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|lastContactedDateTime|DateTimeOffset|Intune Last Contacted Date Time of the Windows autopilot device.|
|addressableUserName|Cadeia de Caracteres|Nome de usuário acessível.|
|userPrincipalName|Cadeia de caracteres|Nome principal do usuário.|
|resourceName|Cadeia de caracteres|Nome do recurso.|
|skuNumber|String|Número SKU|
|systemFamily|Cadeia de Caracteres|Família do Sistema|
|azureActiveDirectoryDeviceId|String|ID do dispositivo AAD - a ser preterida|
|azureAdDeviceId|Cadeia de caracteres|ID do dispositivo AAD|
|managedDeviceId|Cadeia de Caracteres|ID de dispositivo gerenciado|
|displayName|String|Nome de exibição|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 1077

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
  "groupTag": "Group Tag value",
  "purchaseOrderIdentifier": "Purchase Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "enrollmentState": "enrolled",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "addressableUserName": "Addressable User Name value",
  "userPrincipalName": "User Principal Name value",
  "resourceName": "Resource Name value",
  "skuNumber": "Sku Number value",
  "systemFamily": "System Family value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "azureAdDeviceId": "Azure Ad Device Id value",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1126

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
  "groupTag": "Group Tag value",
  "purchaseOrderIdentifier": "Purchase Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "enrollmentState": "enrolled",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "addressableUserName": "Addressable User Name value",
  "userPrincipalName": "User Principal Name value",
  "resourceName": "Resource Name value",
  "skuNumber": "Sku Number value",
  "systemFamily": "System Family value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "azureAdDeviceId": "Azure Ad Device Id value",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value"
}
```



