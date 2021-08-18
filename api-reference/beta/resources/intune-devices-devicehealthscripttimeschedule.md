---
title: Tipo de recurso deviceHealthScriptTimeSchedule
description: Tipo base do cronograma de tempo do script de saúde do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d9f13ec9c3913cadbfb99b37416e24903bb823e2b551a26b1ba27f9933e609c7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54232584"
---
# <a name="devicehealthscripttimeschedule-resource-type"></a>Tipo de recurso deviceHealthScriptTimeSchedule

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo base do cronograma de tempo do script de saúde do dispositivo.


Herda de [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|interval|Int32|O valor x de cada x horas para agendamento por hora, a cada x dias para o Agendamento Diário, a cada x semanas para agendamento semanal, a cada x meses para Agendamento Mensal. Valores válidos de 1 a 23 Herdados de [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)|
|useUtc|Boolean|Indique se a hora é Utc ou hora local do cliente.|
|hora|TimeOfDay|No momento em que o script é agendado para ser executado. Essa coleção pode conter no máximo 20 elementos.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptTimeSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptTimeSchedule",
  "interval": 1024,
  "useUtc": true,
  "time": "String (time of day)"
}
```




