---
title: Tipo de recurso deviceManagementSettings
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f973f2645b37375641bc536b5ace0fa508fb0b0e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854415"
---
# <a name="devicemanagementsettings-resource-type"></a>Tipo de recurso deviceManagementSettings

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Ainda não documentado
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|deviceComplianceCheckinThresholdDays|Int32|O número de dias que tem um dispositivo pode ser executado sem fazer check-in para permanecer em conformidade. Valores válidos de 0 a 120|
|isScheduledActionEnabled|Booliano|O recurso está habilitado ou não para ação agendada para a regra.|
|secureByDefault|Booliano|Quando true, o dispositivo deve ser incompatível quando não há nenhuma política de conformidade direcionada|
|enhancedJailBreak|Booliano|É o recurso habilitado ou não para maior detecção de jailbreak.|
|deviceInactivityBeforeRetirementInDay|Int32|Quando o dispositivo não check-in do número especificado de dias, os dados da empresa podem ser removidos e o dispositivo não estará sob gerenciamento. Valores válidos 30 a 270|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettings",
  "deviceComplianceCheckinThresholdDays": 1024,
  "isScheduledActionEnabled": true,
  "secureByDefault": true,
  "enhancedJailBreak": true,
  "deviceInactivityBeforeRetirementInDay": 1024
}
```





