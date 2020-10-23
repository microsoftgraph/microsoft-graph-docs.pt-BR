---
title: tipo de recurso windowsAutopilotSettings
description: O recurso windowsAutopilotSettings representa uma conta do Windows AutoPilot para sincronizar dados com o serviço de sincronização de dados do dispositivo Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 842a31f563306bdd07bbc4a10677aaa81e9415c8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694946"
---
# <a name="windowsautopilotsettings-resource-type"></a>tipo de recurso windowsAutopilotSettings

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso windowsAutopilotSettings representa uma conta do Windows AutoPilot para sincronizar dados com o serviço de sincronização de dados do dispositivo Windows.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter windowsAutopilotSettings](../api/intune-enrollment-windowsautopilotsettings-get.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Leia as propriedades e as relações do objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .|
|[Atualizar windowsAutopilotSettings](../api/intune-enrollment-windowsautopilotsettings-update.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Atualiza as propriedades de um objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .|
|[ação de sincronização](../api/intune-enrollment-windowsautopilotsettings-sync.md)|Nenhum|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O GUID do objeto.|
|lastSyncDateTime|DateTimeOffset|Data e hora da última sincronização de dados com o DDS Service.|
|lastManualSyncTriggerDateTime|DateTimeOffset|Data e hora da última sincronização de dados com o DDS Service.|
|syncStatus|[windowsAutopilotSyncStatus](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|Indica o status da sincronização com o serviço de DDS (sincronização de dados do dispositivo). Os valores possíveis são: `unknown`, `inProgress`, `completed`, `failed`.|

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





