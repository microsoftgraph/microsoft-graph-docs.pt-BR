---
title: Tipo de recurso deletedWindowsAutopilotDeviceState
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 87113449f0c00722f3aa1d3a1e614873524d43a6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146739"
---
# <a name="deletedwindowsautopilotdevicestate-resource-type"></a>Tipo de recurso deletedWindowsAutopilotDeviceState

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|serialNumber|String|Número de série do dispositivo Autopilot|
|deviceRegistrationId|Cadeia de caracteres|ID de Registro de Dispositivo ZTD .|
|deletionState|[windowsAutopilotDeviceDeletionState](../resources/intune-enrollment-windowsautopilotdevicedeletionstate.md)|Estado de exclusão de dispositivo. Os valores possíveis são: `unknown`, `failed`, `accepted`, `error`.|
|errorMessage|Cadeia de caracteres|Mensagem de erro de exclusão de dispositivo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deletedWindowsAutopilotDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deletedWindowsAutopilotDeviceState",
  "serialNumber": "String",
  "deviceRegistrationId": "String",
  "deletionState": "String",
  "errorMessage": "String"
}
```




