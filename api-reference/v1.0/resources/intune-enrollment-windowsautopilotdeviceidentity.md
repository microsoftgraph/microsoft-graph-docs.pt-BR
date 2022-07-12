---
title: Tipo de recurso windowsAutopilotDeviceIdentity
description: O recurso windowsAutopilotDeviceIdentity representa um dispositivo Windows Autopilot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 74e33481d69f3b8a0d9a2c862bb13494257bfbda
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66729941"
---
# <a name="windowsautopilotdeviceidentity-resource-type"></a>Tipo de recurso windowsAutopilotDeviceIdentity

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso windowsAutopilotDeviceIdentity representa um dispositivo Windows Autopilot.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsAutopilotDeviceIdentities](../api/intune-enrollment-windowsautopilotdeviceidentity-list.md)|[coleção windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Listar propriedades e relações dos objetos [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .|
|[Obter windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-get.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Ler propriedades e relações do objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .|
|[Criar windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-create.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Crie um novo [objeto windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .|
|[Excluir windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-delete.md)|Nenhum|Exclui um [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).|
|[ação assignUserToDevice](../api/intune-enrollment-windowsautopilotdeviceidentity-assignusertodevice.md)|Nenhum|Atribui o usuário a dispositivos do Autopilot.|
|[ação unassignUserFromDevice](../api/intune-enrollment-windowsautopilotdeviceidentity-unassignuserfromdevice.md)|Nenhum|Cancela a atribuição do usuário de um dispositivo do Autopilot.|
|[Ação updateDeviceProperties](../api/intune-enrollment-windowsautopilotdeviceidentity-updatedeviceproperties.md)|Nenhum|Atualizações em dispositivos autopilot.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O GUID do objeto.|
|groupTag|String|Marca de grupo do dispositivo windows autopilot.|
|purchaseOrderIdentifier|String|Identificador do Pedido de Compra do dispositivo Windows Autopilot.|
|serialNumber|Cadeia de caracteres|Número de série do dispositivo do Windows AutoPilot.|
|productKey|Cadeia de caracteres|Chave do produto (Product Key) do dispositivo do Windows AutoPilot.|
|fabricante|String|Fabricante OEM do dispositivo Windows Autopilot.|
|modelo|String|Nome do modelo do dispositivo Windows Autopilot.|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Intune estado de registro do dispositivo Windows Autopilot. Os valores possíveis são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`.|
|lastContactedDateTime|DateTimeOffset|Intune Data e Hora do Último Contato do dispositivo Windows Autopilot.|
|addressableUserName|String|Nome de usuário enderecável.|
|userPrincipalName|String|Nome UPN.|
|resourceName|Cadeia de caracteres|Nome do recurso.|
|skuNumber|String|Número da SKU|
|systemFamily|String|Família do Sistema|
|azureActiveDirectoryDeviceId|String|ID do dispositivo do AAD – a ser preterido|
|managedDeviceId|String|ID do Dispositivo Gerenciado|
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





