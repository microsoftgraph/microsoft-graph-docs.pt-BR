---
title: Tipo de recurso windowsInformationProtectionWipeAction
description: Representa solicitações de limpeza emitidas pelo administrador de locatários para dispositivos de Windows Bring-Your-Own-Device(BYOD).
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c4ac271963c30dbff4de8af3aec8c2a601daf7a5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59068722"
---
# <a name="windowsinformationprotectionwipeaction-resource-type"></a>Tipo de recurso windowsInformationProtectionWipeAction

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa solicitações de limpeza emitidas pelo administrador de locatários para dispositivos de Windows Bring-Your-Own-Device(BYOD).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsInformationProtectionWipeActions](../api/intune-mam-windowsinformationprotectionwipeaction-list.md)|[Coleção windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|Listar propriedades e relações dos [objetos windowsInformationProtectionWipeAction.](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|
|[Obter windowsInformationProtectionWipeAction](../api/intune-mam-windowsinformationprotectionwipeaction-get.md)|[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|Ler propriedades e relações do [objeto windowsInformationProtectionWipeAction.](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|
|[Criar windowsInformationProtectionWipeAction](../api/intune-mam-windowsinformationprotectionwipeaction-create.md)|[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|Crie um novo [objeto windowsInformationProtectionWipeAction.](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|
|[Excluir windowsInformationProtectionWipeAction](../api/intune-mam-windowsinformationprotectionwipeaction-delete.md)|Nenhum|Exclui um [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).|
|[Atualizar windowsInformationProtectionWipeAction](../api/intune-mam-windowsinformationprotectionwipeaction-update.md)|[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|Atualize as propriedades de um [objeto windowsInformationProtectionWipeAction.](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|status|[actionState](../resources/intune-shared-actionstate.md)|Limpar o status da ação. Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|targetedUserId|String|O UserId que está sendo direcionado por essa ação de limpeza.|
|targetedDeviceRegistrationId|Cadeia de Caracteres|O DeviceRegistrationId que está sendo direcionado por essa ação de limpeza.|
|targetedDeviceName|Cadeia de Caracteres|Nome do dispositivo direcionado.|
|targetedDeviceMacAddress|Cadeia de Caracteres|Endereço Mac do dispositivo direcionado.|
|lastCheckInDateTime|DateTimeOffset|Última verificação no momento do dispositivo que foi direcionado por essa ação de limpeza.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionWipeAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "id": "String (identifier)",
  "status": "String",
  "targetedUserId": "String",
  "targetedDeviceRegistrationId": "String",
  "targetedDeviceName": "String",
  "targetedDeviceMacAddress": "String",
  "lastCheckInDateTime": "String (timestamp)"
}
```



