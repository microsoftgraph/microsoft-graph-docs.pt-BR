---
title: tipo de recurso de windows10AppsForceUpdateSchedule
description: Agendamento de atualização do Windows 10 force para aplicativos
author: tfitzmac
ms.openlocfilehash: 851f22e092f2669dfc44911783df6182cda1dc6d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323699"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a>tipo de recurso de windows10AppsForceUpdateSchedule

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Agendamento de atualização do Windows 10 force para aplicativos
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|startDateTime|DateTimeOffset|A hora de início para a força reinicie.|
|recurrence|[windows10AppsUpdateRecurrence](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|Plano de recorrência. Os valores possíveis são: `none`, `daily`, `weekly`, `monthly`.|
|runImmediatelyIfAfterStartDateTime|Boolean|Se for true, executa a tarefa imediatamente se StartDateTime está no passado, para outro, será executada na próxima recorrência.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AppsForceUpdateSchedule",
  "startDateTime": "String (timestamp)",
  "recurrence": "String",
  "runImmediatelyIfAfterStartDateTime": true
}
```





