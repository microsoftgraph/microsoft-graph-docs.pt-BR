---
title: tipo de recurso deviceHealthScriptHourlySchedule
description: Tipo de script de integridade do dispositivo agendamento por hora.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d2276d95d09a1628b07d3b9bc87381b0d85d431f
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44176104"
---
# <a name="devicehealthscripthourlyschedule-resource-type"></a>tipo de recurso deviceHealthScriptHourlySchedule

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo de script de integridade do dispositivo agendamento por hora.


Herda de [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|interval|Int32|O valor x de cada x horas para agendamento por hora, a cada x dias para agenda diária, a cada x semanas para agenda semanal, a cada x meses para agenda mensal. Valores válidos de 1 a 23 herdados de [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptHourlySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptHourlySchedule",
  "interval": 1024
}
```



