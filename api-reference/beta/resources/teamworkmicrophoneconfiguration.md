---
title: tipo de recurso teamworkMicrophoneConfiguration
description: Representa os detalhes sobre a configuração do microfone para um Salas do Microsoft Teams dispositivo.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cd24375f573e9ff57a0cf9786aee26b1e0826c7c
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262249"
---
# <a name="teamworkmicrophoneconfiguration-resource-type"></a>tipo de recurso teamworkMicrophoneConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes sobre a configuração do microfone para um Salas do Microsoft Teams [dispositivo](../resources/teamworkdevice.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isMicrophoneOptional|Booliano|`True` se o microfone configurado for opcional. `False` se o microfone não for opcional e o estado de saúde do dispositivo deve ser calculado.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|defaultMicrophone|[teamworkPeripheral](../resources/teamworkperipheral.md)|Informações sobre o microfone padrão.|
|microfones|[coleção teamworkPeripheral](../resources/teamworkperipheral.md)|Uma coleção de microfones.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkMicrophoneConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkMicrophoneConfiguration",
  "isMicrophoneOptional": "Boolean"
}
```

