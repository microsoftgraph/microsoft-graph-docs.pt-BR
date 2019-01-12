---
title: tipo de recurso de hourlySchedule
description: Agendamento de execução por hora de um script de gerenciamento de dispositivo recorrente.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 004481786fd21ad04e0adbe4e16d3174fc6cc2f4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951884"
---
# <a name="hourlyschedule-resource-type"></a>tipo de recurso de hourlySchedule

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Agendamento de execução por hora de um script de gerenciamento de dispositivo recorrente.

Herda de [runSchedule](../resources/intune-devices-runschedule.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|interval|Int32|Intervalo de número de horas|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hourlySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hourlySchedule",
  "interval": 1024
}
```





