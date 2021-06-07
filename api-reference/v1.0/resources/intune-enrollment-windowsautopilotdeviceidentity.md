---
title: Tipo de recurso windowsAutopilotDeviceIdentity
description: O recurso windowsAutopilotDeviceIdentity representa um Windows Autopilot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6267d113bbd8324941f6711d5eedb42939fbe57b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752823"
---
# <a name="windowsautopilotdeviceidentity-resource-type"></a>Tipo de recurso windowsAutopilotDeviceIdentity

Namespace: microsoft.graph

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

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O GUID do objeto.|
|groupTag|String|Marca de grupo do dispositivo Windows piloto automático.|
|purchaseOrderIdentifier|String|Purchase Order Identifier of the Windows autopilot device.|
|serialNumber|Cadeia de caracteres|Número de série do dispositivo do Windows AutoPilot.|
|productKey|Cadeia de caracteres|Chave do produto (Product Key) do dispositivo do Windows AutoPilot.|
|fabricante|String|Fabricante Oem do dispositivo Windows piloto automático.|
|modelo|String|Nome do modelo do dispositivo Windows piloto automático.|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Estado de registro do intune do dispositivo Windows piloto automático. Os valores possíveis são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`.|
|lastContactedDateTime|DateTimeOffset|Intune Last Contacted Date Time of the Windows autopilot device.|
|addressableUserName|String|Nome de usuário acessível.|
|userPrincipalName|String|Nome principal do usuário.|
|resourceName|Cadeia de caracteres|Nome do recurso.|
|skuNumber|String|Número SKU|
|systemFamily|String|Família do Sistema|
|azureActiveDirectoryDeviceId|String|ID do dispositivo AAD - a ser preterida|
|managedDeviceId|String|ID de dispositivo gerenciado|
|displayName|String|Nome de exibição|

## <a name="relationships"></a>Relações
Nenhum

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
  "managedDeviceId": "String",
  "displayName": "String"
}
```




