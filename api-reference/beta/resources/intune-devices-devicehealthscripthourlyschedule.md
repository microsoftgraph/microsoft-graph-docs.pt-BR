---
title: Tipo de recurso deviceHealthScriptHourlySchedule
description: Tipo de script de saúde do dispositivo agendado por hora.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6128f3d16a3d64858871903131e4c799de03415d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59023469"
---
# <a name="devicehealthscripthourlyschedule-resource-type"></a>Tipo de recurso deviceHealthScriptHourlySchedule

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo de script de saúde do dispositivo agendado por hora.


Herda de [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|interval|Int32|O valor x de cada x horas para agendamento por hora, a cada x dias para o Agendamento Diário, a cada x semanas para agendamento semanal, a cada x meses para Agendamento Mensal. Valores válidos de 1 a 23 Herdados de [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)|

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



