---
title: tipo de recurso teamworkSystemConfiguration
description: Representa os detalhes sobre a configuração do sistema para um dispositivo Microsoft Teams habilitado para uso.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dd22015f77cb65d2be52da8877f9808b73e2cac1
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262270"
---
# <a name="teamworksystemconfiguration-resource-type"></a>tipo de recurso teamworkSystemConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes sobre a configuração do sistema para um dispositivo Microsoft Teams habilitado para [uso.](../resources/teamworkdevice.md) Não aplicável para Salas do Microsoft Teams dispositivos.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|dateTimeConfiguration|[teamworkDateTimeConfiguration](../resources/teamworkdatetimeconfiguration.md)|As configurações de data e hora de um dispositivo.|
|defaultPassword|Cadeia de caracteres|A senha padrão do dispositivo. Somente gravação.|
|deviceLockTimeout|Duração|O tempo de tempo de bloqueio do dispositivo em segundos.|
|isDeviceLockEnabled|Booliano|`True` se o bloqueio do dispositivo estiver habilitado.|
|isLoggingEnabled|Booliano|`True` se o log estiver habilitado.|
|isPowerSavingEnabled|Boolean|`True` se a economia de energia estiver habilitada.|
|isScreenCaptureEnabled|Booliano|`True` se a captura de tela estiver habilitada.|
|isSilentModeEnabled|Boolean|`True` se o modo silencioso estiver habilitado.|
|idioma|Cadeia de caracteres|A opção de idioma do dispositivo.|
|lockPin|String|O pino que desbloqueia o dispositivo. Somente gravação.|
|loggingLevel|Cadeia de caracteres|O nível de registro em log do dispositivo.|
|networkConfiguration|[teamworkNetworkConfiguration](../resources/teamworknetworkconfiguration.md)|A configuração de rede do dispositivo.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkSystemConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkSystemConfiguration",
  "dateTimeConfiguration": {
    "@odata.type": "microsoft.graph.teamworkDateTimeConfiguration"
  },
  "defaultPassword": "String",
  "deviceLockTimeout": "String (duration)",
  "isDeviceLockEnabled": "Boolean",
  "isLoggingEnabled": "Boolean",
  "isPowerSavingEnabled": "Boolean",
  "isScreenCaptureEnabled": "Boolean",
  "isSilentModeEnabled": "Boolean",
  "language": "String",
  "lockPin": "String",
  "loggingLevel": "String",
  "networkConfiguration": {
    "@odata.type": "microsoft.graph.teamworkNetworkConfiguration"
  }
}
```

