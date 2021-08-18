---
title: Tipo de recurso windowsKioskForceUpdateSchedule
description: Windows 10 forçar o agendamento de atualização para dispositivos Kiosk.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 18b6938740db45281ef06529b8b98546fa1f2d169313a3c263a7d616140ea081
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54226332"
---
# <a name="windowskioskforceupdateschedule-resource-type"></a>Tipo de recurso windowsKioskForceUpdateSchedule

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Windows 10 forçar o agendamento de atualização para dispositivos Kiosk.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|startDateTime|DateTimeOffset|A hora de início da reinicialização da força.|
|recurrence|[windows10AppsUpdateRecurrence](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|Agendamento de recorrência. Os valores possíveis são: `none`, `daily`, `weekly`, `monthly`.|
|dayofWeek|[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)|Dia da semana. Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|dayofMonth|Int32|Dia do mês. Valores válidos de 1 a 31|
|runImmediatelyIfAfterStartDateTime|Boolean|Se true, executa a tarefa imediatamente se StartDateTime estiver no passado, senão, será executado na próxima recorrência.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskForceUpdateSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskForceUpdateSchedule",
  "startDateTime": "String (timestamp)",
  "recurrence": "String",
  "dayofWeek": "String",
  "dayofMonth": 1024,
  "runImmediatelyIfAfterStartDateTime": true
}
```




