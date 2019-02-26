---
title: tipo de recurso windowsInformationProtectionDeviceRegistration
description: Representa os registros de registro de dispositivo para os dispositivos do Windows do BYOD (de acompanhamento de dispositivos).
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4d4403ae2e4629a330fadd5136530d66c8a7d7f2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161674"
---
# <a name="windowsinformationprotectiondeviceregistration-resource-type"></a>tipo de recurso windowsInformationProtectionDeviceRegistration

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa os registros de registro de dispositivo para os dispositivos do Windows do BYOD (de acompanhamento de dispositivos).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsInformationProtectionDeviceRegistrations](../api/intune-mam-windowsinformationprotectiondeviceregistration-list.md)|coleção [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|Listar Propriedades e relações dos objetos [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .|
|[Obter windowsInformationProtectionDeviceRegistration](../api/intune-mam-windowsinformationprotectiondeviceregistration-get.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|Leia as propriedades e as relações do objeto [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .|
|[Criar windowsInformationProtectionDeviceRegistration](../api/intune-mam-windowsinformationprotectiondeviceregistration-create.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|Criar um novo objeto [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .|
|[Excluir windowsInformationProtectionDeviceRegistration](../api/intune-mam-windowsinformationprotectiondeviceregistration-delete.md)|Nenhum|Exclui [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).|
|[Atualizar windowsInformationProtectionDeviceRegistration](../api/intune-mam-windowsinformationprotectiondeviceregistration-update.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|Atualiza as propriedades de um objeto [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .|
|[Ação wipe](../api/intune-mam-windowsinformationprotectiondeviceregistration-wipe.md)|Nenhum|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|userId|String|UserId associado a este registro de registro de dispositivo.|
|deviceRegistrationId|Cadeia de caracteres|Identificador de dispositivo para este registro de registro de dispositivo.|
|deviceName|Cadeia de caracteres|Nome do dispositivo.|
|deviceType|String|Tipo de dispositivo, por exemplo, Windows laptop VS Windows Phone.|
|deviceMacAddress|String|Endereço MAC do dispositivo.|
|lastCheckInDateTime|DateTimeOffset|Hora da última verificação do dispositivo.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDeviceRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
  "id": "String (identifier)",
  "userId": "String",
  "deviceRegistrationId": "String",
  "deviceName": "String",
  "deviceType": "String",
  "deviceMacAddress": "String",
  "lastCheckInDateTime": "String (timestamp)"
}
```




