---
title: Tipo de recurso managedDeviceSummarizedAppState
description: Evento representando dispositivos de um usuário com aplicativos com falha ou pendentes.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 910bcf04f7d2578ab4b643951b844ef4eef2d881
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58264511"
---
# <a name="manageddevicesummarizedappstate-resource-type"></a>Tipo de recurso managedDeviceSummarizedAppState

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Evento representando dispositivos de um usuário com aplicativos com falha ou pendentes.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|summarizedAppState|[runState](../resources/intune-troubleshooting-runstate.md)|runState para o objeto. Os possíveis valores são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|deviceId|Cadeia de caracteres|DeviceId do dispositivo representado por este objeto|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceSummarizedAppState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceSummarizedAppState",
  "summarizedAppState": "String",
  "deviceId": "String"
}
```




