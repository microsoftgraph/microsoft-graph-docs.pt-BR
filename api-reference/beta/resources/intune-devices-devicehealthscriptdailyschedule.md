---
title: tipo de recurso deviceHealthScriptDailySchedule
description: Agendamento diário do script de integridade do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1ebe7c98cbdc7f0397a1d95c203006f1070716ff
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060360"
---
# <a name="devicehealthscriptdailyschedule-resource-type"></a>tipo de recurso deviceHealthScriptDailySchedule

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Agendamento diário do script de integridade do dispositivo.


Herda de [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|interval|Int32|O valor x de cada x horas para agendamento por hora, a cada x dias para agenda diária, a cada x semanas para agenda semanal, a cada x meses para agenda mensal. Valores válidos de 1 a 23 herdados de [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)|
|useUtc|Booliano|Indique se a hora é UTC ou horário local do cliente. Herdado de [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)|
|time|TimeOfDay|Em que tempo o script está agendado para ser executado. Essa coleção pode conter um máximo de 20 elementos. Herdado de [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptDailySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptDailySchedule",
  "interval": 1024,
  "useUtc": true,
  "time": "String (time of day)"
}
```






