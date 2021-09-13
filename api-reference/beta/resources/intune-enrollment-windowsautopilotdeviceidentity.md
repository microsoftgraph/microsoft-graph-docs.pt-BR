---
title: Tipo de recurso windowsAutopilotDeviceIdentity
description: O recurso windowsAutopilotDeviceIdentity representa um Windows Autopilot.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 18988b5a22e84ae97e412ae0dfc7daab738027b2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59054286"
---
# <a name="windowsautopilotdeviceidentity-resource-type"></a>Tipo de recurso windowsAutopilotDeviceIdentity

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso windowsAutopilotDeviceIdentity representa um Windows Autopilot.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsAutopilotDeviceIdentities](../api/intune-enrollment-windowsautopilotdeviceidentity-list.md)|[Coleção windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Listar propriedades e relações dos [objetos windowsAutopilotDeviceIdentity.](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|
|[Obter windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-get.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Ler propriedades e relações do [objeto windowsAutopilotDeviceIdentity.](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|
|[Criar windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-create.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Crie um novo [objeto windowsAutopilotDeviceIdentity.](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|
|[Excluir windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-delete.md)|Nenhum|Exclui um [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).|
|[ação assignUserToDevice](../api/intune-enrollment-windowsautopilotdeviceidentity-assignusertodevice.md)|Nenhum|Atribui o usuário a dispositivos autopilot.|
|[ação unassignUserFromDevice](../api/intune-enrollment-windowsautopilotdeviceidentity-unassignuserfromdevice.md)|Nenhum|Desaigna o usuário de um dispositivo autopilot.|
|[Ação updateDeviceProperties](../api/intune-enrollment-windowsautopilotdeviceidentity-updatedeviceproperties.md)|Nenhum|Atualiza as propriedades em dispositivos do Autopilot.|
|[Ação assignResourceAccountToDevice](../api/intune-enrollment-windowsautopilotdeviceidentity-assignresourceaccounttodevice.md)|Nenhum|Atribui conta de recurso a dispositivos autopilot.|
|[Ação unassignResourceAccountFromDevice](../api/intune-enrollment-windowsautopilotdeviceidentity-unassignresourceaccountfromdevice.md)|Nenhum|Desaigna a conta de recurso de um dispositivo Autopilot.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O GUID do objeto.|
|deploymentProfileAssignmentStatus|[windowsAutopilotProfileAssignmentStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|Status de atribuição de perfil do dispositivo Windows piloto automático. Os valores possíveis são: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.|
|deploymentProfileAssignmentDetailedStatus|[windowsAutopilotProfileAssignmentDetailedStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|Status detalhado da atribuição de perfil do dispositivo Windows piloto automático. Os valores possíveis são: `none`, `hardwareRequirementsNotMet`, `surfaceHubProfileNotSupported`, `holoLensProfileNotSupported`, `windowsPcProfileNotSupported`.|
|deploymentProfileAssignedDateTime|DateTimeOffset|Hora do conjunto de perfis do dispositivo Windows piloto automático.|
|groupTag|Cadeia de Caracteres|Marca de grupo do dispositivo Windows piloto automático.|
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
|skuNumber|Cadeia de Caracteres|Número SKU|
|systemFamily|Cadeia de Caracteres|Família do Sistema|
|azureActiveDirectoryDeviceId|Cadeia de Caracteres|ID do dispositivo AAD - a ser preterida|
|azureAdDeviceId|Cadeia de Caracteres|ID do dispositivo AAD|
|managedDeviceId|Cadeia de Caracteres|ID de dispositivo gerenciado|
|displayName|Cadeia de caracteres|Nome de exibição|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|deploymentProfile|[windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|Perfil de implantação atualmente atribuído ao dispositivo Windows piloto automático.|
|intendedDeploymentProfile|[windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|Perfil de implantação destinado a ser atribuído ao dispositivo Windows piloto automático.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "String (identifier)",
  "deploymentProfileAssignmentStatus": "String",
  "deploymentProfileAssignmentDetailedStatus": "String",
  "deploymentProfileAssignedDateTime": "String (timestamp)",
  "groupTag": "String",
  "purchaseOrderIdentifier": "String",
  "serialNumber": "String",
  "productKey": "String",
  "manufacturer": "String",
  "model": "String",
  "enrollmentState": "String",
  "lastContactedDateTime": "String (timestamp)",
  "addressableUserName": "String",
  "userPrincipalName": "String",
  "resourceName": "String",
  "skuNumber": "String",
  "systemFamily": "String",
  "azureActiveDirectoryDeviceId": "String",
  "azureAdDeviceId": "String",
  "managedDeviceId": "String",
  "displayName": "String"
}
```



