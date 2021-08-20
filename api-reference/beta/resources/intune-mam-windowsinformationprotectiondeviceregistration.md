---
title: Tipo de recurso windowsInformationProtectionDeviceRegistration
description: Representa registros de registro de dispositivo para dispositivos de Windows Bring-Your-Own-Device(BYOD).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 68c8ed0f9c4b214d95d286db00a4732587ce188fa548219181048b4ea13705c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54248269"
---
# <a name="windowsinformationprotectiondeviceregistration-resource-type"></a>Tipo de recurso windowsInformationProtectionDeviceRegistration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa registros de registro de dispositivo para dispositivos de Windows Bring-Your-Own-Device(BYOD).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsInformationProtectionDeviceRegistrations](../api/intune-mam-windowsinformationprotectiondeviceregistration-list.md)|[Coleção windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|Listar propriedades e relações dos [objetos windowsInformationProtectionDeviceRegistration.](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|
|[Obter windowsInformationProtectionDeviceRegistration](../api/intune-mam-windowsinformationprotectiondeviceregistration-get.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|Leia propriedades e relações do [objeto windowsInformationProtectionDeviceRegistration.](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|
|[Criar windowsInformationProtectionDeviceRegistration](../api/intune-mam-windowsinformationprotectiondeviceregistration-create.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|Crie um novo [objeto windowsInformationProtectionDeviceRegistration.](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|
|[Excluir windowsInformationProtectionDeviceRegistration](../api/intune-mam-windowsinformationprotectiondeviceregistration-delete.md)|Nenhum|Exclui um [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).|
|[Atualizar windowsInformationProtectionDeviceRegistration](../api/intune-mam-windowsinformationprotectiondeviceregistration-update.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|Atualize as propriedades de um [objeto windowsInformationProtectionDeviceRegistration.](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|
|[Ação wipe](../api/intune-mam-windowsinformationprotectiondeviceregistration-wipe.md)|Nenhum|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|userId|Cadeia de caracteres|UserId associado a esse registro de dispositivo.|
|deviceRegistrationId|Cadeia de caracteres|Identificador de dispositivo para esse registro de dispositivo.|
|deviceName|Cadeia de caracteres|Nome do dispositivo.|
|deviceType|String|Tipo de dispositivo, por exemplo, Windows laptop VS Windows telefone.|
|deviceMacAddress|Cadeia de caracteres|Endereço do Device Mac.|
|lastCheckInDateTime|DateTimeOffset|Última verificação na hora do dispositivo.|

## <a name="relationships"></a>Relações
Nenhum

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




