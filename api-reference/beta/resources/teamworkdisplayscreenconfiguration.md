---
title: tipo de recurso teamworkDisplayScreenConfiguration
description: Representa os detalhes sobre a configuração da tela de exibição para um dispositivo Microsoft Teams habilitado para uso.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2346de5fa301d1b2db7fd50e4a64c7168eea8a47
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262246"
---
# <a name="teamworkdisplayscreenconfiguration-resource-type"></a>tipo de recurso teamworkDisplayScreenConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represente os detalhes sobre a configuração da tela de exibição para um dispositivo Microsoft Teams habilitado [para uso.](../resources/teamworkdevice.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|backlightBrightness|Int32|O nível de brilho no dispositivo (0-100). Não aplicável para Salas do Microsoft Teams dispositivos.|
|backlightTimeout|Duração|Tempo de vida para backlight (30-3600 seg). Não aplicável para Salas do Teams dispositivos.|
|isHighContrastEnabled|Booliano|`True` se o modo de alto contraste estiver habilitado. Não aplicável para Salas do Teams dispositivos.|
|isScreensaverEnabled|Booliano|`True` se o screensaver estiver habilitado. Não aplicável para Salas do Teams dispositivos.|
|screensaverTimeout|Duração|Tempo de tempo do screensaver de 30 a 3600 seg. Não aplicável para Salas do Teams dispositivos.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkDisplayScreenConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDisplayScreenConfiguration",
  "backlightBrightness": "Integer",
  "backlightTimeout": "String (duration)",
  "isHighContrastEnabled": "Boolean",
  "isScreensaverEnabled": "Boolean",
  "screensaverTimeout": "String (duration)"
}
```

