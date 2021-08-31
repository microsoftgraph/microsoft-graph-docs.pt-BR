---
title: Tipo de recurso deviceManagementIntentDeviceState
description: Entidade que representa o estado do dispositivo para uma intenção
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5a1eec4f8073a3ad0032483bbfe60a9d71280238
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58792572"
---
# <a name="devicemanagementintentdevicestate-resource-type"></a>Tipo de recurso deviceManagementIntentDeviceState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa o estado do dispositivo para uma intenção

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementIntentDeviceStates](../api/intune-deviceintent-devicemanagementintentdevicestate-list.md)|[Coleção deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|Listar propriedades e relações dos [objetos deviceManagementIntentDeviceState.](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|
|[Obter deviceManagementIntentDeviceState](../api/intune-deviceintent-devicemanagementintentdevicestate-get.md)|[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|Ler propriedades e relações do [objeto deviceManagementIntentDeviceState.](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|
|[Criar deviceManagementIntentDeviceState](../api/intune-deviceintent-devicemanagementintentdevicestate-create.md)|[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|Crie um novo [objeto deviceManagementIntentDeviceState.](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|
|[Excluir deviceManagementIntentDeviceState](../api/intune-deviceintent-devicemanagementintentdevicestate-delete.md)|Nenhum(a)|Exclui um [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md).|
|[Atualizar deviceManagementIntentDeviceState](../api/intune-deviceintent-devicemanagementintentdevicestate-update.md)|[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|Atualize as propriedades de [um objeto deviceManagementIntentDeviceState.](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID|
|userPrincipalName|Cadeia de caracteres|O nome principal do usuário que está sendo relatado em um dispositivo|
|userName|Cadeia de caracteres|O nome de usuário que está sendo relatado em um dispositivo|
|deviceDisplayName|Cadeia de caracteres|Nome do dispositivo que está sendo relatado|
|lastReportedDateTime|DateTimeOffset|Data da última modificação de um relatório de intenção|
|state|[complianceStatus](../resources/intune-shared-compliancestatus.md)|Estado do dispositivo para uma intenção. Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|deviceId|Cadeia de caracteres|ID do dispositivo que está sendo relatada|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "userName": "String",
  "deviceDisplayName": "String",
  "lastReportedDateTime": "String (timestamp)",
  "state": "String",
  "deviceId": "String"
}
```



