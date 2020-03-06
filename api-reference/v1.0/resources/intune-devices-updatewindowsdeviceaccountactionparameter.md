---
title: Tipo de recurso updateWindowsDeviceAccountActionParameter
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d349128b6b2e415f3930dc3938c354f890073629
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533237"
---
# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a>Tipo de recurso updateWindowsDeviceAccountActionParameter

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|deviceAccount|[windowsDeviceAccount](../resources/intune-devices-windowsdeviceaccount.md)|Ainda não documentado|
|passwordRotationEnabled|Booliano|Ainda não documentado|
|calendarSyncEnabled|Booliano|Ainda não documentado|
|deviceAccountEmail|String|Ainda não documentado|
|exchangeServer|String|Ainda não documentado|
|sessionInitiationProtocalAddress|Cadeia de caracteres|Ainda não documentado|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.updateWindowsDeviceAccountActionParameter",
  "deviceAccount": {
    "@odata.type": "microsoft.graph.windowsDeviceAccount",
    "password": "String"
  },
  "passwordRotationEnabled": true,
  "calendarSyncEnabled": true,
  "deviceAccountEmail": "String",
  "exchangeServer": "String",
  "sessionInitiationProtocalAddress": "String"
}
```




