---
title: Tipo de recurso managedDeviceSummarizedAppState
description: Evento representando dispositivos de um usuário com aplicativos com falha ou pendentes.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 092dfef55500ec023c2cf0d79f63c5161c27c7c0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057198"
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




