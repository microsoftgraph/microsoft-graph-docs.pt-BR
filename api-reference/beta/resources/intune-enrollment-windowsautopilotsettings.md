---
title: tipo de recurso de windowsAutopilotSettings
description: O recurso de windowsAutopilotSettings representa uma conta do Windows piloto automático aos dados de sincronização com o serviço de sincronização de dados de dispositivo do Windows.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7beb1f04efe3b43067eb1cedeed7071561265ce6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881542"
---
# <a name="windowsautopilotsettings-resource-type"></a>tipo de recurso de windowsAutopilotSettings

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

O recurso de windowsAutopilotSettings representa uma conta do Windows piloto automático aos dados de sincronização com o serviço de sincronização de dados de dispositivo do Windows.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter windowsAutopilotSettings](../api/intune-enrollment-windowsautopilotsettings-get.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Leia as propriedades e os relacionamentos do objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .|
|[Atualizar windowsAutopilotSettings](../api/intune-enrollment-windowsautopilotsettings-update.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Atualize as propriedades de um objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .|
|[ação de sincronização](../api/intune-enrollment-windowsautopilotsettings-sync.md)|Nenhum|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O GUID do objeto.|
|lastSyncDateTime|DateTimeOffset|Última dados sincronizar data hora com o serviço DDS.|
|lastManualSyncTriggerDateTime|DateTimeOffset|Última dados sincronizar data hora com o serviço DDS.|
|syncStatus|[windowsAutopilotSyncStatus](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|Indica o status da sincronização com o serviço de sincronização (DDS) de dados do dispositivo. Os valores possíveis são: `unknown`, `inProgress`, `completed`, `failed`.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "id": "String (identifier)",
  "lastSyncDateTime": "String (timestamp)",
  "lastManualSyncTriggerDateTime": "String (timestamp)",
  "syncStatus": "String"
}
```





