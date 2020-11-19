---
title: tipo de recurso windowsKioskForceUpdateSchedule
description: Agendamento de atualização forçada do Windows 10 para dispositivos quiosque.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a3dd2e5872a60884050cd7a32408288955e94f92
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49276165"
---
# <a name="windowskioskforceupdateschedule-resource-type"></a>tipo de recurso windowsKioskForceUpdateSchedule

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Agendamento de atualização forçada do Windows 10 para dispositivos quiosque.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|startDateTime|DateTimeOffset|A hora de início da reinicialização forçada.|
|recurrence|[windows10AppsUpdateRecurrence](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|Agenda de recorrência. Os valores possíveis são: `none`, `daily`, `weekly`, `monthly`.|
|dayofWeek|[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)|Dia da semana. Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|dayofMonth|Int32|Dia do mês. Valores válidos de 1 a 31|
|runImmediatelyIfAfterStartDateTime|Booliano|Se true, executará a tarefa imediatamente se StartDatetime estiver no passado, senão, será executado na próxima recorrência.|

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




