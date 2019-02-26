---
title: Tipo de recurso deviceActionResult
description: Resultado de ação de dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d08b4285f81c7b6f7e4962c4738279f84ba37b7d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261044"
---
# <a name="deviceactionresult-resource-type"></a>Tipo de recurso deviceActionResult

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Resultado de ação de dispositivo

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|actionName|Cadeia de caracteres|Nome da ação|
|actionState|[actionState](../resources/intune-devices-actionstate.md)|Estado da ação. Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|startDateTime|DateTimeOffset|Hora em que a ação foi iniciada|
|lastUpdatedDateTime|DateTimeOffset|Hora da última atualização do estado da ação|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```



