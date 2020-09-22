---
title: tipo de recurso deviceHealthScriptBooleanParameter
description: Propriedades do parâmetro de script Booolean.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5474d5e9d61bf97da05ab7931694581349bad6d9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060402"
---
# <a name="devicehealthscriptbooleanparameter-resource-type"></a>tipo de recurso deviceHealthScriptBooleanParameter

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Propriedades do parâmetro de script Booolean.


Herda de [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|name|Cadeia de caracteres|O nome do parâmetro herdado de [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|
|description|String|A descrição do parâmetro herdado de [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|
|isRequired|Booliano|Se o parâmetro obrigatório é herdado de [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|
|applyDefaultValueWhenNotAssigned|Booliano|Se aplica DefaultValue quando não atribuído herdado de [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|
|defaultValue|Booliano|O valor padrão do parâmetro Boolean|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptBooleanParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptBooleanParameter",
  "name": "String",
  "description": "String",
  "isRequired": true,
  "applyDefaultValueWhenNotAssigned": true,
  "defaultValue": true
}
```






