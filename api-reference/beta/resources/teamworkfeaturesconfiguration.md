---
title: tipo de recurso teamworkFeaturesConfiguration
description: Representa os Microsoft Teams de configuração do cliente para um dispositivo Teams habilitado para Teams.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cbd95b2fa6a5c20126712abb63eaf00f8c065823
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262354"
---
# <a name="teamworkfeaturesconfiguration-resource-type"></a>tipo de recurso teamworkFeaturesConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os Microsoft Teams de configuração do cliente para um dispositivo Teams habilitado para [Teams cliente](../resources/teamworkdevice.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|emailToSendLogsAndFeedback|Cadeia de caracteres|Endereço de email para enviar logs e comentários.|
|isAutoScreenShareEnabled|Booliano|`True` se a tela automática compartilhada estiver habilitada.|
|isBluetoothBeaconingEnabled|Booliano|`True`se Bluetooth sinalizador está habilitado.|
|isHideMeetingNamesEnabled|Booliano|`True` se a ocultação de nomes de reunião estiver habilitada.|
|isSendLogsAndFeedbackEnabled|Boolean|`True` se o envio de logs e comentários estiver habilitado.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkFeaturesConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkFeaturesConfiguration",
  "emailToSendLogsAndFeedback": "String",
  "isAutoScreenShareEnabled": "Boolean",
  "isBluetoothBeaconingEnabled": "Boolean",
  "isHideMeetingNamesEnabled": "Boolean",
  "isSendLogsAndFeedbackEnabled": "Boolean"
}
```

