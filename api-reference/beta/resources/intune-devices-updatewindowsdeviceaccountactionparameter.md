---
title: Tipo de recurso updateWindowsDeviceAccountActionParameter
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fd5ed6f461455b577e695fc10b5061139f8317e0
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58788469"
---
# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a>Tipo de recurso updateWindowsDeviceAccountActionParameter

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|deviceAccount|[windowsDeviceAccount](../resources/intune-devices-windowsdeviceaccount.md)|Ainda não documentado|
|passwordRotationEnabled|Booliano|Ainda não documentado|
|calendarSyncEnabled|Booliano|Ainda não documentado|
|deviceAccountEmail|Cadeia de caracteres|Ainda não documentado|
|exchangeServer|Cadeia de caracteres|Ainda não documentado|
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



