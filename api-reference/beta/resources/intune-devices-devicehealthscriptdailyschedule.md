---
title: Tipo de recurso deviceHealthScriptDailySchedule
description: Agenda diária do script de saúde do dispositivo.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1b73d9020e3d95e658b67e090b311ecc97fe3bc1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017363"
---
# <a name="devicehealthscriptdailyschedule-resource-type"></a>Tipo de recurso deviceHealthScriptDailySchedule

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Agenda diária do script de saúde do dispositivo.


Herda de [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|interval|Int32|O valor x de cada x horas para agendamento por hora, a cada x dias para o Agendamento Diário, a cada x semanas para agendamento semanal, a cada x meses para Agendamento Mensal. Valores válidos de 1 a 23 Herdados de [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)|
|useUtc|Booliano|Indique se a hora é Utc ou hora local do cliente. Herdado [de deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)|
|hora|TimeOfDay|No momento em que o script é agendado para ser executado. Essa coleção pode conter no máximo 20 elementos. Herdado [de deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)|

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



