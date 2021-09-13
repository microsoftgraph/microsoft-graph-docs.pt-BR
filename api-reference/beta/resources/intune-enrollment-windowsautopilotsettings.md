---
title: Tipo de recurso windowsAutopilotSettings
description: O recurso windowsAutopilotSettings representa uma conta Windows Autopilot para sincronizar dados com Windows de sincronização de dados de dispositivo.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d79155c3642eee237fd4bda53ecb6650f5cfbe7e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039956"
---
# <a name="windowsautopilotsettings-resource-type"></a>Tipo de recurso windowsAutopilotSettings

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso windowsAutopilotSettings representa uma conta Windows Autopilot para sincronizar dados com Windows de sincronização de dados de dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter windowsAutopilotSettings](../api/intune-enrollment-windowsautopilotsettings-get.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Leia propriedades e relações do [objeto windowsAutopilotSettings.](../resources/intune-enrollment-windowsautopilotsettings.md)|
|[Atualizar windowsAutopilotSettings](../api/intune-enrollment-windowsautopilotsettings-update.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Atualize as propriedades de um [objeto windowsAutopilotSettings.](../resources/intune-enrollment-windowsautopilotsettings.md)|
|[ação de sincronização](../api/intune-enrollment-windowsautopilotsettings-sync.md)|Nenhum|Inicia uma sincronização de todos os dispositivos registrados do AutoPilot da Store para Empresas e de outros portais. Se a sincronização for bem-sucedida, essa ação retornará um código de resposta 204 No Content. Se uma sincronização já estiver em andamento, a ação retornará um código de resposta conflict 409.  Se essa ação de sincronização for chamada dentro de 10 minutos da sincronização anterior, a ação retornará um código de resposta 429 Solicitações Demais.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O GUID do objeto.|
|lastSyncDateTime|DateTimeOffset|Última data de sincronização de dados com o serviço DDS.|
|lastManualSyncTriggerDateTime|DateTimeOffset|Última data de sincronização de dados com o serviço DDS.|
|syncStatus|[windowsAutopilotSyncStatus](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|Indica o status da sincronização com o serviço de sincronização de dados de dispositivo (DDS). Os valores possíveis são: `unknown`, `inProgress`, `completed`, `failed`.|

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



