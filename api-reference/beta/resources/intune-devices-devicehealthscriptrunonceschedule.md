---
title: Tipo de recurso deviceHealthScriptRunOnceSchedule
description: Script de saúde do dispositivo executado uma vez agendado.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c51150e9299a44495c517e8f78a4e67de3ce47c1
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58802471"
---
# <a name="devicehealthscriptrunonceschedule-resource-type"></a>Tipo de recurso deviceHealthScriptRunOnceSchedule

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Script de saúde do dispositivo executado uma vez agendado.


Herda de [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|interval|Int32|O valor x de cada x horas para agendamento por hora, a cada x dias para o Agendamento Diário, a cada x semanas para agendamento semanal, a cada x meses para Agendamento Mensal. Valores válidos de 1 a 23 Herdados de [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)|
|useUtc|Boleano|Indique se a hora é Utc ou hora local do cliente. Herdado [de deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)|
|hora|TimeOfDay|No momento em que o script é agendado para ser executado. Essa coleção pode conter no máximo 20 elementos. Herdado [de deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)|
|data|Data|A data em que o script está agendado para ser executado. Essa coleção pode conter no máximo 20 elementos.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRunOnceSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunOnceSchedule",
  "interval": 1024,
  "useUtc": true,
  "time": "String (time of day)",
  "date": "String (Date)"
}
```



